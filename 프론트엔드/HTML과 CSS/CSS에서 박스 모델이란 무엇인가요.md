---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# CSS에서 박스 모델이란 무엇인가요?

임연정

💡 #사각형 박스 #레이아웃

## **답변 드리겠습니다!**

<aside>
📌 CSS에서 박스 모델이란 웹 페이지의 요소들을 사각형 박스로 표현하는 방식입니다. HTML의 요소들은 박스로 이루어져 있으며 이 박스는 네 개의 영역으로 이루어져 있습니다. 각 부분은 콘텐츠 영역과 테두리 영역, 그리고 안쪽 여백(padding) 영역, 바깥 여백(margin)으로 구성됩니다.

</aside>

  박스 모델은 웹 페이지의 레이아웃을 유연하게 구성하기 위한 중요한 역할을 합니다. 각 요소의 위치와 크기를 조절하기 위해 박스 모델의 속성들을 사용합니다. 예를 들어, padding을 설정하여 요소의 내용과 테두리 사이에 여백을 만들 수 있고, 테두리를 설정하여 요소 주위에 테두리를 만들 수 있습니다. 요소의 크기를 조절하기 위해 너비 및 높이의 설정과 여백과 테두리의 크기를 조절하여 요소의 전체 크기를 변경할 수도 있습니다.

## **이런 질문도 나올 수 있어요!**

### 마진 병합 현상이란?

  CSS에서, 인접한 블록 요소의 상하단 마진이 서로 겹치어 병합되는 것을 마진 병합 현상이라고 하며, 마진 중에서 큰 값을 가진 마진으로 병합됩니다. 이는 여백을 늘려도 늘어나지 않거나 의도치 않게 요소의 여백이 줄어들게 할 수 있습니다.

  이를 해결하기 위해서는 부모 요소에 `**border**` 속성, 혹은 `**padding**` 속성을 추가하거나 `**overflow: hidden**` 속성을 적용할 수 있습니다. 또한, 자식 요소에 `**display: inline-block**` 속성을 추가할 수도 있습니다.

---

출처: 

[developer.mozilla.org](https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model)

[w3schools.com](https://www.w3schools.com/Css/css_boxmodel.asp)

[codingfactory.net](https://www.codingfactory.net/10556)

[songsong.dev](https://songsong.dev/entry/css-%EC%95%A0%EB%8B%88%EB%A9%94%EC%9D%B4%EC%85%98-jank-%ED%95%B4%EA%B2%B0%ED%95%98%EA%B8%B0-2%ED%8E%B8-%EC%97%AC%EB%B0%B1-%EC%83%81%EC%87%84)

[developer.mozilla.org](https://developer.mozilla.org/ko/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing)

[velog.io](https://velog.io/@ursr0706/%EB%A7%88%EC%A7%84margin)

[velog.io](https://velog.io/@ewaterbin/CSS.-%EB%A7%88%EC%A7%84-%EB%B3%91%ED%95%A9-%ED%98%84%EC%83%81%EA%B3%BC-%ED%95%B4%EA%B2%B0%EB%B0%A9%EB%B2%95-Box-sizing)