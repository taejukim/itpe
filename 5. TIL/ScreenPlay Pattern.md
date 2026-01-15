POM과 다른 디자인패턴
Page 요소를 주로 다루는 POM과 다르게 User의 동작을 주로 다루는 ScreenPlay라는 패턴이 있음

- POM
	- Page class
	- Test class
- ScreenPlay
	- Actor
	- Task
	- UI
	- Test

POM의 경우 중복 코드가 발생하고 Page class 하나가 사이즈가 커질 수 있음
ScreenPlay의 경우 중복코드를 최소화 하고 동작 하나하나를 잘게 쪼개어 관리하기 때문에 Class의 크기가 커지지 않고 유지보수하기 상대적으로 유리 할 수 있음
