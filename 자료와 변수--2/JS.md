## 숫자 자료형 📒

    273 > 273
    3.14 > 3.14

자바스크립트는 소수점이 있는 숫자도 숫자 자료형으로 인식한다.

 <br>

> \+ 더하기 연산자
> \- 빼기 연산자 \* 곱하기 연산자
> / 나누기 연산자
> % 나머지 연산자

 <br>
  <br>
 <br>

## 불 자료형 📗

참과 거짓을 표현할 때 , 조건물을 사용할 때 사용 > true / false
<br> <br>

### 🟢 비교 연산자

> === 양쪽이 같음
> !== 양쪽이 다름

비교 연산자는 숫자, 문자열 자료형에도 사용 가능하다.
문자열 자료형은 **사전의 앞쪽에 있을수록 값이 작다**

 <br>
    
    10 === 10  
     true
    
    '가방' > '하마' 
     false

 <br>


    if (273 < 52) {
        alert('273은 52보다 작아')
     }
     if (273 > 52) {
    	 alert('273은 52보다 커')
    }

<br><br>

### 🟢 논리 부정 연산자

    !ture
     > false

    !false
    > true

<br> <br>

### 🟢 단항 / 이항 / 삼항 연산자

    !true    // 피연산자가 true > 1개   >>  단항 연산자
     > false

    10 + 20   // 피연산자가 10, 20 > 2개  >> 이항 연산자
    > 30

    true ? 10 : 20  // true, 10, 20 > 3개  >> 삼항 연산자
    > 10

<br> <br>

### 🟢 논리합 && / 논리곱 || 여산자

> && 논리곱 연산자 >> 값이 모두 true일 때 true
>
> || 논리합 연산자 >> 하나만 true여도 true

<br>

    true && true > true
    true && false > false

    true || true > true
    true || false > false

<br><br>

### 🟢 typeof 연산자

숫자, 문자열, 볼 같은 자료형을 확인할 때 사용하는 **단항 연산자**
typeof 연산자 뒤에 괄호가 없어도 상관 X

typeof 연산자는 결과로 **string, number, boolean, undefined, function, object, symbol, bigint** 중 하나는 출력

    typeof('문자열')   >  "string" // 문자열
    typeof(24)       >  "number" // 숫자
    typeof(true)     > "boolean"

    typeof '황찌'    >  "string"
    typeof 24       > "number"

    typeof 10 === 'number'    > True

<br> <br>

## 📘 템플릿 문자열

백틱을 사용하여 문자열 내부에 ${ } 안에 표현식을 넣어서 계산

    console.log(`표현식 10 + 24의 값은 ${10 + 24}입니다!)
    > 표현식 10 + 24의 값은 34입니다!

<br> <br>

## 📙 == 연산자 / != 연산자

=== 연산자 / !== 연산자 : **값과 자료형이 같은지** 비교

== 연산자 / !연산자 : **값이 같은지** 비교

    1 == '1'
    true

    false == "0" // false는 0이다
    true

    "" == []   // 빈 문자열은 false이다.
    true

    0 == []
    true
