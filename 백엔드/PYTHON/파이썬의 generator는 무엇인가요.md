---
created: 2023-10-07T09:25
updated: 2023-10-07T18:27
---
# 파이썬의 generator는 무엇인가요?

고동우

#Python #제너레이터(generator)

## **답변 드리겠습니다!**

<aside>
📌 Iterator를 생성하는 함수입니다. yield 키워드를 사용하여 반환하며 yield는 return과 달리 반환 후 종료되지 않고 그 상태를 유지합니다. 한 번에 모든 값을 메모리에 담지 않아 용량이 작은 메모리로도 큰 데이터를 처리할 수 있으며 실행 시, 필요한 순간까지 계산을 미루어 처리하기 때문에 큰 데이터 셋을 처리할 때 메모리 점유율을 줄일 수 있습니다.

</aside>

파이썬의 generator는 iterator를 생성하는 함수로,

generator 함수는 `yield` 키워드를 사용하여 값을 반환하고 그다음 호출 시 이전 상태를 기억하여 계속 실행됩니다. generator는 큰 데이터를 한 번에 메모리에 처리하지 않고 필요할 때마다 요소를 꺼내서 사용하기에 유용합니다.

주요 특징
    - 모든 값을 한 번에 계산하지 않고 필요할 때마다 값을 생성합니다.
    - 큰 데이터를 처리할 때 메모리 사용량을 줄일 수 있습니다.
    - 이전 호출의 상태가 유지되어서, 반복 작업에서 유용합니다.

    - 일반적인 반복문 대신 generator를 사용하면 코드가 간결해지고 가독성이 향상됩니다. (368)

```python
def counter_n(n):
    i = 0
    while i <= n:
        yield i
        i += 1

# generator 객체 생성
counter = count_n(10)

# 값을 하나씩 반환
# 이전 호출의 상태가 유지됨
print(next(counter))  # 출력: 0
print(next(counter))  # 출력: 1
,
,
,
```

## **이런 질문도 나올 수 있어요!**

### generator는 어떤 상황에서 사용하면 좋을까요?

리스트의 경우에는 생성하는 것 만으로도 메모리에 요소를 할당하지만, generator는 필요한 순간까지 계산을 미루었다가 실행 시 값을 생성합니다. 그렇기 때문에 큰 데이터 셋을 처리 시, 메모리 점유율을 줄일 수 있고 한 번에 모든 값을 메모리에 저장하지 않아 큰 데이터도 보다 작은 메모리 용량으로도 처리할 수 있습니다. 따라서 메모리 효율성이 좋습니다.

그러므로 generator는 대규모 데이터 셋을 다루는데 사용합니다. 필요한 만큼의 데이터만 생성하여 메모리 사용량과 연산 비용을 모두 줄일 수 있으며 파생된 여러 클래스를 사용하여 효율적으로 코드를 작성할 수 있습니다.

### **두번째 질문**

질문에 대한 **요약** 답변

## **만반의 준비! 이것도 알아둘까요?**

### **제목 heading3**

내용

---

[카피킬러 기본 결과확인서 - 파이썬의 generator는 무엇인가요 - 239236478.pdf](%25EC%25B9%25B4%25ED%2594%25BC%25ED%2582%25AC%25EB%259F%25AC_%25EA%25B8%25B0%25EB%25B3%25B8_%25EA%25B2%25B0%25EA%25B3%25BC%25ED%2599%2595%25EC%259D%25B8%25EC%2584%259C_-_%25ED%258C%258C%25EC%259D%25B4%25EC%258D%25AC%25EC%259D%2598_generator%25EB%258A%2594_%25EB%25AC%25B4%25EC%2597%2587%25EC%259D%25B8%25EA%25B0%2580%25EC%259A%2594_-_239236478.pdf)

⚠️여기에 각주내용 및 출처, 그림 제목 등에 대해서 달아주세요!!!

표: 노션에서 제공해주는 기본 표 사용. 데이터베이스X

그림: 피그잼으로 도식화하여 사용 ~ 임시로 레퍼런스 사용 가능

코드: 노션에서 제공해주는 코드 블럭 사용 

단축키: ```(백틱 3개)

`백틱`: 메서드 및 코드 블럭에서 사용한 내용을 본문에서 언급할 때 

단축키: 해당 내용을 드래그하여 ctrl+E

인용: 노션에서 제공해주는 기본 스타일 사용

출처가 필요한 내용: *기울게* → 추후 일괄 수정 예정*

⚠️ 질문에 대한 답변 완료 및 저작권, 맞춤법 등의 추가 검사까지 완료

→페이지 아이콘 바꾸기 ✅ 해당 아이콘으로 페이지 아이콘을 바꿔주세요!