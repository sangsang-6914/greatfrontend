# Debounce (GreatFrontEnd)

- 링크: https://www.greatfrontend.com/interviews/study/gfe75/questions/javascript/debounce
- 난이도: Medium
- 풀이 날짜: 2025-11-23

## 접근 방법

1. 클로저 함수를 사용해서 디바운스 함수 호출 시점의 타이머 기억
2. 이전 타이머가 존재하면 타이머 제거
3. setTimeout을 사용하여 인자로 받은 wait ms만큼 대기
4. context에 this를 저장하여 호출시점의 this를 사용
5. ...args를 이용하여 호출시점의 인자를 사용
6. func.apply(this, args)를 사용하여 this, args 소실 방지

## 배운 점 / 리팩터링 아이디어

- 클로저함수에 대한 이해
- func.apply(this, args)를 활용한 함수실행 이유 확인
