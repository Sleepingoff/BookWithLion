---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# cors란 무엇인가요?

김모건

💡 #웹 개발 #CORS 대처법 #CORS 우회법

## **답변 드리겠습니다!**

<aside>
📌 `**CORS**`*(Cross-Origin Resource Sharing)*란 교차 출처 리소스 공유라는 의미로, 웹 애플리케이션이 다른 출처의 리소스에 접근할 수 있도록 브라우저와 서버가 협력하는 방식입니다.

CORS에 대처하는 방법은 서버 측에서 허용하는 **`Origin`**, 메서드, 헤더 등을 응답 헤더에 명시하는 것 입니다. CORS를 우회하는 방법은 프록시 서버를 사용하거나 `**JSONP**`와 같은 기법이 있습니다. 프록시 서버는 요청을 중계하고 응답을 수정하여 CORS 오류를 방지합니다. JSONP는 스크립트 태그를 사용하여 JSON 데이터를 콜백 함수로 감싸서 전달하는 방식입니다. 

</aside>

  CORS는 한 출처(*Origin*)에서 실행되는 웹 애플리케이션이 다른 출처의 리소스에 접근할 수 있도록 허용하는 메커니즘입니다. 예를 들어, A.com에서 실행되는 스크립트가 B.com의 API를 호출하는 경우, CORS가 필요합니다. CORS는 보안을 위해 `**동일 출처 정책**`*(SOP: Same Origin Policy)*을 따르는 브라우저에서 교차 출처 요청을 제한하기 때문에 발생하는 문제입니다. 따라서 CORS에 대처하는 방법과 우회하는 방법을 알아야 합니다.

  브라우저는 `**XMLHttpRequest**`나 `**Fetch API**`와 같은 API를 사용하여 교차 출처 요청을 보냅니다. 이때 요청 헤더에 protocol, hostname, port를 포함하는 Origin이라는 필드에 요청을 보내는 출처를 담습니다. 서버는 요청을 받고, 응답 헤더에 `**Access-Control-Allow-Origin**`이라는 필드에 허용하는 출처를 담아서 보냅니다. 이때 전체선택자(`***`)**를 사용하면 모든 출처를 허용하고, 특정 출처를 명시하면 해당 출처만 허용합니다. 브라우저는 응답 헤더를 확인하고, 요청한 출처가 허용된 출처에 포함되면 응답을 처리하고, 그렇지 않으면 오류를 발생시킵니다.

## **이런 질문도 나올 수 있어요!**

### CORS에 대처하는 방법을 구체적으로 설명해주세요.

  서버 측에서 응답 헤더에 CORS 관련 필드를 추가하여 브라우저에게 교차 출처 요청을 허용한다고 알려줍니다. 예를 들어, 다음과 같은 헤더들이 있습니다. 

   `**Access-Control-Allow-Origin**` : 허용하는 출처를 명시합니다. * 를 사용하면 모든 출처를 허용합니다. 

  `**Access-Control-Allow-Methods**` : 허용하는 HTTP 메서드(GET, POST, PUT, DELETE 등)를 명시합니다.

  `**Access-Control-Allow-Headers**` : 허용하는 HTTP 헤더를 명시합니다. Content-type, Authorization 등이 있습니다. 

  `**Access-Control-Allow-Credentials**` : 인증 정보(쿠키, HTTP 인증)를 함께 보낼 수 있도록 허용하는지 여부를 명시합니다. true 또는 false 값을 가집니다. 

  서버 측에서는 요청 메서드가 `**GET**`, `**HEAD**`, `**POST**`가 아니거나, 특정 헤더나 인증 정보를 포함하는 요청에 대해서는 `**Preflight Request**`를 받습니다. 이는 실제 요청을 보내기 전에 OPTIONS 메서드로 요청을 보내서 서버의 요청 권한 허용 여부를 미리 확인하는 것 입니다. 서버는 Preflight Request에 대해서도 CORS 관련 헤더를 응답해야 합니다.

