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

<br><br>

## 배열 요소 제거하기

### 1. 인덱스로 제거

    배열.splice(인덱스, 제거할 요소의 개수)

<br>

    const animals = ['dog', 'cat', 'rabbit']

    animals.splice(2, 1)
    ["rabbit"}

    animals > ["dog", "cat"}

<br>

### 2. 값으로 제거하기

    const 인덱스 = 배열.indexOf(요소)
    배열.splice(인덱스, 1)

<br>

    const animals = ['dog', 'cat', 'rabbit']

    const index = animals.indexOf('cat')

    index > 2
    <br><br>

## 자료의 비파괴 & 파괴

### 비파괴적 처리

> > **처리 후에 원본 애용이 변경되지 않음**

<br>

    const a = '안녕'
    const b = '하세요'

    const c = a + b

    c > "안녕하세요"

    a > "안녕"
    b > "하세요   // 원본 내용 변경 X

<br><br>

### 파괴적 처리

> > **처리후에 원본 내용이 변경**

    const animals = [ "dog" , "cat" , "pig"]

    array.push("rabbit")  > 4

    array >  [ "dog" , "cat" , "pig" , "rabbit"]

<br>

**자료 보호를 위해서 비파괴적 처리를 하는 것이 좋음**
