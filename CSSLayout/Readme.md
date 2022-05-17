# Web programing CSS Layout

- 블로그 주소
	- https://bwoh.github.io

- Colab 주소
	- https://colab.research.google.com/drive/1xKFW2Emvd2h17yEcF2gshOAo7gQEi1JQ
	

## Web Programing CSS Layout

- CSS Layoout에 대한 학습


### emment 문법
+ html:5[tab] -> html 자동완성 기능
+ > : 자식 , + : 형제, ^ : 부모, () : 그룹화, [] : 속성, * 곱하기

### CSS Layout 문법 정리
pseudo-class:is() -> 여러개를 묶을때 사용한다.     
:nth-child() -> 짝수 또는 홀수 layout 전부다 적용     
hover -> 마우스 커서를 올려두었을 때 변화     
        
display-> grid/ flex      
__flex는 1차원적으로 수평혹은 수직 한방향으로만 레이아웃을 나눌 수 있다__       
__grid는 2차원적으로 수평 수직을 동시에 영역을 나눌 수 있다__        
 
### flex

- flex-direction
  	
배치되는 축의 방향 결정/ column, row,row-reverse,column-reverse

- flex-wrap
컨테이너가 더 이상 아이템들을 한 곳에 담지 못할때 줄바꿈을 설정한다      
nowrap, wrap, wraprevers     

- flex-flow 
flex-direction과 flex-wrap을 한꺼번에 지정할 수 있는 속성    
방향 + wrap 순으로     

- flex-basis
내부 글자크기 -> weight height auto 등등

- flex-grow
비율을 의미함. flew-basis보다 커지거나 작아질 수 있음.

### grid

- grid-template
     
grid-template-rows -> 행의 개수와 크기를 알려준다.     
grid-template-columns-> 열의 개수와 크기를 알려준다.   
gird-template-> rows와 columns 합쳐준기능 (row와 column 순서)


##### grid 영역확장
- grid-column or grid-row
grid-column 또는 grid-row로 확장 가능      
/ 앞에서부터 뒤 숫자의 앞 까지      
2 / 4: 2에서부터 4 앞까지인 3까지 (즉, 2~3 확장)      

- grid-area
첫 번째는 시작 row        
두 번째는 시작 column       
세 번째는 종료 row (전까지)        
네 번째는 종료 column (전까지)         




<code>
    .box2 {
      /* grid-column: 2 / 4; 동일 */
      grid-column: 2 / span 2;
    }
    .box4 {
      grid-area: 2 / 1 / 4 / 3;
    }
</code>



### 기타.

- media query
<code>
	@media (max-width:600px){
		.container{
			grid-template-columns: auto;
		}
		.item {
        flex-basis: 1rem;
      }
    }
</code>
 
의미: 최대 600px까지는 flex direction이 column 더 작아지면 row방향으로 바뀜       

- gap
layout 사이의 거리를 의미함.       




justify-content

grid-template-columns
grid-column

flex-basis
display
text-shadow
text-align
