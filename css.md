# css
cascading style sheet
웹페이지를 꾸며주는 언어  html을 꾸며줌(정보는 전혀 없음)
정보와 디자인을 분리하기위해 만들어 졌음


### 적용하는법
```
1.
<style> 
 li{
    color:red;
 }

</style>
```

```
2.
```
author style -> user style -> browser 으로 cascading됨


### 기본문법
#### 선택자와 선언

```
<style>
//선택자
li {
	//선언
		//속성:값:
	color:red;
	text-decoration:underline;
}
</style>

<ul>
	<li>HTML</li>
	<li>CSS</li>
	<li>JavaScript</li>
```
#### 선택자의 종류
선택자는 꾸며줄 대상을 뜻함
```
태그 선택자
<style>
li {
	color:red;
	text-decoration:underline;
}
</style>
```

```
아이디 선택자
<style>
#slect{
	font=size:100px;
}

</style>
	
	<li>HTML</li>
	<li id="select">CSS</li>
	<li>JavaScript</li>
```
```
클래스 선택자
<style>
#slect{
	font=size:100px;
}
.deactive{
 text=decoration:line-through;
 }

</style>
	
	<h1 class ="deactive">수업의 순서</h1>
	<li class="deactive">HTML</li>
	<li id="select">CSS</li>
	<li class="deactive">JavaScript</li>
```
```
부모 자식 선택자
ul li{
 color:red;
 }
 ul 밑에있는 모든 li 들을 빨간색
 ```
