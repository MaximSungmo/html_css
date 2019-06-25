HTML



CSS - 선택자 

- 태그 선택자  : 선택자  {  속성: 속성값;  }

- Class 선택자 : .CLASSNAME { 속성이름: 속성값; }

- ID 선택자 : #ID { 속성이름: 속성값; }

- 종속 선택자 :  h1#head { … }  | .headline.selected { … }  |  input#user-id.focused { …}  |  p.title { … }

- 하위 선택자 : body h1, body h2, body p { … }  |  p .txt1 { … }   .headline span

- 그룹 선택자 : body h1, body h2, body p { … }  | .right_box, .left_box { … }

- 수도 선택자(Psuedo Selector) : 

  ```css
  :hover   -> 마우스의 커서가 올라가 있는 상태
  :active  -> 마우스 커서를 클릭한 순간부터 놀기 직전까지 상태
  :link    -> 링크를 클릭하지 않은 그냥 링크만 되어 있는 상태
  :visited -> 링크를 눌러서 방문한 후 상태
  :before  -> 문장이 시작되기 전
  :after   -> 문장이 끝난 다음
  ```

- 전체 선택자 : 브라우저별로 기본 셋팅값이 다르므로 전체 초기화를 해주어야함

  \* { margin:0; padding:0 }    |    #idname *  또는  .classname *

주석 : /* */ 만 사용할 수 있다.   



우선 순위

ID > Class > 태그 

각 요소당 점수를 매겨서 비교하므로 하위 선택자를 고르는 경우에서 우선 순위가 동일한 선택자가 나올 경우에는 코드 실행 순서에 의하여 마지막에 실행된 것이 적용된다. 



CSS - 박스모델

1. 마진과 패딩

- ```css
  /*방법1.  4개의 방향을 각각 지정*/
         margin-top:10px;
         margin-right:20px;
         margin-bottom:30px;
         margin-left:40px;
  /*방법2. 각 방향으로 한꺼번에 지정하는 단축형*/
         margin: 10px 20px 30px 40px;   
  ```

- ```css
  /*width 와 height 지정*/
  width: 속성값 
  height: 속성값
  /*width 와 height의 속성값은 %(퍼센트) 또는 px(픽셀 사용)최대(최소) width 와  최대(최소) height 지정*/
  max-width: 속성값
  min-width: 속성값      
  max-height: 속성값 
  min-height: 속성값 
  ```

2. 백그라운드 이미지

- ```css
  background-: 속성값  
  속성값 리스트
  color:  색상을 지정,
  image:  배경 이미지 지정 URL(‘……’)
  repeat: 배경이미지의 반복  repeat, no-repeat, repeat-x, repeat-y
  position:  백그라운드 이미지의 위치  x,y 축을 기준으로  픽셀  값으로 지정
  ```

3. 박스모델 

- ```css
  float: right(오른쪽), left(왼쪽), none(없음)
  ```



CSS - 글꼴 및 텍스트의 이해

1. 글꼴 사이즈 지정

```CSS
font-size: 12px  과  font-size : 75% 는 같다.
% 보다는 em를 많이 쓴다.
font-size: 12px  과  font-size : 0.75em 은 같다.
```

2. 텍스트 처리방법

- ```CSS
  line-height: 속성값  ( px, %, em )
  ```

  

