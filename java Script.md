# java script

정적인 html에 더해 **사용자와 상호 작용** 할 수 있는 웹페이지를 만들어주는 언어


html 과 연결하는법
```
1. script tag
<body>
    <script>
    document.write(1+1); //html에선 할수없지만  java 에서는 2로 출력할 수 있다.
   </script>

</body>
```

```
2. 이벤트  --- on 붙은애들 
<body>
  <input type=" button=" value"hi" onclick="alert('hi')">  // onclick =javascript 전용 속성
  <input type="text" onchange="alert('changed')"> //onchange= 변화감지
  <input type="text" onkeydown="alert('key down')"> // onkeydown= 키눌렀냐?
</body> 
```

## 제어할 태그 선택하기
```
document.querySelector('body').style.backgroundColor = "black";
document.querySelector('#target')
document.querySelector('.classname')
```

## 연산자
```
=== 같냐? //비교연산자
```



 
