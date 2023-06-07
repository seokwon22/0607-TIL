## HTML

# web

웹은 클라이언트가 서버로 **요청**을 보내고 
서버는 클라이언트에게 **응답**을 보내는 방식으로 작동함.

http(HyerText Transfer Protocol)은 client와 server 사이의 통신규약을 뜻한다.

# html

HTML(HyperText Marup Language)는 온라인 상의 `문서`를 만들기 위해 데이터를 구조화 시키는 언어이다.

# html 요소의 구성

```
<p style='color:red;'> hello, world! </p>
```

- 요소의 내용 
`hello, world!`

- 여는 태그 : 태그의 시작을 의미 
`<p style='color:red;>`

- 닫는 태그 : 태그의 끝을 의미
`</p>`

- 속성 : 해당 태그에 적용되는 기능
`style='color:red;'`

- 요소: <여는태그> 내용 </닫는태그>
`<p style='color:red;> hello, world! </p>`


## html 블록 요소

- 줄 바꿈
- 블록 요소 안에 텍스트와 인라인 요소 포함 가능
- 블록 요소 안에 블록 요소 포함 가능 (일부 불가)

||||||
|-|-|-|-|-|
|div|fieldset|footer|form|h1|
h2|header|ol|p|section|


## html 인라인 요소

- 줄 바꿈 없음
- 인라인 요소 안에 텍스트와 인라인 요소 포함 가능
- 인라인 요소 안에 블록 요소 포함 불가

||||||
|-|-|-|-|-|
|a|br|button|em|i|
img|input|span|strong|textarea|

## semantic tag

```
<header>
    <nav>
    </nav>
</header>

<section>
    <article></article>
    <article></article>
</section>

<aside></aside>

<footer></footer>
```

## 참고 링크
- [MDN](https://developer.mozilla.org/ko/)
- [w3school](https://www.w3schools.com/)