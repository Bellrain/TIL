# html

>hyper text markup language

하이퍼 텍스트를 가장 중요한 특징으로 하는 마크업 이라는 형식을 가진 컴퓨터 프로그래밍 언어
웹 브라우저와 대화하는 언어





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



## 속성

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

