## 함수의 정의

> 함수의 생성 방법 3가지

+ 함수 선언문
+ 함수 표현식
+ Function() 생성자 함수

> 함수 리터럴

```javascript
function add(arg){
  return arg;
}
```

> 함수 선언문 방식
+ 반드시 함수명이 정의되어 있어야 한다.

```javascript
//add라는 함수의 이름이 반드시 필요하다.
function add(arg){
  return arg;
}
```

> 함수 표현식 방식
+ 함수를 하나의 변수로 표현하며, 익명함수를 사용한다.
+ 함수명을 정의하여도 변수의 이름으로만 호출가능
+ __함수명__ 을 사용하면 __제귀함수__ 를 __구현__ 할수 있다.

```javascript
var add = function (arg){
  return arg;
}

var div = function multi(arg){
  return arg;
}

add();  //호출 가능
div(); //호출 가능
multi(); //호출 불가

```

> Function() 함수 생성자 이용 방법

```javascript
// new Function (arg , functionbady )
var add = new Function('arg0', 'return arg');
```

