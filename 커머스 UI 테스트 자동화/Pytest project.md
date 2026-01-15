### 폴더 구조
```sh
├── conf                                                                         
│   ├── beta.py      # 베타 환경에 URL 및 계정 정보
│   └── sandbox.py   # 샌드박스 환경에 URL 및 계정 정보                  
├── conftest.py      # Project 전역 conftest.py(project root 정의)├── poetry.lock  
├── pyproject.toml                                                               
├── README.md                                                                    ├── .env                                                                   
├── src                                                                          
│   ├── api          # UI 테스트에서 활용할 API Wrapper class                        
│   ├── pages        # Page class                                                
│   │   ├── base_page.py                                                         
│   │   ├── order_gift_list_page.py                                              
│   │   ├── order_gift_detail_page.py     
│   │   ├── gift_inbox_page.py     
│   │   ├── gift_inbox_detail_page.py                                            
│   │   └── giftbox_main_page.py                                                 
│   ├── project.py    # conf 환경에 맞는 모든 정보를 들고 있는 Class (singleton)
│   ├── apis.py       # API 모음 class    
│   ├── http_request_adapter.py # http(header 주입, GET, POST 등) 어댑터 클래스
│   ├── login.py      # 로그인 기능 class (get session, get gtkn)                  
│   ├── properties.py # 환경에 맞는 conf의 정보를 수집하는 class (singleton)            
│   ├── testbase.py   # 모든 테스트에서 상속 받는 base class(before, after, 공통)       
│   └── utils                                                                    
└── tests                                                                        
    ├── gift 
	│   └── basic_test.py  # 기본 로그인 후 페이지 로드 테스트     
    └── ...                                                                 
```
