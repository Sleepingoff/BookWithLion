---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# 답변) Virtual DOM이란 무엇인지 설명하시오.  (🔨수정중..)

<aside>
🔥 오태권

</aside>

## 답변드리겠습니다.

<aside>
📌 Virtual DOM은 실제가 아닌, 가상의 DOM으로서, 웹 애플리케이션의 효율적인 업데이트와 랜더링을 위해 도입된 개념입니다. 브라우저는 코드 실행평가 과정이 끝난 후, 실제 DOM이 아닌, 가상의 DOM을 만들어서 DOM조작을 가상적으로 랜더링해본 뒤, 실제 DOM과 차이가 나는 부분에 대해서만 리랜더링을 하게 하도록 합니다. 즉, 하나의 변경이 있을 때, 전체의 DOM이 재랜더링이 아닌, 차이가 나는 부분만 재랜더링함으로써, 보다 동적이고 빠른 UI를 제공할 수 있도록 합니다.

</aside>

## 1. **상세**

**가상 DOM의 작동 방식은 다음과 같습니다.**

- **초기 랜더링 → 상태 변화 감지 → 가상 DOM 업데이트 → 실제 DOM 업데이트**

1. **초기 렌더링:** 웹 애플리케이션이 처음으로 실행될 때, **가상 DOM 트리**가 생성됩니다. 이 트리는 실제 DOM과 동일한 구조를 가지지만, **초기 상태**를 반영합니다.
2. **상태 변화 감지:** 웹 애플리케이션의 상태가 변경될 때, **가상 DOM 트리가 다시 생성됩니다**. 이전 **가상 DOM 트리와 비교하여 변경된 부분**을 감지합니다.
3. **가상 DOM 업데이트:** 변경된 부분만 가상 DOM에서 업데이트합니다. 이 단계에서는 실제 DOM을 직접 조작하지 않으며, **가상 DOM의 업데이트는 메모리 상**에서 처리됩니다.
4. **실제 DOM 업데이트:** 가상 DOM의 변경 내용을 실제 DOM에 적용합니다. 이 단계에서는 최소한의 DOM 조작만 수행하여 성능을 향상시킵니다.

# 의견 : 팀 회의

상대적인 비교군이 있었으면 좋겠다.

ex) 리액트를 사용했을때 어떤것 (자바스크립트) 보다 가상 돔 활용으로 랜더링이 빠르다.

컨벤션은 번호 없이 글머리 기호 사용을 하지 않습니다. (수정 요망 숫자는 가능)