### CORS를 우회하는 방법에 대해 구체적으로 설명해주세요.

  `**Proxy**` 서버를 사용하여 요청을 중계하고 응답을 수정하는 방법이 있습니다. 예를 들어, A.com에서 B.com의 API를 호출하려고 하는데 CORS 오류가 발생한다면, C.com이라는 프록시 서버를 만들고, A.com에서는 C.com에 요청을 보내고, C.com에서는 B.com에 요청을 보내고, B.com에서 받은 응답에 

```jsx
Access-Control-Allow-Origin: *
```

 라는 헤더를 추가하여 A.com에 전달하는 방식입니다.

 또 JSONP*(JSON with Padding)* 라는 기법을 사용하는 방법이 있습니다. 이는 스크립트 태그의 src 속성을 사용하여 교차 출처 리소스를 불러오는 방법입니다. 스크립트 태그는 CORS 정책의 제약을 받지 않으므로, JSON 데이터를 콜백 함수로 감싸서 전달할 수 있습니다. 예를 들어, A.com에서 B.com의 API를 호출하려고 하는데 CORS 오류가 발생한다면, 다음과 같은 코드를 사용할 수 있습니다.

```jsx
<script src=“B.com/api?callback=foo”></script>
```

이때 B.com의 API는 `**foo({“data”: “some data”})**` 와 같은 형식으로 응답해야 합니다. 그러면 A.com에서 foo라는 함수를 정의하고, 그 함수 안에서 JSON 데이터를 처리할 수 있습니다.

## **만반의 준비! 이것도 알아둘까요?**

### CORS의 Origin 의 의미

protocol + hostname + port

![Untitled](Untitled%2049.png)

