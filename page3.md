# 조건문

### if 조건문

      if문은 보통 이런식으로 나타낸다.

      if (불 표현식) {

            // 실행되는 문장이 한 행이라면 중괄호를 생략할 수 있다. 하지만 그렇지 않다면 중괄호로 감싸야 한다.

      }

### if else 조건문

      if else 조건문의 형식은 보통 이렇습니다.

      if(불 표현식) {

           // 불 표현식이 참일 때 실행할 문장

      } else {

          //  불 표현식이 거짓일 때 실행할 문장

      }

<hr />

### 중첩조건문

      if (불 표현식) {
      
            if (불 표현식) {
            
              문장;
                  
            } else {
            
      if(불 표현식) {
      
             문장;
                  
           } else {
            
             문장;
                  
           }
            
      }
<hr />

### if else if 조건문

      if(불 표현식) {
  
                  } else if {
  
            } else {
  
      }
 
※ if else if 는 중복되지 않는 세가지 이상의 조건을 구분할때 사용합니다.

ex)

      let Date = new Date();
 
      let hours() = date.getHours();
 
            if(hours < 11) {
 
                  console.log("아침 먹을 시간");
 
            } else if {
  
                  console.log("점심 먹을 시간");
 
            } else {
 
                  console.log("저녁 먹을 시간")
 
            }
 
            -> 점심 먹을 시간

<hr />

### switch 조건문

 switch 조건문의 기본 형태
 
      switch(<비교할 값>) {
            case <값> :
                 <문장>
                 break;
            case <값> :
                 <문장>
                 break;
            default:
                 <문장>
                 break;
     }
     
   - break 키워드는 switch 조건문이나 반복문을 빠져나갈 때 사용한다.
     
   - break 키워드를 사용하지 않으면 switch 조건문을 벗어나지 않은체 문장을 읽어내린다.
     
   - switch 조건문의 괄호 안에는 비교할 값을 입력한다.
     
   - 입력한 표현식과 case 키워드 옆에 있는 표현식이 같다면 case 키워드 바로 다음에 오는 문장을 차례대로 실행한다.

<hr />

### 삼항 연산자

삼항 연산자란 프로그램의 진행을 조건에 따라 변화시킬 수 있다.

<hr />

#### 삼항 연산자의 기본 형태

    <불 표현식> ? <참> : <거짓>
    
    // 참과 거짓 위치에 불 자료형
    
    console.log(number % 2 == 0 ? true : false);
    
    // 참과 거짓 위치에 문자열 자료형
    
    console.log(number % 2 == 0 ? "짝수" : "홀수");
    
