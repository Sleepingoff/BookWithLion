---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# AI 답변) 반응형 웹의 3요소에 대해 설명해주세요.

임연정(답변) 우준하(1차 수정 완료)

💡 #그리드 레이아웃 #가변형 이미지 #미디어 쿼리

## **답변 드리겠습니다!**

<aside>
📌 부모 요소에 **`display: grid`** 속성을 추가하는 **그리드 레이아웃**과 **`max-width`**, **`width`**, **`min-width`** 등을 이용하여 화면 크기에 따라 높이와 너비가 바뀌는 **가변형 이미지**가 있습니다. 마지막으로 화면, 티비, 프린터와 같은 미디어 타입과 적어도 하나 이상의 표현식으로 구성되는 **미디어 쿼리**가 있습니다.

</aside>

미디어 쿼리는 CSS3에 포함되어 있으며 화면의 크기가 바뀌어도 컨텐츠의 변경 없이 스타일 시트를 달리 적용하여 적절한 모양을 보여줄 수 있습니다.

반응형 웹은 하나의 웹 사이트 화면이 PC, 스마트폰, 태블릿 PC 등 접속하는 디스플레이의 종류에 따라 화면의 크기가 자동으로 변하도록 만든 웹페이지 접근 기법입니다. 반응형 웹과 적응형 웹은 비슷한 목적을 가지고 있지만, 반응형 웹은 하나의 웹 페이지에서 모든 기기에 대해 최적화된 화면을 제공하는 반면, 적응형 웹은 사용자의 기기 및 해상도의 정보를 미리 받아서 조건에 맞는 화면을 보여주는 것입니다.

## **이런 질문도 나올 수 있어요!**

### 반응형 웹을 만들기 위해 사용하는 단위에 대해 설명해주세요.

반응형 웹을 만들기 위해서는, 먼저 **`meta`** 태그에 `name="viewport"`와 `conetent` 속성을 추가해야 합니다. 이를 통해 뷰포트(viewport)의 크기를 설정할 수 있습니다. 대표적으로 사용되는 단위로는 다음과 같은 것들이 있습니다.

**px**: 절대적인 크기를 나타내는 단위입니다. 고정된 값이어서 사용하기 편하지만 반응형 웹에는 적절하지 않습니다.

**rem**: 기본 폰트 사이즈가 있다면, 1rem은 기본 폰트 사이즈와 같습니다. 기본 폰트 사이즈가 없다면, 1rem은 16px과 같습니다.

**em**: 부모 요소의 폰트 사이즈를 기준으로 합니다.

**%**: 부모 요소의 크기를 기준으로 합니다.

### 반응형 웹을 사용하는 이유에 대해 설명해주세요.

- 간편한 유지 보수

반응형 웹은 유지 보수가 간편합니다. 모바일과 테스크톱 버전을 따로 만들어 두 개의 웹사이트를 만들게 되면 웹사이트를 수정하거나 새로운 내용이 추가될 때 개별적으로 추가 및 수정이 필요합니다. 하지만 반응형 웹은 화면에 따라 달라지는 모든 디자인을 하나의 HTML 파일과 CSS 파일에서 작업하기 때문에 유지 보수가 비교적 쉽습니다.

- 최적화된 검색 엔진

반응형 홈페이지는 하나의 주소로 검색 결과에 좀 더 노출이 잘 될 수 있고, 동일한 URL이 모든 디바이스에서 작동하므로 사용자 경험이 향상됩니다.

- 유리한 마케팅

반응형 웹이라는 기술을 이용하여 웹사이트를 개발하면 환경이나 기기에 맞춰지는 최적화된 구조로 웹사이트를 변경하여 보여줄 수 있습니다.

## **만반의 준비! 이것도 알아둘까요?**

### VH/VW (viewport height/ viewport width)이란?

**vh**: 뷰포트의 화면의 높이를 100단위로 나눈 값입니다. 100vh는 전체 화면의 높이가 기준이 됩니다.

**vw**: 뷰포트의 화면의 너비를 100단위로 나눈 값입니다. 100vw는 전체 화면의 너비가 기준이 됩니다.

### PX, EM이란?

### 반응형 웹을 만들기 위해 사용하는 단위에 대해 설명해주세요.

CSS에서는 크기를 나타내는 다양한 단위를 사용합니다. 그 중에서도 **px**, **em**, **rem** 등이 자주 사용됩니다.

**px**: 절대적인 크기를 나타내는 단위입니다. 고정된 값이어서 사용하기 편하지만 반응형 웹에는 적절하지 않습니다.

**em**: 부모 요소에 비례하여 사이즈를 갖게 되는 상대적인 단위입니다. 부모 요소에 font-size가 16px로 되어 있다면 1em은 자동적으로 16px과 같아집니다.

**rem**: 최상위 요소인 <html> 요소에 비례하여 사이즈를 갖게 되는 상대적인 단위입니다. <html>에 font-size가 16px로 되어 있다면 1rem은 자동적으로 16px과 같아집니다.

따라서, px는 고정된 크기를 가지고 있어 반응형 웹에서 적절하지 않습니다. em과 rem은 상대적인 크기를 가지고 있어 반응형 웹에서 유용하게 사용됩니다.

---

출처: 

[1. bing.com](https://bing.com/search?q=%eb%b0%98%ec%9d%91%ed%98%95+%ec%9b%b9+3%ec%9a%94%ec%86%8c)

[2. velog.io](https://velog.io/@jmlee9707/CS-CSS-%EB%B0%98%EC%9D%91%ED%98%95-%EC%9B%B9%EC%9D%98-3%EC%9A%94%EC%86%8C-%EB%B0%98%EC%9D%91%ED%98%95-%EC%9B%B9%EA%B3%BC-%EC%A0%81%EC%9D%91%ED%98%95-%EC%9B%B9)

[3. kimdirector.co.kr](https://www.kimdirector.co.kr/691)

[4. knulab.com](https://knulab.com/archives/1153)

[1. bing.com](https://bing.com/search?q=%eb%b0%98%ec%9d%91%ed%98%95+%ec%9b%b9+%eb%8b%a8%ec%9c%84)

[2. blog.naver.com](https://m.blog.naver.com/zzaoday/221908180058)

[3. yeoninim.tistory.com](https://yeoninim.tistory.com/38)

[4. gnews365.tistory.com](https://gnews365.tistory.com/entry/css-%EB%8B%A8%EC%9C%84-media-query-%EB%B0%98%EC%9D%91%ED%98%95-%EC%9B%B9)

[5. designbase.co.kr](https://designbase.co.kr/webcoding-15/)

[1. bing.com](https://bing.com/search?q=)

[2. bing.com](https://bing.com/search?q=PX%2c+EM%ec%97%90+%eb%8c%80%ed%95%b4+%ec%84%a4%eb%aa%85%ed%95%b4%ec%a3%bc%ec%84%b8%ec%9a%94.)

[3. webprogrammingstory.tistory.com](https://webprogrammingstory.tistory.com/entry/css-%ED%81%AC%EA%B8%B0-%EB%8B%A8%EC%9C%84-px-em-rem-%EC%9D%98-%EC%B0%A8%EC%9D%B4%EC%A0%90)

[4. blog.naver.com](https://blog.naver.com/PostView.nhn?blogId=idsobol&logNo=221188713482)

[5. studyingazae.tistory.com](https://studyingazae.tistory.com/194)