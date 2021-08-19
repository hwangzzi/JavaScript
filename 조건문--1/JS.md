조건문 - if

**조건에 따라서 코드를 실행하거나 실행하지 않을 때 사용하는 구문**으로 _코드가 실행되는 흐름을 변경_ 할 수 있다
→ _조건 분기_

    if(불 값이 나오는 표현식) {
        값이 참일 때 실행할 문장 }

<br>

    if (25 < 100) {
    alert('25 > 100 => true')
    }

    alert('종료')  //  > 종료가 출력

<br> <br>

## if else 조건문 🤔

else 구문은 if 조건문 바로 뒤에 붙여 좀 더 편리하게 조건문을 사용할 수 있도록 **반대되는 상황**을 표현하는 구문

    const date = new Date()
    const hour = date.getHours()


    if ( hour < 12) {
    alert('오전')
    }
      else {
    alert('오후')
    }

<br><br>

## 중첩 조건문 🤔

조건문 안에 조건문을 중첩해 사용하는 것

<br>

    if (hour < 11) {
    alert('아침 먹을 시간')
    }

     else {
    if (hour < 15) {
    alert('점심 먹을 시간')
    }

    else {
    alert('저녁 먹을 시간') }
    }

<br>
<br>

## if else if 조건문 🤔

if 조건문은 조건이 한 문장일 때 중괄호가 생략이 가능한데, **중첩 조건문에서 중괄호를 생략한 형태**가 if else if 조건문이다.

**겹치지 않는 3가지 이상의 조건**을 나눌 때 사용.

<br>

    if (hour < 11) {
    alert('아침 먹을 시간')
    }

     else if
    if (hour < 15) {
    alert('점심 먹을 시간')
    }

    else {
    alert('저녁 먹을 시간')
    }
