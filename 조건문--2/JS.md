# switch 조건문

- [ ] **break & default**

<br>

    switch (자료) {

    case 조건A:
        break

    case 조건B :
    	default	 // **default는 생략 가능**
    	}

<br>

    swith (input % 2) {

    case 0:
    alert('짝')
    break

    case 1:
    alert('홀')
    break

    default:
    alert('숫자가 아님')
    break
    }

<br>

## 조건부 연산자 🤔

    불 표현식 ? 참일 때 값 : 거짓일때 값

<br>

    const result = (number >=0 ' 0 이상의 숫자입니다.' : = '0보다 작은 숫자입니다.'

<br><br>

# 짧은 조건문 👀

## ➕ 논리합 연산자를 사용한 조건문

논리합 연산자를 사용한 표현식은 **무.조.건. 참**

    true || ....

<br>

    true || console.log('트루')
    > true	// 참이므로 좌변 실행

    false || console.('트루')
    > 트루	// 거짓이므로 우변을 실행
