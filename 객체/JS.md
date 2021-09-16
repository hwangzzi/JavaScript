# 객체

## 객체란 ?

object, 실제로 존재하는 사물을 의미하며 이름과 값으로 구성된 속성, property을 가진 JS의 기본 데이터 타입을 의미한다.

    typeof ([])
    > "object // 객체를 의미
    <br><br>

배열은 요소에 접근할 때 인덱스를 사용하지만,
객체는 키, key를 사용한다

    키:값

<br>

    const product = {
        제품명: '건조 망고',
        유형: '당절임',
        성분: '망고, 설탕',
        원산지: '필리핀'
        }

<br>

## 속성과 메소드

배열 내부에 있는 값은 요소, element
객체 내부에 있는 값은 속성, property

객체의 속성 중 함수 자료형인 속성을 메소드, method라고 부른다.

<br>

    const pet = {
        name: '구름'
        eat: function (food) { }
        }

    // 메소드를 호출
    person.eat( )

## 메소드 내부에서 this 사용하기

    // 변수 선언
    const pet = {
        name: '구름',
        eat: function (food) {
    	 alert(this.name + '은' + food + '을 먹는다.')}
    	 }

    // 메소드 호출
    pet.eat('밥')

<br>

## 동적으로 객체 속성 추가/제거

### 동적으로 객체 속성 추가

    // 객체 선언
    const student = { }
    student.이름 = '김베리'
    student.취미 = '게임'
    student.장래희망 = '오버워치'

    // 출력
    console.log(JSON.stringify(student, null, 2))

<br>
