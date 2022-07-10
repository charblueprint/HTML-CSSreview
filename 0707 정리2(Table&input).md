# 3. HTML 2.0 table(1)
```HTML
<html>
<head>
<meta charset="UTF-8">
<title>HTML 1일차 HTML2.0 태그</title>
</head>
<body>
	<!-- <iframe src="https://www.nate.com/" scrolling="no" frameborder="0" width="100%" height="900"></iframe>-->
<table border="1" width="400">
  <tr height="40">
    <td width="100">123</td>
    <td>123</td>
    <td>123</td>
  </tr>
  <tr height="40">
    <td>123</td>
    <td>123</td>
    <td>123</td>
  </tr>
</table>
<table border="1" width="400" height="90" align="center">
  <tr>
    <td colspan="2">1,2</td>
    <td>3</td>
    <td>4</td>
  </tr>
  <tr>
    <td colspan="3">5,6,7</td>
    <td rowspan="2">8,12</td>
  </tr>
  <tr>
    <td>9</td>
    <td>10</td>
    <td>11</td>
  </tr>
</table>
</body>
</html>
```
***
[결과]
<html>
<head>
<meta charset="UTF-8">
<title>HTML 1일차 HTML2.0 태그</title>
</head>
<body>
	<!-- <iframe src="https://www.nate.com/" scrolling="no" frameborder="0" width="100%" height="900"></iframe>-->
<table border="1" width="400">
  <tr height="40">
    <td width="100">123</td>
    <td>123</td>
    <td>123</td>
  </tr>
  <tr height="40">
    <td>123</td>
    <td>123</td>
    <td>123</td>
  </tr>
</table>
<table border="1" width="400" height="90" align="center">
  <tr>
    <td colspan="2">1,2</td>
    <td>3</td>
    <td>4</td>
  </tr>
  <tr>
    <td colspan="3">5,6,7</td>
    <td rowspan="2">8,12</td>
  </tr>
  <tr>
    <td>9</td>
    <td>10</td>
    <td>11</td>
  </tr>
</table>
</body>
</html>
***
## iframe
**iframe** : 외부 페이지를 현재 페이지로 load하여 출력하는 태그입니다.
**width-100%** : 브라우저 가로크기를 모두 사용한다는 뜻
**frameborder** : iframe시 외곽선을 지울때 사용합니다.
## table
table : 테이블을 생성할 때 사용하는 태그입니다.
tr : 테이블의 **가로 한 줄** 입니다.
td : 테이블의 **한 칸** 입니다.

[width, height를 table에 적용하는 방식]
1.tr에 height를 사용하여 td의 높이를 모두 맞춤(* width는 사용하지 않습니다.)
2.td에는 width를 사용하나 첫번째 tr에 해당되는 td에만 width를 적용합니다.

### table 병합
**colspan** : 가로칸을 합칠 때 사용합니다. 숫자는 무조건 2부터 사용합니다.(사용하는 칸수를 입력합니다.)
**rowspan** : 세로칸을 합칠 때 사용합니다. 숫자는 무조건 2부터 사용합니다.

**align** : left,right,center 표안에 이미지, 텍스트 위치를 변경하는 태그입니다. 참고로 web은 기본이 left(왼쪽 정렬)입니다.

