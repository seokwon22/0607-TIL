# CSS
- css는 문서의 스타일을 지정해주는 언어이다.

## 사용방법
- inline : 태그 안에서 사용
```
<tag style='속성:값;'></tag>
```
- 내부 : head 안에서 title뒤에 사용
```
<style></style>
```
- 외부 : head 뒤에 link 태그를 사용
```
<link rel='stylesheet' href='경로'>
```

## css 우선순위
- 스타일 선언은 위에서 아래로 순차적으로 실행. 마지막에 선언된 스타일이 우선순위 가짐
- 특정 요소에 중복 선언했을 경우
inline > id > class > type

## 선택자
`type`
```
p{
    color: blue;
}
```
`id`
```
#id값{
    color: blue;
}
```
`class`
```
.class값{
    color: blue;
}
```
`전체`
```
*{
    margin: 0px;
    padding: 0px;
}
```
`자식`
```
tag > tag{
    color: blue;
}
```
`인접`
```
tag + tag{
    color: blue;
}
```
`하위`
```
#article span{
    color: blue;
}
```
`가상 클래스`
```
a;hover{
    color: blue;
}
```
`속성`
```
p[title]{
    color: blue;
}
```

## 속성 선택자
`[attr]` : attr 속성을 가진 요소 선택
`[attr=value]` : attr 속성의 값이 value와 일치하는 요소 선택
`[attr~=value]` : attr 속성의 값이 value와 일치하는 요소 선택 (공백 포함)
`[attr|= value]`  : value로 시작하는 요소들을 선택 (- 포함)
`[attr^=value]` : attr 속성의 값이 value로 시작하는 요소들을 선택
`[attr$=value]` : attr 속성의 값이 value로 끝나는 요소들을 선택
`[attr*=value]` : attr 속성의 값에 value를 포함하고 있는 요소들을 선택