# Web programing HTML Form

- 블로그 주소
	- https://bwoh.github.io

- Colab 주소
	- https://colab.research.google.com/drive/1c_DLlMd1aCXJ8d0glTEBWSkN34v9X_PT#scrollTo=SDMcAjAdprJu
	

## Web Programing HTML Form

- HTML Form에 대한 학습
입력폼-> 데이터 입력을 위해 채울 수 있는 양식 제공     
양식에 채운후에 __서버로 제출(HTML Form의 궁극적인 목표)__    
form에서는 type이 중요함.     

### HTML Form 문법 정리

- label
입력 폼의 데이터 라벨을 하나 생성함.

- input
	1. type -> 입력할 데이터 type 지정 -> text/ email/checkbox/radio/password/datetime-local/color
		- 메모는 input 대신해서 textarea사용함 + rows (줄지정)    
			```<textarea name="memo" rows="10"></textarea><br/>```
	2. placeholder->데이터 입력하지 않았을 시에 나타나는 글자
	3. pattern -> input의 형식을 지정해주는 것
	4. value-> 기본적으로 입력값이 더해주는 경우
	
```<input type="tel" name="phone" placeholder="010-0000-0000" pattern="01[0-9]-[0-9]{4}-[0-9]{4}"/>
<input type="text" name="search_query" value="노래방+"/><br/>```

- action
form의 데이터를 보내는 주소를 입력
```<body>
  <h3>팀장님, 노래방은 여기서 검색하세요.</h3>
  <form action="https://www.youtube.com/results">
    <label>검색 단어:</label><br/>
    <input type="text" name="search_query" value="노래방+"><br/>
    <br/>
    <input type="submit" value="제출">
  </form>
</body>```
여기서 name -> search_query가 아니면 동작X 사이트마다 다름       


