# 조건문

### if 조건문

if문은 보통 이런식으로 나타낸다.

if (<불 표현식>) {

   실행되는 문장이 한 행이라면 중괄호를 생략할 수 있다. 하지만 그렇지 않다면 중괄호로 감싸야 한다.

}

### if else 조건문

if else 조건문의 형식은 보통 이렇습니다.

if(<불 표현식>) {

   불 표현식이 참일 때 실행할 문장

}else{

   불 표현식이 거짓일 때 실행할 문장

}
  
<hr />

### 중첩조건문

if (불 표현식) {

if (불 표현식) {

    문장;

}

} else {

if(불 표현식) {

  문장;

} else {

    문장;

  }

}

<hr />

### if else if 조건문

if(<불 표현식>) {
  
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
  
  console.log("점심 먹을 시간")
 
 } else {
 
 console.log("저녁 먹을 시간")
 
 }
 
-> 점심 먹을 시간

<hr />

