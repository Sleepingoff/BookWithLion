---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# css에서 c는 cascading을 의미하는데 이에 대한 설명과 캐스캐이딩 시스템의 장점은?

<aside>
💡

</aside>

- **요약**

CSS에서 C는 Cascading을 의미합니다. Cascading은 CSS에서 스타일 규칙들이 어떻게 적용할지를 결정하는 방법입니다. 이 방법의 장점은 스타일 규칙들이 우선순위에 따라 상속되며, 이를 통해 코드의 재사용성과 유지보수성이 향상된다는 점입니다.

- **상세**

Cascading 시스템은 CSS에서 스타일 규칙들이 어떻게 적용할지를 결정하는 방법입니다. Cascading은 우선순위, 상속, 그리고 스타일 우선순위로 총 3가지 방식으로 이루어집니다: 

우선순위는 CSS 규칙 중 어떤 규칙을 우선하는지를 결정합니다. 이는 다양한 방법으로 이루어집니다: 중요도, 우선순위, 소스 순서 등이 그 예입니다.

상속은 부모 요소에 있는 스타일 규칙이 자식 요소로 상속되는 방법입니다. 예를 들어, `font-family`를 설정한 경우, 자식 요소에서 별도로 `font-family`를 설정하지 않아도 부모 요소의 값이 상속됩니다.

스타일 우선순위는 요소의 스타일 규칙이 적용되는 방식을 결정합니다. 이는 브라우저에 의해 미리 정해진 우선순위에 따라 이루어집니다.

Cascading 시스템의 장점은 코드의 재사용성과 유지보수성이 향상된다는 점입니다. 스타일 규칙들이 우선순위에 따라 상속되기 때문에, 같은 스타일 규칙을 반복해서 작성하지 않아도 되며, 코드를 수정할 때도 한 곳에서만 수정하면 되므로 유지보수성이 향상됩니다.

### 꼬리 질문

**Cascading 시스템에서 중요도는 어떻게 결정될까요?**

Cascading 시스템에서 중요도는 `!important` 키워드를 사용하여 결정됩니다. 이 키워드는 특정 스타일 규칙이 다른 규칙보다 높은 우선순위를 가지도록 만듭니다. 이는 특정 요소에 적용되는 스타일 규칙이 동일한 우선순위를 가지는 다른 규칙들보다 더 높은 우선순위를 가지도록 하기 위해 사용됩니다. 이를 통해, 해당 스타일 규칙이 더 높은 우선순위를 가지므로 다른 규칙들보다 우선하여 적용됩니다.

### 추가 개념

CSS에서는 선택자가 우선순위에 영향을 미칩니다. 예를 들어, `#id` 선택자가 `.class` 선택자보다 우선순위가 높습니다. 또한, `!important` 키워드를 사용하면 중요도를 높일 수 있습니다.