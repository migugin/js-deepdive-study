## 목차

[📗배운 점](#📗배운-점)

[🤔궁금한 점](#🤔궁금한-점)

[📌중요한 점](#📌중요한-점)

## 📗배운 점

### strict mode (엄격 모드)

> **strict mode** : JavaScript 코드를 엄격하게 해석하고 실행하는 모드. 이 모드를 사용하면 일부 실수를 오류로 감지하고, 일부 안전하지 않은 작성 방식을 방지할 수 있다.

필자는 `ESLint` 를 선호한다.

---

적용방법 : 전역 또는 함수 몸체의 선두에 `'use strict'`를 추가한다.

> **전역에 사용하는것은 피하자.**
>
> - strict 는 script 단위로 적용되기 때문에 다른 스크립트에 영향을 주지 않고 해당 스크립트만 적용된다.
> - 여기서 strict mode 와 non-strict mode 를 혼용하는것은 오류를 발생시킬 수도 있다.

> **함수 단위로 적용하는것도 피하자.**
>
> - 어디는 적용하고 어디는 적용 안하는것도 바람직 하지 않고 모든 함수에 일일이 적용하는것도 번거롭다.

따라서 **_strict mode 는 즉시 실행 함수로 감싼 스크립트 단위로 적용_**하는것이 바람직 하다.

---

> **strict mode 가 발생 시키는 에러.**

1. 선언하지 않은 변수를 참조하면 ReferenceError 가 나옴.
2. delete 연산자로 변수, 함수, 매개변수를 삭제하면 SystaxError 가 뜸.
3. 중복된 매개변수 사용 또한 SystaxError.
4. whit 문도 SystaxError.

> **strict mode 적용에 의한 변화**

1. 일반 함수에서 this를 호출하면 undefined가 나온다. 생성자 함수가 아닌곳에선 this를 호출할 필요가 없기 때문이다.
2. 매개변수에 전달된 인수를 재할당 하여 변경하여도 argments 객체에 반영되지 않는다.

## 🤔궁금한 점

## 📌중요한 점