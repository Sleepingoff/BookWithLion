# !DOCTYPE이 무엇인지 설명하시오.

임연정

💡 #문서 유형 정의 #DTD #렌더링 모드

## **답변 드리겠습니다!**

<aside>
📌 `**!DOCTYPE**`은 HTML 문서의 첫 번째 줄에 위치해야 하며, 문서의 버전과 유형을 정의하는 HTML 태그입니다. 문서 해석 및 렌더링 하는데 필수적인 정보를 웹브라우저로 전달합니다. 같은 내용의 HTML 문서라도 `**!DOCTYPE**`을 선언하지 않는다면 브라우저 환경에 따라 전혀 다른 결과물이 발생할 수 있습니다. 각 브라우저는 문서 간의 호환성을 높이고, HTML 문서를 동일하게 인식할 수 있게 선언합니다.

</aside>

  document type의 약어로 `**!doctype**`이며 선언은 `**<!DOCTYPE html>**` 로 작성됩니다. 문서 타입 정의*(DTD: Document Type Definition)*는 HTML, XHTML, HTML5, 세 가지 문서 유형이 존재하며, 유형에 따라 마크업 문서의 요소와 속성들을 처리하는 기준이 되어 유효성 검사에 이용됩니다.    

  SGML*(Standard Generalized Markup Language)*에 기반한 이전의 HTML 과는 다르게 HTML5에선 SGML에 기반을 두지 않아 DTD 참조가 필요 없기 때문에 간단히 선언할 수 있습니다. 따라서 `**!doctype**` 선언은 선택적이지만 하위 호환성을 위해 사용하는 것이 좋습니다. `**!doctype**` 선언은 대소문자를 구분하지 않으며, 선언 이후에는 HTML 문서의 모든 요소와 태그가 정확한 방식으로 작성되어야 합니다. 이를 통해 웹 브라우저는 문서를 올바르게 해석하여 사용자에게 적절한 화면을 제공할 수 있습니다.

## **이런 질문도 나올 수 있어요!**

### **!DOCTYPE을 선언하지 않으면 어떻게 되나요?**

  `**!DOCTYPE**`을 선언하지 않으면 브라우저는 문서를 비표준 모드로 해석합니다. 이는 브라우저가 문서를 렌더링 하는 방식을 이전 버전의 HTML과 호환되도록 조정하는 것을 의미합니다. `**!DOCTYPE**`을 선언하지 않으면 예상치 못한 렌더링 결과가 발생하여 특정 기능이 동작하지 않을 수도 있으며 크로스 브라우징에 어려움을 겪게 될 수 있습니다. 따라서 `**!DOCTYPE**`을 선언하여 문서의 표준 모드로 브라우저가 해석하도록 하는 것이 좋습니다.

## **만반의 준비! 이것도 알아둘까요?**

### 렌더링 모드의 종류

  렌더링 모드란 웹페이지를 읽는 방식으로, 웹 표준에 따라 다양한 웹브라우저에서 웹페이지를 올바르게 표시할 수 있게 합니다. 렌더링 모드에는 표준모드*(standard mode)*와 비표준 모드*(quirks mode)*, 거의 표준모드*(almost standard mode)* 또는 엄격 모드*(strict mode)*가 존재합니다.

  표준모드는 `**!DOCTYPE**`을 선언하여 실행되며 웹 표준에 따라 렌더링 됩니다.

  비표준 모드는 `**!DOCTYPE**`을 선언하지 않았을 때 실행되며 예전 브라우저처럼 렌더링 되어 올바르지 못하게 표현됩니다.

---

출처: 

[(HTML) DOCTYPE (velog.io)](https://velog.io/@yunsungyang-omc/HTML-DOCTYPE)

[문서 유형 (Doctype) | JETT Analysis](https://ssd0908.tistory.com/entry/HTML-DOCTYPE-%EC%84%A0%EC%96%B8-%EC%9D%98%EB%AF%B8-%EB%B0%8F-%ED%98%84%EC%9E%AC%EB%8A%94-%EC%96%B4%EB%96%BB%EA%B2%8C-%EC%82%AC%EC%9A%A9%ED%95%98%EB%8A%94%EA%B0%80)

[DOCTYPE이란 도대체 무엇인가? : 네이버 블로그 (naver.com)](https://m.blog.naver.com/redtaeung/221929431362)

[(Web) DTD(Document Type Definition)란? | by Su Bak | Medium](https://medium.com/@su_bak/web-dtd-document-type-definition-%EB%9E%80-1a1413771189)

[코딩의 시작, TCP School](http://www.tcpschool.com/html-tags/doctype)