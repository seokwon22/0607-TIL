# HTML
- 문서를 구조화 시키는 언어이다.


## 블럭 요소
- 줄 바꿈 요소.
- `article`, `dd`, `div`, `dl`, `fieldset`, `footer`, `form`, `h1`, `h2`, `header`, `ol`, `p`, `section`, `table` ...

## 인라인 요소
- 줄 바꿈 없음
- `a`, `br`, `button`, `em`, `i`, `img`, `input`, `span`, `strong`, `textarea` ...

## 기본 구조
```
<html>
    <head>
        <meta>
        <title></title>
    </head>
    <body>
    </body>
</html>
```

## html sematic tag
```
<header>
    <nav></nav>
</header>

<section>
    <article></article>
    <article></article>
</section>

<footer></footer>
```

## Form
- 클라이언트가 서버로 요청을 보내면 서버는 클라이언트에게 응답한다

- 전송방식
    - GET : request header에 data 담아서 전송 (queryString)
    - POST : request body에 data 담아서 전송

*queryString이란?*
- k=value&k=value&k=value 형태로 전달되는 문자열


## 다양한 tag들
`p`
```
<p>hello world</p>
```
`a`
```
<a href='https://www.naver.com'>네이버</a>
```
`list`
- ordered list (ol)
```
<ol>
    <li></li>
<ol>
```
- unordered list (ul)
```
<ul>
    <li></li>
<ul>
```
- description list (dl)
```
<dl>
    <dt></dt>
    <dd></dd>
<dl>
```
`table`
```
<table>
        <tr>  <!-- table row -->
            <th>컬럼1</th> <!-- table heather -->
            <th>컬럼2</th>
        </tr>
        <tr>
            <td>데이터1</td>
            <td>데이터2</td>
        </tr>
        <tr>
            <td>데이터3</td>
            <td>데이터4</td>
        </tr>
    </table>

```
```
<table border="1">
    <caption>테이블 제목</caption>
    <colgroup>
        <col width="100px" />
        <col width="200px" />
    </colgroup>
    <thead>
        <tr>
            <th>컬럼1</th>
            <th>컬럼2</th>
            <th>컬럼3</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>1</td>
            <td>2</td>
            <td>3</td>
        </tr>

        <tr>
            <td>4</td>
            <td>5</td>
            <td>6</td>
        </tr>
    </tbody>

    <tfoot>
        <tr>
            <td>foot1</td>
            <td>foot2</td>
            <td>foot3</td>
        </tr>
    </tfoot>
</table>
```

`form`
```
<form action='경로' method='전송 방식'>
    <input type='형태' name='name' value='value'>
    <input type='submit' value='전송'>
</form>
```