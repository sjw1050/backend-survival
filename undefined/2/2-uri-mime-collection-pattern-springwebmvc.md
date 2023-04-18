# \[2주차 URI/MIME/Collection Pattern/SpringWebMVC]

#### URI란?

* 리소스를 식별하는 방법
* URI에는 URL, URN이 있으나 대부분 URL을 사용하여 거의 동의어에 가깝다

#### MIME Type(Content Type, Media Type)

* 강의를 수강 전 본인이 알던 MIME Type은 text/html, text/css, text/javascript, application/xml, application/json정도이다
* 여기에 한가지를 추가 한 text/plain이 있다 text/plain은 주로 Email에서 자주 사용했다고 한다

#### Collection Pattern

* 여러리소스를 하나의 그룹으로 묶을 수 있다 **ex) /members/{id}** {id}는 Post ID라고 부른다
* !! Post ID와 리소스를 식별하는 ID는 다르다

**ex) /members?member\_id={member\_id}** 이런식으로 사용도 가능한데 이건 국비과정에서 프로젝트할 떄 자주쓰던거라 본인에게도 많이 익숙하다

또한 그룹이 아니면 단수형의 사용이 가능하다

* /session - 세션은 하나만 유지되고, 다른세션을 참고할 일이 없다

#### CRUD

드디어 익숙한 단어가 나왔다 바로 CRUD에 대해 설명하겠다

* Create / Read / Update / Delete이다

> Http 메소드와 같이 설명하겠다
>
> * Create - POST - **ex) POST /members** ㄴ 회원가입이라고 보면 된다 본인은 members/regist 이런식으로 많이 사용하였다
> * Read - GET - **ex) GET /members** ㄴ 멤버의 목록을 보여준다
> * Update - PUT, PATCH **ex) /members/{id}** ㄴ id에 해당하는 멤버를 업데이트(회원수정)한다
> * Delete - DELETE **ex) /members/{id}** ㄴ id에 해당하는 멤버를 삭제한다(회원탈퇴) 이런 식으로 표현이 가능하다

#### CQS란 무엇인가?

* CRUD를 중요한 특징에 따라 분류한다 - Command / Query로 나뉜다

1. Command (Create, Update, Delete) : 상태가 변하여 안전성이 떨어진다
2. Query (Read) - 상태가 변하지 않아 안전하다

**Spring WebMVC의 내용은 이미 알고있고, 추가로 알게된 부분만 작성한다**

#### 배운 것

* CQS란 무엇인가에 대해 알게 되었다
* CRUD는 이미 익숙하고 알고 있지만 한번 더 복습하는 개념으로 공부되었다
* CollectPattern을 사용했지만 Collection Pattern인지 모르고 사용하였다
* Spring Web MVC에서 ExceptionHandler에 대해 알게되었다

#### 어려웠던 것

* 이번 강의에서는 이해가 안가거나 어려운 것은 없었다

#### 느낀 점

* 국비과정을 수료하면서 사용하던 것들이 어떤 역할을 가지고 있는지 또는 어떤 패턴을 사용하는지 전혀 몰랐던 것에 대하여 나의 무의식이 행하고 있던 무지함을 반성하게 되었다
* 기본 개념에 대한 공부를 조금 더 해야 할 것 같다고 느꼈다.
