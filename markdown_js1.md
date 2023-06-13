# Javascript
var 변수 = 값

## 변수 선언 규칙

- 대소문자 구분
- 영문, $, _로 시작
- 영문, $, _, 숫자 사용 가능
- 키워드(예약어)사용 불가

## 변수 범위

- 전역변수: window 객체에 포함됨
- 지역변수: 함수나 객체의 내부에 선언

## 타입의 종류

- string

- number

- boolean

- null

- object

- function

## alert

- alert : 경고, 코드 디버깅용

```jsx
alert(’단순 대화창’)
```

- confirm : 확인 / 취소 버튼 (true, false 리턴)

```jsx
confirm('배경을 파란색으로 변경할까요?')
```

- prompt : 텍스트박스, 확인 / 취소 버튼 ( text, null 리턴)

```jsx
var txt = prompt('좋아하는 과목을 선택해 주세요 (1:python, 2:html, 3:javascript');
```

## 함수

```jsx
function func01(){
	alert('기본 함수');
}
```

- 명시적 함수

- 익명 함수 → lambda와 거의 비슷.

- 즉시 실행 함수

- 함수 리터럴

- 클로저 (외부 함수에 접근 가능)

## control

- `if` : if {조건문} else if {조건문} else{}
```jsx
if (i == 0){
    alert('hi');
} else if(i == 0){
	alert('hey');
} else {
	alert('babe');
}
```

- `switch` : break 넣어줘야 내가 선택한거에서 멈춤. break안쓰면 선택한거부터 쭉 실행됨

```jsx
switch(~~){
case "":
	alert("");
	break;
case "":
	alert("");
	break;
}
```

- `for` : for (변수; 조건; 증감;){}의 형태로

```jsx
for(var i = 0; i < 10; i++){
}
```

- `do while` : do 안에 있는 명령 먼저 수행하고 while 조건 판별

```jsx
do{
} while{
}
```

## DOM

Document Object Model

DOM은 nodes와 objects로 문서를 표현


`getElementById` : 아이디값으로 탐색, 노드 값을 리턴
-> id는 단일값이라 Element에 's' 안붙음

`getElementsByName`, `getElementsByTagName`, `getElementsByClassName` 등등은 elements에 대한 리스트를 리턴.

*onload = 윈도우가 실행될 때.*

*innerHTML → <tag></tag> 사이에*

## 객체

객체의 구성

- property : 속성
- function(method) : 기능
- this : 객체 내부의 메서드나 속성을 정의
- prototype : 객체 확장

## string객체

- 문자열 합치기

```jsx
var str3 = str1 + " " + str2;
```

```jsx

var str4 = str1.concat(" ", str2);
```

```jsx

var joinTest = ["010", "2539", "7976"].join("-")
```

- 다른 자료형 합치기

```jsx
var numVal = 12.5;
var bool = true;
var result = 'str' + numVal + 1 + bool;

result -> str12.51true
```

- 문자열 비교하기

```jsx
== : 비교연산자
=== : 엄격한 비교연산자
```

- 문자열 검색하기

```jsx
var str = "홍길동 이순신 유재석 강호동 홍길동";
            var prop = prompt("검색할 이름을 작성해 주세요");
            alert("indexOf : " + str.indexOf(prop));
            alert("lastIndexOf : " + str.lastIndexOf(prop));
```

- 문자열 추출하기

```jsx
var strVal = "문자열 추출하기.관련 메서드:indexOf, substring.";
            var sIdx = strVal.indexOf(":");
            var eIdx = strVal.lastIndexOf(".");
            var sub = strVal.substring(sIdx+1, eIdx);
            alert(sub);

            var splitVal = sub.split(",");
            console.log(splitVal);
            alert(splitVal[0]);
            alert(splitVal[1]);
```

- 문자열 나누기

```jsx
var prop = prompt("쉼표로 구분하여 키워드를 입력하세요", "사과, 바나나, 키위, 수박");

        prop = prop.split(",");

        var result = "";
        for (i = 0; i < prop.length; i++){
            result += i + " : " + prop[i] + "<br/>";
        }

        document.getElementById("key").innerHTML = result;
```