# 4. HTML2.0 table(2)
```HTML
<html>
<head>
<meta charset="EUC-KR">
<title>HTML 1일차 Table(HTML2.0)</title>
</head>
<body>
	<table border="1" width="450" height="30" cellspacing="0"
		cellpadding="0">
		<tr>
			<td><b>아이디</b></td>
			<td width="250"></td>
			<td rowspan="2" bgcolor="orange"><a
				href="https://www.coupang.com/np/search?component=&q=%EC%98%A4%ED%8C%94+%EB%B0%98%EC%A7%80&channel=user"
				target="_blank"><img src="./jew.jpg" width="100" height="60"></a></td>
		</tr>
		<tr>
			<td><b>패스워드</b></td>
			<td></td>
		</tr>
		<tr>
			<td colspan="3" align="center">아이디 및 패스워드 찾기</td>
		</tr>
		<tr>
			<td colspan="2">아이디 및 패스워드 저장</td>
			<td align="right">회원가입</td>
		</tr>
	</table>
</body>
</html>
```
***
[결과]
<html>
<head>
<meta charset="EUC-KR">
<title>HTML 1일차 Table(HTML2.0)</title>
</head>
<body>
	<table border="1" width="450" height="30" cellspacing="0"
		cellpadding="0">
		<tr>
			<td><b>아이디</b></td>
			<td width="250"></td>
			<td rowspan="2" bgcolor="orange"><a
				href="https://www.coupang.com/np/search?component=&q=%EC%98%A4%ED%8C%94+%EB%B0%98%EC%A7%80&channel=user"
				target="_blank"> <img src="./jew.jpg" width="100" height="60"></a></td>
		</tr>
		<tr>
			<td><b>패스워드</b></td>
			<td></td>
		</tr>
		<tr>
			<td colspan="3" align="center">아이디 및 패스워드 찾기</td>
		</tr>
		<tr>
			<td colspan="2">아이디 및 패스워드 저장</td>
			<td align="right">회원가입</td>
		</tr>
	</table>
</body>
</html>

***

## 여백 크기 설정
**cellpadding**="여백크기" : 표의 안쪽 여백 사이즈
**cellspacing**="여백크기" : 표의 바깥쪽 여백
## 배경색 설정
**bgcolor**="배경색" : backgoundcolor(배경색)

# 5. HTML3.0 - 1. input(1)
```HTML
<html>
<head>
<meta charset="EUC-KR">
<title>HTML 1일차 HTML3.0 신규태그</title>
</head>
<body>
	<input type="text">
	<br>
	<input type="password">
	<br>
	<input type="checkbox">
	<input type="radio" name="agree">동의함
	<input type="radio" name="agree">동의 안함
  <br>
	<input type="radio" name="payway"> 신용카드
	<input type="radio" name="payway"> 계좌이체
	<input type="radio" name="payway"> 휴대폰결제
	<br>
	<input type="button" value="로그인">
	<br>
	<input type="text" value="hong" readonly>
	<input type="checkbox" checked>동의함
</body>
</html>
```
***
[결과]

<html>
<head>
<meta charset="EUC-KR">
<title>HTML 1일차 HTML3.0 신규태그</title>
</head>
<body>
	<input type="text">
	<br>
	<input type="password">
	<br>
	<input type="checkbox">
	<input type="radio" name="agree">동의함
	<input type="radio" name="agree">동의 안함
  <br>
	<input type="radio" name="payway"> 신용카드
	<input type="radio" name="payway"> 계좌이체
	<input type="radio" name="payway"> 휴대폰결제
	<br>
	<input type="button" value="로그인">
	<br>
	<input type="text" value="hong" readonly>
	<input type="checkbox" checked>동의함
</body>
</html>

