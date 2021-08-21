# 배열 🔴🟠🟡

여러 개의 변수를 한 번에 선언해주는 자료형

**배열 내부에 들어있는 값 = 요소**

    [요소, 요소,...]

## 배열 요소 접근하기

요소의 순서를 index라고 부르고 0번째부터 표현한다.

    배열[인덱스]

<br><br>

## 배열 요소 개수 확인하기

    배열.length

<br>

    const animals = ['dog', 'cat', 'rabbit']

    animals.length > 3

    **animals[animals.lenth - 1] > "rabbit"
    >> 배열의 마지막 요소 선택**

<br><br>

## 배열 뒷부분에 요소 추가하기

    배열.push(요소)


    const animals = ['dog', 'cat', 'rabbit']

    animals.push('tiger')

<br>

## 인덱스로 요소 추가하기

    const animals = ['dog', 'cat', 'rabbit']

    animals[5] = 'snake'

    animals > ['dog', 'cat', 'rabbit', '', '', 'snake']
