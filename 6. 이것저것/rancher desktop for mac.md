### 크로스 플랫폼 적용
- 빌드 중 shell 오류 발생 시 크로스 플랫폼 적용이 되지 않아 에러가 발생한다.
- 아래와 같이 컨테이너를 실행하면 크로스 플랫폼이 적용되어 빌드되어 진다.
```sh
docker run --privileged --rm tonistiigi/binfmt --install all

installing: s390x OK                                                             
installing: ppc64le OK                                                           
installing: riscv64 OK                                                           
installing: mips64le OK                                                          
installing: mips64 OK                                                            
installing: arm OK                                                              
installing: 386 OK                                                               
installing: loong64 OK                                                           

{                                                                               
  "supported": [                                                                 
    "linux/arm64",                                                               
    "linux/amd64",                                                               
    "linux/amd64/v2",                                                            
    "linux/riscv64",                                                             
    "linux/ppc64le",                                                             
    "linux/s390x",                                                               
    "linux/386",                                                                 
    "linux/mips64le",                                                            
    "linux/mips64",                                                              
    "linux/loong64",                                                             
    "linux/arm/v7",                                                              
    "linux/arm/v6"                                                               
  ],                                                                             
  "emulators": [                                                                 
    "qemu-arm",                                                                  
    "qemu-i386",                                                                 
    "qemu-loongarch64",                                                          
    "qemu-mips64",                                                               
    "qemu-mips64el",                                                             
    "qemu-ppc64le",                                                              
    "qemu-riscv64",                                                              
    "qemu-s390x",                                                                
    "qemu-x86_64"                                                                
  ]                                                                              
}
```

### docker.sock 위치
* rancher desktop을 사용해 Docker를 사용하는 경우 Docker desktop과 다른 docker.sock 경로를 가진다.
	> ~/.rd/docker.sock

`sudo ln -s ~/.rd/docker.sock /var/run/docker.sock` 을 입력해 docker desktop과 동일한 경로로 링크를 걸면 된다.
