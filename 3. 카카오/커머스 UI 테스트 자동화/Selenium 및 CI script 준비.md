### 웹브라우저 버전 선택
* Jenkins pipeline을 이용해 test를 실행할 예정이다
* 해당 job을 수행할때 choice parameter를 사용해 넘겨주는 chrome 버전을 사용해 테스트가 이뤄져야 한다.
### Selenoid 사용
* Docker-compose를 사용해 Selenoid, Python(Pytest, Selene) 컨테이너를 두개 띄워야 한다.
* 해당 작업은 jenkins pipeline에서 담당한다.
* 현재 CI Script는 아래와 같이 Pytest 프로젝트를 실행한다. 
```groovy
// pytest.groovy
// Docker Compose 템플릿 로드
def composeTemplate = libraryResource 'selenium/docker-compose.python-basic.yml'
def dockerfilePython = libraryResource 'selenium/Dockerfile.python-basic'
                    
// Docker Compose 파일 작성
writeFile file: 'docker-compose.yml', text: composeTemplate
writeFile file: 'Dockerfile.python-basic', text: dockerfilePython
		
// 빌드 및 시작
sh docker compose up --build -d
	    
// 테스트 시작
sh '''
	docker compose run --rm \\
		${envFlags.join(' ')} \\
		app poetry run pytest ${nodeOption} ${config.testPath} \\
			--capture=tee-sys \\
			--junit-xml=${junitReport} \\
			--alluredir=allure-results \\
			--clean-alluredir
'''
```

```dockerfile
# Dockerfile.python-basic
FROM idock.daumkakao.io/service_qa/poetry_image:3.13

COPY pyproject.toml poetry.lock* ./
RUN poetry install --no-interaction --no-root

COPY . .

CMD [ "tail", "-f", "/dev/null"]

```

```yml
# docker-compose.python-basic.yml
services:
  app:
    build:
      context: .
      dockerfile: Dockerfile.python-basic
    volumes:
      - ./allure-results:/app/allure-results:rw
    environment:
      - PYTHONUNBUFFERED=1
    working_dir: /app
    # 컨테이너 이름에 빌드 번호 포함하여 충돌 방지
    container_name: "test-app-${BUILD_NUMBER:-latest}"
```
### 예상되는 결과
- 별도 폴더에 selenoid를 위한 Dockerfile 및  poetry_image와 함께 실행할 수 있는 docker-compose.yml 파일이 나와야 합니다.
- Selenoid를 위한 browsers.json 파일도 있어야 합니다.
	- 현재는 chrome 최신 버전만 고려하고 있습니다.
- Jenkins pipeline을 위한 groovy 파일이 나와야 합니다.
	- /var/selenoid_test.groovy 로 명명해주세요
	- 
* Selenoid docker file을 가지고 디버깅을 위해 local 환경에서도 수행할 수 있어야 합니다.
	* 빠르게 띄울수 있도로 .sh 파일 또는 Python 파일을 만들어주세요.