***
## input
(https://developer.mozilla.org/ko/docs/Web/HTML/Element/Input)를 참고해보자!
**input** : 웹 기반 양식에서 사용자의 데이터를 받을 수 있는 대화형 컨트롤을 생성하는 태그입니다.
**type**: 문자를 입력 받을 수 있는 속성을 의미합니다.

[type의 종류]
1. **text** : 사용자가 키보드 마우스 터치 사용할 때 쓰이는 타입
1. **password** : 사용자가 입력한 값을 disc모양으로 출력을 하게 됩니다.
2. **checkbox** : 마우스 클릭으로 선택할때 사용하고, 아이디를 저장하여 자동 로그인하는등 사용합니다. 또한 다중선택이 가능합니다.
   * **checked** : checkbox에서 쓰이는 속성인데, **사용자가 체크하기 이전에 미리 특정 값으로 선택**되게 할 수 있다.
3. **radio** : 단일 선택이 가능하며 그룹화를 할때는 name으로 해당 요소들끼리 묶어서 사용합니다.
4. **button** : value를 이용해서 버튼 내에 텍스트를 삽입할 수 있다.
  (button의 value와 text의 value와는 의미가 다른데, **text의 경우에는 text 필드 안에 value값이 들어가 있는 것**이다. 이 경우에는 이미 'hong'이라는 값이 삽입되어 있음을 알 수 있다. 이 저장된 값인 'hong'은 java로 넘어갑니다.)
5. **readonly** : 중복체크에 쓰이는 속성이고, **읽기전용**입니다.


# 6. HTML3.0 - 1. input(2)
``` html
<html>
<head>
<meta charset="EUC-KR">
<title>HTML3.0 기본태그2</title>
</head>
<body>
	<select>
		<option>SKT</option>
		<option>LG U+</option>
		<option>KT</option>
		<option>알뜰폰</option>
	</select>
	<br>
	<br>
	<textarea cols="50" rows="10">
		이용약관
	</textarea>
	<br>
	<form method ="post" action="https://naver.com">
	<input type="text">
	<br>
	<input type="checkbox">sms 수신동의
	<br>
	<input type="password">
	<br>
	<input type="button" value="전송" onclick="abc()">
	<input type="submit" value="전송2">
	<br>
	<input type="reset" value="취소">
	</form>
	<br>
</body>
<script>
function abc(){
location.href="https://nate.com"}
</script>
</html>
```
***
[결과]
<html>
<head>
<meta charset="EUC-KR">
<title>HTML3.0 기본태그2</title>
</head>
<body>
	<select>
		<option>SKT</option>
		<option>LG U+</option>
		<option>KT</option>
		<option>알뜰폰</option>
	</select>
	<br>
	<br>
	<textarea cols="50" rows="10">
		이용약관
	</textarea>
	<br>
	<form method ="post" action="https://naver.com">
	<input type="text">
	<br>
	<input type="checkbox">sms 수신동의
	<br>
	<input type="password">
	<br>
	<input type="button" value="전송" onclick="abc()">
	<input type="submit" value="전송2">
	<br>
	<input type="reset" value="취소">
	</form>
	<br>
</body>
<script>
function abc(){
location.href="https://nate.com"}
</script>
</html>

***

## select & option
**select** : 일반적으로 선택 태그라고 하며, 사용자가 범위 안의 내용을 선택 할 때 사용합니다. *(select - option : 부모 태그 - 자식 태그)*
**option** : **선택할 옵션을 추가** 할 때 옵션 하나당 option을 붙여 사용한다.
**textarea** : 사용자가 많은 양의 내용을 입력하고자 할 때 사용합니다. 이 textarea의 경우 태그 사이에 적힌 모든 글자를 출력하기 때문에 주석을 달면 안됩니다.

## form

**form** : 사용자가 입력한 데이터를 전송 할 때 사용합니다. submit과 reset는 **form 안**에서 사용됩니다.

  * **submit** : **내용을 전송**하는데 사용되며, 키보드 엔터를 누를 경우 작동이 됩니다.
(참고로 button과 동일해 보이지만 button은 form과는 연관이 없으며 클릭으로 진행이 됩니다.)
* **reset** : 내용을 **초기화** 합니다.

<p>
[form을 전송하는 두 가지 방법 : post, get]   

* **get** : URL 주소 뒤에 파라미터를 붙여서 데이터를 전달하는 방식입니다. post보단 빠르지만 **전달하는 내용이 보인다는 단점**이 존재합니다.
* **post** : 사용자가 입력한 데이터를 URL 주소에 붙이지 않고 **HTTP Request 헤더에 포함**시켜서 전송하는 방식입니다. 길이 제한이 없으며, 안에 있는 내용이 안 보여 **보안이 유지된다는 장점**이 존재합니다.
  하지만 get보다 느리고 뒤로가기 버튼을 누를 때 정보가 저장되어 있지 않다는 단점이 존재합니다.
</p>
