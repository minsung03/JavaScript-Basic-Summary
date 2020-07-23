# 조건문

### if 조건문

let input = 32;

if ( input % 2 == 0 ) { // input을 2로 나누었을 때 나머지가 0이라면 짝수 출력

  console.log("짝수");

}

if( input % 2 == 1 ) { // input을 2로 나누었을 때 나머지가 1이라면 홀수 출력

console.log("홀수");

}

-> 짝수

<hr />

### 현재 시간 구하기

let Date = new Date();

console.log(date.getFullYear());

console.log(date.getMonth());

※ getMonth는 0부터 11까지 반환되므로 1을 더해야한다.

console.log(date.getDay());

console.log(date.getHours());

console.log(date.getMinutes());

console.log(date.getSeconds()); 

