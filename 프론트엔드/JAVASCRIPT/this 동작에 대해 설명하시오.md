---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# this 동작에 대해 설명하시오.

이지은(AI)

💡 #this #전역스코프 #메서드 #화살표함수 #생성자 #이벤트리스너

## **답변 드리겠습니다!**

<aside>
📌 this는 함수가 호출되는 위치에 따라 값이 다르게 출력됩니다. 예를들어 전역 스코프에서 호출되는 함수의 this는 전역 객체인 window를 가르킵니다. 객체 안에 메서드로 정의되어있는 함수를 호출한 경우에는 멤버 접근 연산자 앞의 객체를 가르킵니다. 화살표 함수의 경우는 상위 스코프를 가르킵니다. new 연산자를 사용해서 생성자 함수를 호출할 경우에는 인스턴스를 가르킵니다. 이벤트 리스너에서의 this는 이벤트가 발생한 target을 가르킵니다.

</aside>

수정할것

this에 관한 정의 : **자신이 속한 객체 또는 자신이 생성할 인스턴스를 가리키는 자기 참조 변수**(self-reference variable)

핵심1. this는 '자신이 속한 객체를 가리키는 변수' 이다. 핵심2. this는 자신을 '호출'하는 방법에 따라 다른 값을 가리킨다.

전역(선언적)함수, **내부함수**, 화살표함수, 생성자 함수가 있다고 명시적으로 말해주고 내부함수에 대한 내용도 추가할것

클래스에서의 this

상세 추가

call apply bind 메서드