# Chap1 - 리팩토링이란?

## 코드 동작이 변하지 않는다는 것을 어떻게 보장할 수 있을까?

- 코드 변경과 안전성을 보장하는 자동화 도구를 사용
- 롤백을 위한 버전 관리 툴 사용
- 절차
  - 테스트 실패
  - 테스트 성공
  - 리팩토링 주기
  - 롤백

## 구현 세부 사항에 관심을 두면 어떨까?

- 함수 구현 보다 입력 값과 결과 값을 중요하게 여긴다

## 블특정하고 검증되지 않은 동작에 관심을 두면 어떨까?

- 어떻게 동작하는지 최소한의 설명이 필요. 그렇지 않으면 검증할 수 없다

## 성능에 관심을 두면 어떨까?

- 구현에서 결과가 충분히 좋다는 것은 적절한 시간 안에 입력으로 기댓값을 산출할 수 있다는 의미이다
- 성능을 고려하는 것은 우리가 기대하는 기대치와 테스트를 결정하기 전까지는 부차적인 문제이다

## 동작이 변하지 않는다면 리팩토링의 요점은?

- 행동을 유지하면서 품질을 향상 시키는 것

## 품질이란 무엇이며 리팩토링과 어떤 관련이 있을까

- SOLID
  - Single responsibility
  - Open closed
  - Liskov substitution
  - Interface segregation
  - Dependency inversion
- DRY : Don't Repeat Yourself
- KISS : Keep It Simple, Stupid
- GRASP : General Responsibility Assignment Software Patterns
- YAGNI : Ya Ain't Gonna Need It
