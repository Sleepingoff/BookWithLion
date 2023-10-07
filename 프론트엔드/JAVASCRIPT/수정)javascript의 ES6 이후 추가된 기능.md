---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# javascript의 ES6 이후 추가된 기능은 무엇이 있습니까?

<aside>
💡 **최신 JavaScript 트렌드에 맞는 프로그래밍을 하고 있는지 알아 보는 있는 질문입니다.**

</aside>

- **요약 (316자)**

 2015년 승인된 ECMAScript 제 6판을 기준으로 매년 새로운 판이 출판되고 있습니다. 자바스크립트에 ES6 이전과 뚜렷하게 다른 추가기능으로는 let, const, arrow func, classes, module, destructuring, map/set, promise, await/async,rest/spread properties, class fileds 등이 있습니다. 말씀드린 추가 기능을 통해서 자바스크립트는 좀 더 객체 지향 프로그래밍 언어가 되었으며, 의도치 않은 오류가 줄어들고, 데이터를 가공 및 접근이 보다 용이해질 수 있게 됬습니다.

- **상세**

### 꼬리 질문

1. 꼬리 질문

### 추가 개념

- 부록으로 아래 내용 추가

2023년 06월 27일 [ECMASCript 제 14판을 최종 승인](https://www.ecma-international.org/news/ecma-international-approves-new-standards-at-the-125th-general-assembly-27-june-2023/) 했다.

ECMAScript 의 변경 기록 및 앞으로 추가될 내용은 [ECMA-262 GitHub 저장소](https://github.com/tc39/proposals/blob/HEAD/finished-proposals.md)에서 확인할 수 있다.

ES (ECMAScript): ECMA 스크립트란, Ecma International 이 ECMA-262 기술 규격에 따라 정의하고 있는 표준화된 스크립트 프로그래밍 언어를 말한다. 자바스크립트를 표준화하기 위해 만들어졌다. ECMA-262 는 매년 새로운 판이 출판되며 꾸준히 업데이트가 되고 있다.

ES6 => ES2015 (ECMAScript 2015)

ES7 => ES2015 (ECMAScript 2015)

ES8 => ES2015 (ECMAScript 2015)

...

ES13 => ES2022 (ECMAScript 2022)

ES14 => ES2023 (ECMAScript 2023)

ES15 => [ES2024](https://tc39.es/ecma262/#sec-intro) (ECMAScript 2024) // ES문서와 해당 연도는 9 차이가 난다.

**ES6 (ECMAScript 2015) 추가 기능**

- [ ]  **arrow**
- [ ]  enhanced object literals
- [ ]  **template strings**
- [ ]  **destructuring**
- [ ]  default, rest, spread
- [ ]  **let, const**
- [ ]  **Iterators, for...of**
- [ ]  generators
- [ ]  unicode
- [ ]  **classes (클래스)**

- [ ]  **modules**
- [ ]  module loaders
- [ ]  **map, set, weakmap, weakset**
- [ ]  proxies
- [ ]  symbols
- [ ]  subclassable build-ins
- [ ]  **promises (비동기 프로그래밍)**
- [ ]  math, number, string, array, object APIs
- [ ]  binary and octal literals
- [ ]  reflect api
- [ ]  tail calls (꼬리 물기 최적화)

**ES7 (ECMAScript 2016) 추가 기능**

- [ ]  Array.prototype.includes()
- [ ]  지수 연산자(**)

**ES8 (ECMAScript 2017) 추가 기능**

- [ ]  문자열 패딩
- [ ]  Object.entries(), Object.values()
- [ ]  Object.getOwnPropertyDescriptors()
- [ ]  후행 쉼표
- [ ]  Shared memory and atomics (공유된 메모리와 원자 / SharedArrayBuffer 객체와 Atomics 객체를 사용한 메모리 공유)
- [ ]  **Async Functions (async, await)**
- [ ]  오류 처리

**ES9 (ECMAScript 2018) 추가 기능**

- [ ]  Asynchronous Iteration (비동기 반복 / for-await-of)
- [ ]  **Rest/Spread Properties** (전개연산자 및 rest 파라미터 => 배열로 변경)
- [ ]  Promise.prototype.finally()
- [ ]  정규식 기능 추가 (s(dotAll) 플래그, 명명된 캡처 그룹, 룩비하인드 어서션, 유니코드 속성 이스케이프)
- [ ]  템플릿 리터럴 제한 해제

**ES10 (ECMAScript 2019) 추가 기능**

- [ ]  Array.prototype.flat(), Array.prototype.flatMap()
- [ ]  Object.fromEnties()
- [ ]  String.prototype.trimStart(), String.prototype.trimEnd()
- [ ]  선택적 catch 할당
- [ ]  Function.prototype.toString()
- [ ]  Symbol.prototype.description

**ES11 (ECMAScript 2020) 추가 기능**

- [ ]  Bigint
- [ ]  동적으로 가져오기
- [ ]  옵셔널 체이닝
- [ ]  Promise.allSettled()
- [ ]  null 계열의 값을 병합하기
- [ ]  String.prototype.matchAll()
- [ ]  모듈 네임스페이스 export 문법
- [ ]  import.meta
- [ ]  globalThis

**ES12 (ECMAScript 2021) 추가 기능**

- [ ]  String.prototype.replaceAll()
- [ ]  Promise.any()
- [ ]  논리 연산자와 할당 표현식
- [ ]  숫자 구분 기호
- [ ]  약한 참조
- [ ]  Intl.ListFormat
- [ ]  Intl,DataTimeFormat 의 dataStyle 및 timeStyle 옵션

**ES13 (ECMASCript 2022) 추가 기능**

- [ ]  Top-level await (모듈 최상단에서 await 사용 가능)
- [ ]  **Class fields (접근 제어자 속성 #)**
- [ ]  클래스 내 정적 블록 (static 초기화 블록)
- [ ]  in 키워드의 기능 확장 (객체에 private 인스턴스 존재 확인)
- [ ]  정규식 표현식 플래그 d를 통한 일치 인덱스 (일치하는 하위 문자열에 시작 또는 종료 인덱스를 제공)
- [ ]  Error.prototype.cause 속성 (추가적인 Context Message)
- [ ]  .at() 키워드 추가 (배열의 음수 인덱싱 가능)
- [ ]  Object.hasOwn 키워드 추가 (Object.prototype.hasOwnProperty 의 대안으로 추가)

**ES14 (ECMAScript 2023) 추가 기능**

- [ ]  Array.prototype.findLast(), Array.prototype.findLastIndex() 메소드 (역방향으로 요소를 탐색)
- [ ]  Array.prototype.toReversed() / .toSroted() / .toSliced(index,count) / .with(index, value) 메소드
- [ ]  (원본 배열을 변경하지 않고 새로운 배열을 반환)
- [ ]  WeakMap 의 키로 Symbol 사용
- [ ]  HashBang(Shebang) 문법 (실행할 프로그램의 인터프리터 정의. 스크립트 첫 라인에 #! 시작)

참고자료 1. [위키백과](https://ko.wikipedia.org/wiki/ECMA%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8) - ECMA스크립트

참고자료 2. [ES6 - ES9](https://velog.io/@katanazero86/ES6-ES9-%EA%B0%84%EB%9E%B5-%EC%A0%95%EB%A6%AC) 간략 정리

참고자료 3. 모던 자바스크립트 핵심 가이드 : ES7 - ES12 추가 기능

참고자료 4. [ES13 추가된 기능](https://dev-juwon.netlify.app/blog/js_03_ecma2022/)들

참고자료 5. [ES14 추가된 기능](https://guiyomi.tistory.com/146)들