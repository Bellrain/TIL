# html

>hyper text markup language

하이퍼 텍스트를 가장 중요한 특징으로 하는 마크업 이라는 형식을 가진 컴퓨터 프로그래밍 언어
웹 브라우저와 대화하는 언어
```
<!DOCTYPE html>
<head> // 상세설명
	<meta charset="utf-8">/// 대충 우리 이런 언어로 쓸거다
	<meta name="viewport" content="width=device-width"> 
	<title>JS Bin</title>
</head>
<body> //실제 사용자들한테 보여질 내용
 <h1>heading</h1>
</body>
```


## tag
html 의 가장 기본적인 문법

```
        시작태그      닫히는 태그
인생은 <strong>고통</strong>이야 몰랐어? 
```
강조하기 

```
<h1>오늘의 영화대사 </h1>       h2 = 더작은 글씨
```
제목으로 처리하기 h1 == heading 1


```
 <ul>
  <li>기술소개</li>
  <li>기본문법</li>
  <li>하이퍼텍스트와 속성</li>
  <li>리스트와 태그의 중첩</li>
 </ul>

<ol> = 숫자매겨서 그루핑하기 <ordered list>
<ul> = un ordered list
```
그루핑 태그
```
<meta charset="utf-8">
```


글씨가 깨질땐



## 속성 =attribute

```
<a href="인터넷 주소">(황정민 - 악마를 보았다)</a>
```
하이퍼 링크 걸기

```
<a href="인터넷 주소" target="_blank">(황정민 - 악마를 보았다)</a>
title="유명한 한국영화" 커서 가져갔을때 문자 출력
```

새로운 탭에 열기

> href 와 target,title은 속성이다 
> 속성의 순서는 상관없음
> 주렁주렁 계속 필요한 속성들을 달아주면 됨

```
<p> </p> 단락 구분 태그
```
```
<br>
```
void element 그냥 줄바꿈이란 태그라서 열리는 태그만 필요 마지막에 쓰면 됨 <br> 을 넣는 개수에 따라 줄을 띄우는 간격이 늘어남 
```
<img src="파일명.jpg" width="크기숫자" height="높이 숫자" alt="이미지에 문제가 생겼을때 대신 출력할 값"> title 사용가능 
```
이미지 올리는 태그 닫을 필요 없음

### 표만들기
```
<table border="1,2">
<thead>
<tr>
 <th>이름</th>     <th>성별</th>   <th>주소</th>
</tr> 
</thead>
<tbody>
<tr>
 <td>최진혁</td>    <td>남</td>     <td>청주</td> 
</tr>
<tr>
 <td>최유빈</td>    <td>여</td>     <td>청주</td> 
</tr>
</tbody>
</table>
```
과거에는 레이아웃을 잡을때 웹페이지전체를 표로 써서 잡을 때도 있었다

```
셀병합
<td rowspan="숫자">
<td  colspan="숫자">
```
### form

```
<html>
<body>
<form action="제출버튼 누르면 여기로 보내라">
	<p>아이디 :<input type="text"name="id"></p>
	<p>비밀번호 : <input type='"password" name="pwd"></p>
	<p><input type="submit"> //제출버튼</p>
</form>
</body>
</html>
```
####  문자입력
```
<form action="">
	<input type="text" name="id" value="default value">
	<input type="password" name="pwd" value="default value">
	text area : 
 <textarea cols="50" rows="10">default value</textarea>
```

#### Dropdown list
선택지 만들기
```
<form>
	<h1> 색상</h1>
		<select name="color">
			<option value="red">붉은색</option>	
			<option value="blue">파란색</option>
			<option value="yellow">노란색</option>
		<select>
	<input type="submit">
	<h1> 색상2</h1>
	<select name="color2" multiple>
			<option value="red">붉은색</option>	
			<option value="blue">파란색</option>
			<option value="yellow">노란색</option>
		<select>
	<input type="submit">
</form>
```



## Checklist
* HTML 표준의 역사는 어떻게 될까요?
  * HTML 표준을 지키는 것은 왜 중요할까요?
```
  html 표준을 지키는 것은 다른 여러 표준들을 지키는 것처럼 중요하다. 정보를 차별없이 제공하고 웹 브라우저의 종류나 버전에 상관없이 모든 사용자들이 동일한 웹사이트를 보게 하기위해 표준을 지키는 것이 중요하다.
```
  * XHTML 2.0은 왜 세상에 나오지 못하게 되었을까요?
 ```
  XHTML이 html 이 할수 없는 몇가지 일을 할수 있지만 어느정도의 자잘한 오류는 무시하고 실행할 수 있는html과 달리 엄격하게 문법을 지켜야하는 xhtml이 개발자들에게 받아들여지지 않았고 결국 html5를 개발하는 방향으로 선회하게 된다
```
  * HTML5 표준은 어떤 과정을 통해 정해질까요?
* 브라우저의 역사는 어떻게 될까요?
  * Internet Explorer가 브라우저 시장을 독점하면서 어떤 문제가 일어났고, 이 문제는 어떻게 해결되었을까요?
  * 현재 시점에 브라우저별 점유율은 어떻게 될까요? 이 브라우저별 점유율을 알아보는 것은 왜 중요할까요?
  * 브라우저 엔진(렌더링 엔진)이란 무엇일까요? 어떤 브라우저들이 어떤 엔진을 쓸까요?
  * 모바일 시대 이후, 최근에 출시된 브라우저들은 어떤 특징을 가지고 있을까요?
* HTML 문서는 어떤 구조로 이루어져 있나요?
  * `<head>`에 자주 들어가는 엘리먼트들은 어떤 것이 있고, 어떤 역할을 할까요?
  * 시맨틱 태그는 무엇일까요?
    * 시맨틱 엘리먼트를 사용하면 어떤 점이 좋을까요?
    * `<section>`과 `<div>`, `<header>`, `<footer>`, `<article>` 엘리먼트의 차이점은 무엇인가요?
  * 블록 레벨 엘리먼트와 인라인 엘리먼트는 어떤 차이가 있을까요?
