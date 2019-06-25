# html_css

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





