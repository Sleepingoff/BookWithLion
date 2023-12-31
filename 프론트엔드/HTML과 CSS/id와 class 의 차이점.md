---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# id와 class 의 차이점을 설명하시오.

임연정

💡 #유일한 요소 #복수 요소 #선택자 우선 순위

## **답변 드리겠습니다!**

<aside>
📌 id는 전체 페이지에서 하나의 유일한 요소에 적용하고 class는 복수의 요소에 적용할 때 사용됩니다. 따라서 id는 한 문서에서 한 번만 사용할 수 있지만, class는 여러 번 반복해서 사용이 가능합니다. id는 유일하게 사용되기 때문에 우선적으로 적용되어 class보다 우선순위가 높습니다.

</aside>

  id 속성과 class 속성의 차이는 고유성에 있습니다. id는 전체 페이지에서 유일한 요소에 적용할 때, 그리고 class는 복수의 요소에 적용할 때 사용한다는 점입니다. 다시 말해, id 속성은 태그에 유일한 이름을 붙이고 싶을 때 사용하고 class 속성은 같은 유형으로 반복되는 태그들을 유형별로 분류하고 싶을 때 사용합니다. CSS에서 id 속성을 사용할 때는 id 이름 앞에 # 기호를 붙여서 사용하며 class 속성을 사용할 때는 class 이름 앞에 . 기호를 붙여 사용합니다. 하나의 id는 한 문서에서 한 번만 사용이 가능하지만, 하나의 class는 중복 사용이 가능합니다. id는 유일하게 쓰이기 때문에 우선적으로 적용되어 class보다 우선순위가 높습니다.

## **이런 질문도 나올 수 있어요!**

### **그렇다면 선택자 우선 순위가 어떻게 되는지?**

  첫 번째로 `**!important**` 키워드가 적용된 스타일을 최우선하고, 두 번째로 inline 스타일을 우선합니다. 세 번째로 ID 선택자, 네 번째로 class 선택자를 우선하여 ID 선택자가 class 선택자보다 우선순위가 높습니다. 다섯 번째로 tag 선택자, 마지막으로 전체 선택자를 우선합니다.

---

출처: 

[클래스(class)와 아이디(id)의 차이점](https://heinafantasy.com/155)

[[HTML] id속성과 class속성의 차이](https://velog.io/@jeju_daun/%EA%B8%B0%EC%88%A0%EB%A9%B4%EC%A0%91%EC%A4%80%EB%B9%84-id%EC%86%8D%EC%84%B1%EA%B3%BC-class%EC%86%8D%EC%84%B1%EC%9D%98-%EC%B0%A8%EC%9D%B4)