## number객체
```jsx
var num01 = 3;
alert(num01 + " : " + typeof(num01));
// type : number
```

```jsx
var num02 = new Number(3);
alert(num02 + " : " + typeof(num02));
// type : object
```

```jsx
alert(parseInt("1") + 1);
// 2
```

```jsx
alert(parseInt("a"));   //NaN
```


- `Math.random()` : 0.1 <= x < 1.0
- `Math.floor` : 주어진 숫자와 같거나 작은 정수 중에서 가장 큰 수 반환
- `Math.round` : 입력값을 반올림한 수와 가장 가까운 정수 값을 반환
- `Math. ceil` : 주어진 숫자보다 크거나 같은 숫자 중 가장 적은 숫자를 integer로 반환


## Date 객체

```jsx
var today = new Date();

            var year = today.getFullYear();
            var month = today.getMonth() + 1; //0부터 시작이라 +1
            var day = today.getDate();
```
## Date Get Methods
- `getFullYear()`
- `getMonth()`
- `getDate()`
- `getDay()`
- `getHours()`
- `getMinutes()`
- `getSeconds()`
- `getTime()`

## Array 배열
```jsx
var arrayLiteral = ["v1", "v2", 3, 4];
alert(arrayLiteral);
// v1,v2,3,4
```
- 다중 배열
```jsx
arr[0][0] = "수박";
arr[0][1] = "오렌지";
arr[0][2] = "귤";

arr[1][0] = 1;
arr[1][1] = 2;
arr[1][2] = 3;

arr[2][0] = ["python", "html"];
arr[2][1] = ["css", "javascript", "jquery"];
arr[2][2] = ["django", ["machine learning", "deep learning"]];
// 여기에서 javascript를 뽑아오려면
alert(arr[2][1][1])
```

- join 함수
```jsx
var arr = ["1", "2", "3", "4"].join("+");
// 1+2+3+4
```
- 배열 정렬
    - sort() : 문자 정렬
    ```jsx
    var arr = ["a", "c", "d", "b"];
            arr.sort();
    ```

    - sort() : 숫자 정렬
    ```jsx
    var arr = [1, 3, 2, 9, 5, 11, 24];
        arr.sort(compareNum);

    function compareNum(a, b){
            return a - b;
        }
    ```

    - reverse() : 거꾸로 출력
    ```jsx
    var arr = [19, 2, 22, 41, 33, 17];
            arr.reverse();
    ```

- 배열 저장 방식
    - push()
    ```jsx
    var queue = new Array();
    queue.push("first");
    queue.push("second");
    console.log(queue); // ['first', 'second']
    queue.push("third");
    console.log(queue);  // ['first', 'second', 'third']
    ```

    - shift()
    ```jsx
    var a = queue.shift();   // 첫번째 요소를 잘라내기 해서 가져옴
    console.log("a : " + a); // a : first
    console.log(queue);      // ['second', 'third']
    ```

    - pop()
    ```jsx
    var b = queue.pop();      // 마지막 요소 잘라내기 해서 가져옴
    console.log("b : " + b);  // b : third
    console.log(queue); 
    ```

- slice() : 배열의 부분을 가지고 새 배열 생성
```jsx
var arrayTest01 = new Array(1, 2, 3, 4, 5, 6, 7);
var array01 = arrayTest01.slice(1, 3); 
// 2, 3 출력
```

## 팝업
```
open(url, target, windowFeatuures)
```

## window
- 프로퍼티

`document`, `history`, `location`, `navigator`, `screen`, `frames`, `parent`, `top`, `self`

- 메서드

`alert()`, `confirm()`, `prompt()`, `back()`, `forward()`, `setInterval()`, `clearInterval()`, `setTimeout()`, `open()`, `close()`, `scroll(),scrollBy(), scrollTo()`