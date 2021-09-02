# 반복문

## for in 반복문

배열과 함께 사용할 수 있는 반복문으로
**배열 요소를 하나하나 꺼내서 특정 문장**을 실행할 때 사용

        for (const 반복 변수 in 배열 또는 객체) {
    	    문장	}

<br>

    const todos = ['기상','식사',취침']

    for (const i in todos) {
    	console.log(`${i}번째 할 일: ${todos[i]}')
    	}

> 0번째 할 일: 기상
> 1번째 할 일: 식사
> 2번째 할 일: 취침

<br><br>

## for of 반복문

**요소의 값을 반복**할 때 사용

        for (const 반복 변수 of 배열 또는 객체) {
        문장 }

<br>

     const todos = ['기상','식사',취침']
     for (const todo of todos) {
         console.log(`오늘의 할 일:${todo}`)
         }

<br><br>

for (let i = 0; i < 반복 횟수; i++) {
문장 }

<br>

     const todos = ['기상','식사',취침']
     for (const todo of todos) {
         console.log(`오늘의 할 일:${todo}`)
         }

<br><br>

## for 반복문

특정 횟수만큼 반복하고 싶을 때 사용하는 반복문

    for (let i = 0; i < 반복 횟수; i++) {
        문장 }

<br>

    for (let i = 0; i < 5; i++) {
        console.log(``${i}번째 반복입니다.`) }

<br><br>

## while 반복문

문장을 한 번만 실행하고 끝나는 것이 아니라 불 표현식 true면 계속해서 문장을 실행한다는 것입니다.

        while (불 표현식) {
    	    문장 }

반복문이 무한 반복되는 것 => infinite loop

let i - 0
while (ture) {
alert(`${i}번째 반복입니다.`)
i = i + i }

<br>

    let i = 0
    while (confirm('계속 진행하시겠습니까?')) {
        alert(`${i}번째 반복입니다.`)
        i = i + i }

<br>

confirm( ) 함수를 입력하면 사용자에게 확인을 받는 대화상자가 실행된다.

<br>

### while 반복문과 함께 배열 사용하기

while 반복문과 for 반복문은 서로 대체해서 사용가능

    let i = 0
    const array = [1,2,3,4,5]

    while (i < array.length) {
    	console.log(`${i} : ${array[i]}`)
    	i++ }

<br><br>

## break 키워드

break 키워드는 switch 조건문이나 반복문을 벗어날 때 사용하는 키워드

    while (true) {
       } 	break

<br><br>

    for (let i = 0; true; i++) {
        alert(i + '번째 반복문입니다.')

    const isContinue = confirm('계속 하시겠습니까?')
    if (!isContinue) {
    	break
    	}
    }

    alert('프로그램 종료')

<br><br>

## continue 키워드

continue 키워드는 반복문 안의 반복 작업을 멈추고 반복문의 처음으로 돌아가 다음 반복 작업을 진행

for (let i = 0; i < 5l i++) {
// 현재 반복 작업 중지 >> 다음 반복 작업 수행.
continue
alert(i)
}

<br>

    let output = 0

        // 반복문
    for (let i = i; i <= 10; i++) {
    	// 조건문
    	if (i % 2 === 1) {
    		// 홀수면 현재 반복 중지하고 다음 반복 수행
    	continue }
    	output += i }

    	//출력
    	alert(output)

<br> <br>

## 중첩 반복문을 사용하는 피라미드

중첩 조건문과 마찬가지로 반복문을 여러 겹 중첩해 사용

[1,2,3]처럼 배열이 한 겹으로 감싸진 배열 > 1차원 배열,
[[1,2,3,], [4,5,6] 처럼 두 겹으로 감싸진 배열 > 2차원 배열
