# 함수

## 함수의 기본 형태

### 익명 함수

함수는 코드의 집합을 나타내는 자료형

    function () { }

<br>

    //  변수 생성

    const 함수 = functon () {
        console.log('함수 내부의 코드 ...1')
        console.log('함수 내부의 코드 ...2')
        console.log('함수 내부의 코드 ...3')
        console.log('') }

    // 함수 호출
    함수 ()
    함수 ()

    // 출력
    console.log(typeof 함수)
    console.log(함수)

<br> <br>

## 선언적 함수

    function 함수() {
    }

<br>

    // 함수 생성

    function 함수 () {
        console.log('함수 내부의 코드 1')
        console.log('함수 내부의 코드 2')
        console.log('')
        }

    // 함수 호출

    함수()
    함수()

    // 출력

    console.log(typeof 함수)
    console.log(함수)

<br>

## 매개변수와 리턴값

매개변수 : 함수를 호출할 때 괄호 안에 적는 것
prompt( ) 함수를 사용해 매개변수로 메세지를 넣음

    function 함수(매개변수, "","") {
    	문장
    	문장
    	return 리턴값
    	}

<br>

    // 함수 선언
    function f(x) {
        return x * x
        }

    // 함수 호출
    console.log(f(3))

    >> 9

<br>
## 나머지 매개변수

    function 함수 이름(...나머지 매개변수) { }

<br>

    function sample(...items) {
        console.log(items)
        }

    sample(1,2)
    sample(1,2,3)
    sample(1,2,3,4)

    >> [1,2] [1,2,3] [1,2,3,4]

<br>

## 콜백 함수

매개변수로 전달하는 함수

    // 함수 선언
    function callThreeTimes (callback) {
     for (let i = 0; i < 3; i++) {
    	 callback(i)
    	 }
    	 }


    function print (i) {
    console.log($`${i}번째 함수 호출`)
    }


    // 함수 호출
    callThreeTimes(print)

    > 0번째 함수 호출
      1번째 함수 호출
      2번째 함수 호출

<br>

    function callThreeTimes(callback) {
    for (let i = 0; i < 3; i++) {
        callback(i)
        }
        }

    // 함수 호출
    callThreeTimes(function (i) {
    	console.log(`${i}번째 함수 호출`)
    	})

    > 0번째 함수 호출
      1번째 함수 호출
      2번째 함수 호출

<br>

### 콜백 함수를 활용하는 함수: forEach()

    function (value, index, array) { }

<br>

### map( )

map( )메소드는 콜백함수에서 리턴한 값들을 기반으로 새로운 배열을 만드는 함수

    let numbers = [10,20,30,]

    numbers = numbers.map(function (value,
    index,array) {
    return value * value })

    // 출력
    numbers.forEach(console.log)

<br>

### filter( )

콜백 함수에서 리턴하는 값이 true인 것들만 모아서 새로운 배열을 만드는 함수

    const numbers = [0,1,2,3,4]
    const evenNumbers = number.filter(function (value) { return value % 2 === 0 })

    console.log(`원래 배열: ${numbers}`)
    console..log
