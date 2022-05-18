# Web programing CSS

- 블로그 주소
	- https://bwoh.github.io

- Colab 주소
	- https://colab.research.google.com/drive/1aHHrMcM1RqbtLBGmZsOCU46RIo1w-ijg
	

## Web Programing CSS

- CSS에 대한 학습


### CSS 란?
__Cascading Style Sheets로 연쇄적으로 따라가서 스타일 sheet을 바꾸어라는 의미이다__     
css문서를 통해서 HTML 문서를 어떻게 표현할지 세부사항을 기술함      
=> 어떤것을 표시하는지, 어떻게 표현할지 알려주어야함    
_어떤것 -> Selector (element /class /ID)로 나뉨_      
_어떻게 표현할지 -> Declaration (property:value)형식으로 표현함._     

#### selector
Element(tag, 여러개도 가능) -> tag사용, 여러개는 콤마로 구분, 전체는 *     
class(.사용) -> .class이름// 공통된 특성을 묶은 그룹을 의미     
ID(#사용) -> 고유 식별자 #사용 #id값     


#### CSS 사용방법
1. HTML head부분에 style element 사용
2. 별도의 파일에 CSS 저장
	-link rel='stylesheet' href='index.css' 이렇게 head에 선언하고 파일 분리가능.
3. HTML element내에서 style애트리뷰트 지정 (적용순위 가장 높음)
4. [] => attribute selector임

#### CSS 기본 함수

```div > li -> 직계 자손들만 적용
div li -> div로 감싸져있는 li 전부다 의미
 (*) -> 모든 것에 대한 것을 의미
div , li-> div와 li에 해당되는 것을 의미
```


#### emment 기능
emment란? 자동완성기능을 의미한다.

```
 ex) div>li + tab -> div와 li 생성
 ex) div>ul>li*5 -> div와 ul 밑에 li 5개 생성
 ex) div>ul$*3>li$*3 -> $-> 순서를 생성해줌 ul1, ul2, ul3 // li1 li2 li3
 ex) div.container>ul.character -> div의 css class를 설정해준다.
```

