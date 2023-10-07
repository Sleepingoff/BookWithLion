---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# SPA 무엇인가요?

신명진(AI)

💡 #SPA #Single Page Application 

## **답변 드리겠습니다!**

<aside>
📌 (275자)
Single Page Application 의 약자로 단일 페이지 애플리케이션이라고도 합니다. SPA는 서버로부터 현재 페이지에서 변경된 부분만 동적으로 다시 작성함으로써 사용자와 소통하는 방식의 애플리케이션입니다. 이를 CSR(Client Side Rendering)이라고 하는데, 처음에 한 번 페이지를 전체 로딩 한 후 이후부터는 바뀐 데이터 부분만 변경해서 렌더링 하기 때문에 매번 전체 렌더링 하는 것보다 효율적입니다. 전체 트래픽 양이 감소하고 렌더링 속도가 빨라진다는 장점이 있지만 검색이 잘되지 않는다는 단점이 있습니다.

</aside>

Single Page Application 의 약자로 단일 페이지 애플리케이션이라고도 합니다. SPA는 서버로부터 완전한 새 페이지를 불러오지 않고 현재 페이지를 동적으로 다시 작성함으로써 사용자와 소통하는 방식의 애플리케이션입니다. 이를 CSR(Client Side Rendering) 방식으로 렌더링이라고 합니다. 그러나모든 SPA가 CSR 방식을 사용하는 것은 아닙니다.
 SPA는 처음에 한 번 서버로부터 정적 리소스를 요청합니다. 그리고 받은 데이터는 전부 캐시에 저장합니다. 이후부터는 사용자의 요청으로 바뀐 데이터 부분만 변경해서 렌더링 하기 때문에 매번 전체를 렌더링 하는 것보다 효율적입니다. 

  장점으로는 속도가 빨라 깜빡거림이 없어 자연스러운 사용자 경험을 제공할 수 있습니다. 필요한 리소스만 로딩하기 때문에 성능이 우수합니다. 서버의 템플릿 연산을 클라이언트로 분산하여 효율적입니다. 컴포넌트 별로 개발이 가능해지므로 생산성이 향상됩니다. 모바일 앱 개발 시 동일한 API를 사용하도록 설계할 수 있습니다.

 단점으로는 JavaScript 파일을 번들링해서 한 번에 받기 때문에 초기 구동 속도가 느립니다.(Webpack의 code splitting으로 해결) 검색엔진최적화(SEO)가 어렵습니다. (SSR로 해결) SSR에서는 사용자에 대한 정보를 서버측에서 세션으로 관리를 하지만 CSR 방식에서는 클라이언트 측의 쿠키말고는 사용자에 대한 정보를 저장할 공간이 없습니다.  이 때문에 보안 이슈가 발생할 수 있습니다. (프론트엔드에 비즈니스 로직 최소화로 해결) 스크립트 언어로 화면의 전환이 이루어지므로 잘 만들어진 검색 엔진이 아니면 크롤링 하기 어렵습니다. 위 같은 단점을 보완할 수 있는 React.js, Vue.js, Angular.js 등의 자바스크립트 라이브러리를 사용합니다.

![Untitled](Untitled%2050.png)

![Untitled](Untitled%2051.png)

## **이런 질문도 나올 수 있어요!**

### MPA(Multiple Page Application)

여러 개의 페이지로 구성된 애플리케이션입니다. MPA는 SSR(Server Side Application) 방식으로 렌더링 합니다. 새로운 페이지를 요청할 때마다 서버에서 렌더링 된 정적 리소스(HTML, CSS, JavaScript)가 다운로드 됩니다. 페이지를 이동하거나 새로고침 하면 전체 페이지를 다시 렌더링 합니다.

![Untitled](Untitled%2052.png)

참고

[싱글 페이지 애플리케이션 - 위키백과, 우리 모두의 백과사전 (wikipedia.org)](https://ko.wikipedia.org/wiki/%EC%8B%B1%EA%B8%80_%ED%8E%98%EC%9D%B4%EC%A7%80_%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98)

[SPA (Single Page Application) 이란 무엇인가? (tistory.com)](https://memostack.tistory.com/51)

[SPA(Single Page Application) 이란? 개요/장점/단점 (tistory.com)](https://doctorson0309.tistory.com/157)