출처: 유튜브, 클돌의 터전  [https://www.youtube.com/watch?v=j2Q2Ev6CZzQ&t=92s](https://www.youtube.com/watch?v=j2Q2Ev6CZzQ&t=92s)

### 어떤 상황에서 CORS Error 를 만날 수 있나요?

개발 중에 포트 번호가 다른 서버와 클라이언트 서버 간의 데이터 송수신에 발생할 수 있습니다. 

### SOP(Same Origin Policy)

동일 출처 정책. 악의적 사용자의 하이제킹(Hijacking)을 방지하기 위하여, 같은 Origin 간의 접근 요청 및 데이터만 송수신을 허용한다.

### Localhost

현재 기기의 hostname 으로 127.0.0.1 을 가리킨다.

### White List

서버 측에서 접근을 허용하는 클라이언트(origin)

### Preflight Request

브라우저가 Simple Request 가 아닌 PUT, DELETE 와 같은 요청에 대해 사전에 Preflight request option 메서드로 CORS 인지 여부를 확인하는 요청을 보내게 된다.

---

💡 #웹 개발 #CORS*(Cross-Origin Resource Sharing)* 문제

## **답변 드리겠습니다!**

<aside>
📌 CORS란 교차 출처 리소스 공유라는 의미로, 웹 애플리케이션이 다른 출처의 리소스에 접근할 수 있도록 브라우저와 서버가 협력하는 방식입니다.

CORS에 대처하는 방법은 서버 측에서 허용하는 출처와 메서드, 헤더 등을 응답 헤더에 명시하는 것입니다. 예를 들어, Access-Control-Allow-Origin, Access-Control-Allow-Methods, Access-Control-Allow-Headers 등의 헤더를 사용합니다.

CORS를 우회하는 방법은 프록시 서버를 사용하거나 JSONP와 같은 기법을 사용하는 것입니다. 프록시 서버는 요청을 중계하고 응답을 수정하여 CORS 오류를 방지합니다. JSONP는 스크립트 태그를 사용하여 JSON 데이터를 콜백 함수로 감싸서 전달하는 방식입니다. 

</aside>

 CORS는 한 출처에서 실행되는 웹 애플리케이션이 다른 출처의 리소스에 접근할 수 있도록 허용하는 메커니즘입니다. 예를 들어, A.com에서 실행되는 스크립트가 B.com의 API를 호출하는 경우, CORS가 필요합니다. CORS는 보안을 위해 동일 출처 정책*(SOP: Same Origin Policy)*을 따르는 브라우저에서 교차 출처 요청을 제한하기 때문에 발생하는 문제입니다. 따라서 CORS에 대처하는 방법과 우회하는 방법을 알아야 합니다.

## **이런 질문도 나올 수 있어요!**

### CORS는 다음과 같은 과정으로 동작합니다.

- 브라우저는 XMLHttpRequest나 Fetch API와 같은 API를 사용하여 교차 출처 요청을 보냅니다. 이때 요청 헤더에 Origin이라는 필드에 요청을 보내는 출처를 담습니다.
- 서버는 요청을 받고, 응답 헤더에 Access-Control-Allow-Origin이라는 필드에 허용하는 출처를 담아서 보냅니다. 이때 * 를 사용하면 모든 출처를 허용하고, 특정 출처를 명시하면 해당 출처만 허용합니다.
- 브라우저는 응답 헤더를 확인하고, 요청한 출처가 허용된 출처에 포함되면 응답을 처리하고, 그렇지 않으면 오류를 발생시킵니다.

### CORS에 대처하는 방법은 다음과 같습니다.

- 서버 측에서 응답 헤더에 CORS 관련 필드를 추가하여 브라우저에게 교차 출처 요청을 허용한다고 알려줍니다. 예를 들어, 다음과 같은 헤더들이 있습니다.
    - Access-Control-Allow-Origin: 허용하는 출처를 명시합니다. * 를 사용하면 모든 출처를 허용합니다.
    - Access-Control-Allow-Methods: 허용하는 HTTP 메서드를 명시합니다. GET, POST, PUT, DELETE 등이 있습니다.
    - Access-Control-Allow-Headers: 허용하는 HTTP 헤더를 명시합니다. Content-Type, Authorization 등이 있습니다.
    - Access-Control-Allow-Credentials: 인증 정보(쿠키, HTTP 인증)를 함께 보낼 수 있도록 허용하는지 여부를 명시합니다. true 또는 false 값을 가집니다.
- 서버 측에서는 요청 메서드가 GET, HEAD, POST가 아니거나, 특정 헤더나 인증 정보를 포함하는 요청에 대해서는 프리플라이트 요청이라는 것을 받습니다. 이는 실제 요청을 보내기 전에 OPTIONS 메서드로 요청을 보내서 서버의 허용 여부를 미리 확인하는 것입니다. 서버는 프리플라이트 요청에 대해서도 CORS 관련 헤더를 응답해야 합니다.

### CORS를 우회하는 방법은 다음과 같습니다.

- 프록시 서버를 사용하여 요청을 중계하고 응답을 수정하는 방법입니다. 예를 들어, A.com에서 B.com의 API를 호출하려고 하는데 CORS 오류가 발생한다면, C.com이라는 프록시 서버를 만들고, A.com에서는 C.com에 요청을 보내고, C.com에서는 B.com에 요청을 보내고, B.com에서 받은 응답에 Access-Control-Allow-Origin: * 라는 헤더를 추가하여 A.com에 전달하는 방식입니다.
- JSONP(JSON with Padding)라는 기법을 사용하는 방법입니다. 이는 스크립트 태그의 src 속성을 사용하여 교차 출처 리소스를 불러오는 방법입니다. 스크립트 태그는 CORS 정책의 제약을 받지 않으므로, JSON 데이터를 콜백 함수로 감싸서 전달할 수 있습니다. 예를 들어, A.com에서 B.com의 API를 호출하려고 하는데 CORS 오류가 발생한다면, 다음과 같은 코드를 사용할 수 있습니다.
    - <script src=“B.com/api?callback=foo”></script>
    - 이때 B.com의 API는 foo({“data”: “some data”})와 같은 형식으로 응답해야 합니다.
    - 그러면 A.com에서 foo라는 함수를 정의하고, 그 함수 안에서 JSON 데이터를 처리할 수 있습니다.

## **만반의 준비! 이것도 알아둘까요?**

### **제목 heading3**

내용