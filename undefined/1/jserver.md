# \[1주차 JavaHttpServer, SpringMVC]

## HTTPServer을 이용하여 서버 구현 

> InetSoketAddress \n
> HTTPServer \n
> exchange와 람다식 활용

### 배운 것

1. InetSocket으로 포트를 열고 HttpServer를 통해서 서버를 만들어준다 
2. createContext메소드를 실행하면서 path를 줄 수 있고, exchange와 람다를 활용하여 Request와 Response를 구현할 수 있다. 
3.인텔리제이의 refactor의 extract Method를 통해 메소드 구현이 가능하다 

### 어려웠던 것

localhost:8080접속이 되지않는 문제가 생김 
Task :app:processResources NO-SOURCE 해당 문구가 오류인 줄 알아서 이것저것 찾다가 시간을 많이 소모하였음.. 
원인은 보여줄 내용이 없어서 접속이 차단되는거였다...
Request 및 response코드를 입력하니 접속이 아주 잘됨..ㅠㅠ

### 오늘 진행한 것

강의를 보면서 콘솔에서 idea . 으로 인텔리제이를 바로 실행하는 게 궁금하여 찾아보고 적용시켰다 이전 데브노트에서 빌드가 되지않았던 문제를 다른 방법으로 해결한 것 같아 뿌듯하다

### [1주차 SpringMVC]

드디어 익숙한 스프링을 보게 되었다 
MVC패턴이란 Model - View - Controller로 이루어진 패턴이다 

내가 알고있는 MVC는 아래와 같다 
> *Controller* - 사용자가 입력한 데이터를 입력받아 Model의 데이터처리 및 결과값을 View로 전송한다 \n 
> *Model* - Controller에서 입력받은 데이터를 처리한다 \n
> *View* - 사용자에게 처리된 데이터를 보여준다

본인은 국비과정에서 
*@Controller* \n 
*@RequestMapping("/member/")* \n

*@GetMapping("regist")* \n
이런식으로 많이 사용을 했다 
localhost:8080/member/regist주소로 가면 registForm으로 이동하게끔 만들었었다

스프링은 새로 알게된 내용은 없어서 배운 것, 어려웠던 것을 생략한다