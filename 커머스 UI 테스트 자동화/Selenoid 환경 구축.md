## 필요 항목
* selenoid, selenoid-ui 컨테이너가 필요
* selenoid:
	* 이미지 : aerokube/selenoid:latest
	* 필요 볼륨 : 
		* video : ./video:/opt/selenoid/video
		* log :  ./logs:/opt/selenoid/logs
		* docker.sock : /var/run/docker.sock:/var/run/docker.sock
		* browser.json : ./browsers.json:/etc/selenoid/browsers.json:ro
* selenoid-ui:
	* 이미지 : aerokube/selenoid-ui:latest
* 네트워크 통일
* 