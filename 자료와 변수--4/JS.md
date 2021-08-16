# 📚 자료형 변환 📚

## 문자열 입력 🅰️

    prompt(메세지 문자열, 기본 입력 문자열)

 <br>
	**prompt( )함수는 사용자로부터 내용을 입력받아서 사용**
	<br>
	
	


     const input = prompt('message', '_default')
     alert(input)

    const input = '안녕' // prompt에 내용을 입력할 경우 변환
    alert(input)



함수를 실행한 후 값을 남기는 것을 return이라고 한다.

<br><br>

## 불 입력 📙

    confirm(메세지 문자열)

<br>

    const input = confirm('수락하시겠습니까?')
    alert(input)

**confirm( )함수는 사용자에게 확인을 요구하는 메세지 창이 나타난다.**
확인 버튼은 **true** 취소 버튼은 **false**를 return한다. 따라서 input에 불 자료형이 들어가고 값이 출력된다.

<br> <br>

## 숫자 자료형으로 변환하기 🔢

    Number(자료)

다른 자료형을 **숫자 자료형으로 변환할 때** 사용

    Number("24")
    > 24

    typeof(Number("24")
    > "number"

 <br>

**> **NaN**
Not a Number**

"숫자가 아니다"라는 뜻으로 **숫자로 변환할 수 없는 경우** 출력된다.

<br>

    Number("24")
    > NaN   	// 값은 숫자가 아님

    typeof(Number("$24"))
    > "number"		// 자료형은 숫자가 맞음

<br>
Number( )함수를 사용해서 변환했기에 자바스크립트에서 자료형은 숫자이지만, 숫자로 변환할 수 없으므로 NaN을 출력.

<br><br>

### **⭐️ 불을 숫자로 변환하면 1은 true, 0은 false⭐️**

    Number(true)	> 1
    Number(false)	> 0

<br> <br>

## ➗ ➖ ➕ ✖️ 숫자 연산자로 자료형 변환하기

    "24" - 0
    > 24

    typeof("24" - 0)
    > number

    true - 0
    > 1

    typeof(true - 0)
    > "number"

<br> <br>

## 문자열 자료형으로 변환하기 🅱️

    String(자료)

다른 자료형을 **문자열 자료형으로 변환할 때** 사용
<br>

    String(3.14)
    > "3.14"

    String(true)
    > "true"

<br>

## "문자열 연산자"로 자료형 변환하기

    24 + ""
    > "24"

    true + ""
    > "true"

<br><br>

## 불 자료형으로 변환하기 📒

    Boolean(자료)

## ⭐️⭐️ 0 , NaN, ... , 빈 문자열, null, undefined는 false ⭐️⭐️

    Boolean(0)	> false

    let 변수		> undefined
    Boolean(변수) > false

<br><br>

## ‼️ 논리 부정 연산자로 자료형 변환하기 ‼️

Boolean( ) 함수 대신 **논리 부정 연산자 ! 를 2번 !!사용하면 불 자료형으로 변환** 가능

    !!24
    > true

    !!0
    > false

    !!'안녕'
    > true

    !!''
    > false
