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
