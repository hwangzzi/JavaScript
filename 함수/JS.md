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
