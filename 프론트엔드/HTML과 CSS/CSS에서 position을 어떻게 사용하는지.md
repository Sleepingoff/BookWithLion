# CSS에서 position을 어떻게 사용하는지 설명해주세요.

임연정

💡 #HTML 요소 배치 #static #relative #absolute #fixed #sticky

## **답변 드리겠습니다!**

<aside>
📌 CSS에서 HTML 문서 상에 요소가 배치되는 방식을 결정하기 위해 position 속성을 사용합니다. 요소의 정확한 위치 지정을 위해서 top, left, bottom, right 속성과 함께 사용되며 **`static`**, **`relative`**, **`absolute`**, **`fixed`**, **`sticky`**, 총 5가지의 값이 쓰입니다.

</aside>

  **`static`**은 position 속성의 default 값이며 기본적인 문서의 흐름에 따라 요소의 위치를 배치합니다. **`relative`**는 요소를 자신의 원래 위치를 기준으로 잡아 상대적으로 배치합니다. 다만, 다른 요소들에게 영향을 주지 않습니다.

  **`absolute`**는 요소를 문서의 가장 가까운 조상 요소에 상대적으로 배치합니다. 만약 조상 요소가 없다면 문서 본문(body)을 기준으로 배치하며 마찬가지로 다른 요소들의 배치에 영향을 주지 않습니다.

  **`fixed`**는 요소를 뷰포트 기준으로 상대적으로 배치하며 스크롤이 되어도 요소가 고정됩니다.

  **`sticky`**는 요소를 문서의 흐름에 따라 배치하다가 스크롤링 할 때 상대적으로 이동시키며 지정된 오프셋을 기준으로 동작합니다.

## **이런 질문도 나올 수 있어요!**

### 언제 absolute positioning 대신에 translate ()를 쓰는게 좋나요?

  CSS에서 **`absolute positioning`**과 **`translate()`**는 서로 다른 목적을 가지고 있습니다.

  **`absolute positioning`**은 엘리먼트를 특정 위치에 위치시키기 위해 사용되며, **`translate()`**는 디자인 애니메이션 혹은 모션에 목적을 두고 있습니다. `**translate()**`같은 CSS3 애니메이션 함수는 GPU로 처리하기 때문에 속도가 빠릅니다.

  반면 `**absolute**`를 사용하면 레이아웃을 계산하기 위해 CPU의 연산처리가 동반됩니다. 그 후 reflow와 repaint가 발생하여 속도가 느려질 수 있습니다. 또한 **`absolute`** 사용 시엔 주변 요소에 영향을 미치지만 **`translate()`**은 좌표 공간을 변형시키기 때문에 다른 요소에 영향을 미치지 않습니다.

  따라서 사용하는 상황에 따라 선택하시면 됩니다.

---

출처: 

[(CSS) CSS Position 설명. CSS를 사용하다보면 position 속성을 사용할 때가 많이… | by Su Bak | Medium](https://medium.com/@su_bak/css-css-position-%EC%84%A4%EB%AA%85-f2c0a0b26556)

[electronic-moongchi.tistory.com](https://electronic-moongchi.tistory.com/26)

[developer.mozilla.org](https://developer.mozilla.org/ko/docs/Web/CSS/position)

[-TIL/CSS/absolute대신 translate() 사용하는 이유.md at master · FE-Lex-Kim/-TIL (github.com)](https://github.com/FE-Lex-Kim/-TIL/blob/master/CSS/absolute%EB%8C%80%EC%8B%A0%C2%A0translate()%20%EC%82%AC%EC%9A%A9%ED%95%98%EB%8A%94%20%EC%9D%B4%EC%9C%A0.md)

[프론트엔드 면접 문제 2탄 ⭐️ (velog.io)](https://velog.io/@cjy0029/%ED%94%84%EB%A1%A0%ED%8A%B8%EC%97%94%EB%93%9C-%EB%A9%B4%EC%A0%91-%EB%AC%B8%EC%A0%9C-2%ED%83%84-giv1twbt)