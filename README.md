# 숙제 안하면 라면만 ( 까르보나라 금지 )
[민성](#김민성)
<hr/> 

## 자바스크립트 입문   
#### part1, part2(12,13,14)   

<hr/>

## Jquery 인터랙티브       
#### page chapter2까지 ( 미션도전 제외 )    


## 자바스크립트 입문 part1 정리  
<hr/>

## 키워드   

### 키워드는 특별한 의미가 부여된 단어이다.    

<hr />

#### break else true case false function... 등의 키워드가 있다.

<hr />

## 식별자

### 식별자는 이름을 붙일 때 사용하는 단어이다. 변수와 함수 이름 등으로 사용된다.

#### 식별자 이름을 붙힐 때 주의할 점

- 키워드를 사용하면 안된다.
- 특수 문자는 _ 와 $ 만 허용된다.
- 숫자로 시작하면 안된다.
- 공백은 입력하면 안된다.
  
  ex) alpha(o) 273alpha(x)
### JavaScript 식별자의 종류

- 식별자 뒤에 괄호가 없으면 변수또는 상수가 단독으로 사용되고, 속성이 다른 식별자와 사용된다.

- 식별자 뒤에 괄호가 있으면  함수가 단독으로 사용이 되고, 메소드가 다른 식별자와 사용된다.

### 식별자의 의미를 더 명확하게 하려고 사용하는 규칙 3가지

- 생성자 함수의 이름은 항상 대문자로 시작합니다.

- 변수, 함수, 속성, 메소드의 이름은 항상 소문자로 시작합니다.

- 여러 단어로 된 식별자는 각 단어의 첫 글자를 대문자로 합니다.

ex) will out => willOut, will return => willReturn, i am a boy => iAmABoy

<hr />

## 주석

주석은 프로그램의 진행에 전혀 영향을 주지 않은 코드이다. 주로 코드를 설명할때 사용한다.

### 한 줄 주석 처리 => //주석 (//뒤에 주석은 실행되지 않는다.)

### 여러 줄 주석 처리 => /* 여러줄 주석 * / ( /* 사이의 주석은 실행되지 않는다. */ )

ex) // 주석은 코드실행에 영향을 주지 않습니다.

   /* 
   
   console.log("asd");
   
   console.log("asd");
   
   console.log("asd");
   
   */
   
<hr />


## 출력

### 출력 메소드

자바스크립트의 가장 기본적인 출력 방법은 console  console 객체의 log() 메소드를 사용하는 것이다.

<hr />

## 기본 자료형

### 숫자

가장 기본적인 자료형은 숫자이다. 0,1,2,3 같은 것을 말한다.

#### JavaScript의 숫자 생성

console.log(1);
console.log(1.323);

#### 연산자 종류

+ : 덧셈연산자

- : 뺄셈연산자

* : 곱셈연산자

/ : 나눗셈연산자

### 연산자 우선순의

console.log(5 + 3 * 2)
 
 16 이라고 나온다면 우선순위가 적용이 되지 않은 것이다. 곱셈이 덧셈보다 우선순위가 높기 때문에 곱셈을 먼저 계산해야 한다.
 
 만약 앞에 두 수를 먼저 더하고 싶으면 (5 + 3) * 2 처럼 괄호를 사용해야 한다.
 
<hr />

### 나머지 연산자 %

10 % 5 => 0

7 % 3 => 1

숫자의 나머지를 구한다고 보면 된다.

### 숫자와 연산자

1. console.log(1 + 2);
=> 3

2. console.log(1 - 2);
=> -1

3. console.log(1 * 2);
=> 2

4. console.log(1 / 2);
=> 0.5

5. console.log(1 % 2);
=> 1

<hr />

### 음수와 나머지 연산자

나머지 연산자의 부호는 왼쪽 피연산자의 부호를 따르므로 오른쪽의 부호는 전혀 상관이 없다.

console.log(4 % 3);
=> 1

console.log(-4 % 3);
=> -1

console.log(4 % -3);
=> 1

console.log(-4 % -3);
=> -1

<hr />

### 소수점이 있는 숫자와 나머지 연산자

console.log(5.0 % 2.2); 

소수점이 있는 숫자연산에 제한이 있기 때문에 0.5999999999999996이라고 출력이 된다. 이러한 현상은 대부분의 프로그래밍 언어에서 발생하는 문제이다.

따라서 소수점이 있는 숫자에 나머지 연산자를 적용하면 안된다.

<hr />

## 문자열

문자의 집합을 문자열이라고 한다.

ex) 'abcdefg', 'Hello World', '안녕하세요' 등....

### 기본 문자열

자바스크립트는 기본적인 문자열을 생성할 때 큰 따옴표나 작은따옴표를 사용합니다.

ex) "안녕하세요"
   => '안녕하세요'
   
   '안녕하세요'
   => '안녕하세요'
   
어떤 방법으로 문자열알 만들어도 상관없지만. 따옴표는 항상 일관되게 사용하는 것이 좋다.

다만 문자열 내부에서 따옴표를 사용해야 한다면, 예외적으로 당므 두 가지 따옴표를 모두 씁니다.

console.log("This is 'String'");

=> This is 'String'

console.log('This is "String"');

=> This is "String"

<hr />

### 이스케이프 문자

따옴표 앞에 \를 붙히면 따옴표를 문자 그대로 사용할 수 있다.

ex) console.log("This is \"String\"")

-> This is "String"

console.log("This is \'String\'')l
This is 'String'

### 자주 사용하는 이스케이프 문자들

\t -> 수평탭

\n -> 줄바꿈

\' -> 작은따옴표

\" -> 큰따옴표

\\ -> 역슬래시

ex) console.log("이름\t나이");

-> 이름    나이

console.log("안녕\n하세요");

-> 안녕
  
   하세요
   
console.log("\\\\");

-> \\

<hr />

### 문자열 연결 연산자

문자열 연결 연산자로 서로를 연결한다.

console.log("가나다" + "라마" + "바사아" + "자차카타" + "파하");

-> 가나다라마바사아자차카타파하

<hr />

### 문자 선택 연산자

문자열[숫자] = 문자 

ex) console.log("안녕하세요"[0]);

-> 안

    console.log("안녕하세요"[1]);
    
-> 녕

    console.log("안녕하세요"[3]);
    
-> 세

<hr />

### 템플릿 문자열

ex) `안녕하세요`

->'안녕하세요'

` 기호로 문자열을 생성하면 출력으로 작은따옴표로 만든 문자열이 나오는 것을 확인할 수 있다. 템플릿 문자열은 생성이후 일반문자와 똑같이 취급된다.

하지만 템플릿 문자열은 생성할때 내부에 ${<표현식>}을 사용할 수 있다. 내부에 ${<표현식>}을 입력하면 표현식이 계산되어 문자열이 들어간다.

ex) `52 + 273 = ${52 + 273}`

-> '52 + 273 = 325'

`올해는 ${new Date().getFullYear()}년입니다.`

-> '올해는 2020년입니다.'

템플릿 문자열은 굉장히 편리한 기능이지만 최신 웹브라우저에서만 사용할 수 있다.
따라서 모든 버전의  익스플로러에서 사용할 수 있는 것은 아니므로 각별한 주의가 필요하다.

<hr />

### 템플릿 문자 대체 방법;

'52 + 273' = ' + (52 + 273)

-> '52 + 273 = 325'

'올해는 ' + new Date().getFullYear() + '년입니다.'

-> 올해는 2020년입니다.

<hr />

### 템플릿 문자열과 문자 선택 연산자

ex)

`올해는 ${new Date().getFullYear()}년입니다.`[]

-> 2

`올해는 ${new Date().getFullYear()}년입니다.`[]

-> 0

`올해는 ${new Date().getFullYear()}년입니다.`[]


-> 2
`올해는 ${new Date().getFullYear()}년입니다.`[]

-> 0

<hr />

### 불

불은 참과 거짓으로 표현할깨 사용한다.

ex)

true -> true

false -> false

<hr />

### 비교 연산자

== 같습니다

!= 다릅니다.

> 왼쪽 피연산자가 큽니다.

< 오른쪽 피연산자가 큽니다.

>= 왼쪽 피연산자가 크거나 같습니다.

<= 오른쪽 피연산자가 크거나 같습니다.

<hr />

### 불과 비교 연산자

console.log(52 < 273);

-> true
console.log(52 > 273);

-> false


console.log("하마" < "가방");

-> false

### 논리 연산자

! : 논리 부정 연산자

|| : 논리합 연산자

&& : 논리곱 연산자

<hr />

### 논리 부정 연산자

console.log(!true)

-> false

console.log(!false)

-> true

console.log(!(52 < 273))

-> false

console.log(!(52 > 273))

-> true

<hr />

### 논리합 연산자

논리합 연산자는 2개의 피연산자 중에 하나만 true이면 전체가 true되는 연산자입니다. 일반적으로 논리합 연산자는 또는(or) 이라고 불린다.

왼쪽 피연산자 true    오른쪽 피연산자 true    결과  true

왼쪽 피연산자 true    오른쪽 피연산자 false   결과  true

왼쪽 피연산자 false   오른쪽 피연산자 true    결과  true

왼쪽 피연산자 false   오른쪽 피연산자 false   결과  false


ex)

"치킨 또는 배 먹을래?" -> "응 치킨 먹을게."

"치킨 또는 개미 먹을래?" -> 응 치킨 먹을게."

" 개미 또는 개미 먹을래?" -> "안 먹으면 안 되겠니.."

<hr />

### 논리곱 연산자

논리곱 연산자는 2개의 피연산자 모두 true여야 전체가 true되는 연산자이다. 일반적으로 and 연산자로 불린다.

왼쪽 피연산자 true    오른쪽 피연산자 true    결과  true

왼쪽 피연산자 true    오른쪽 피연산자 false   결과  false

왼쪽 피연산자 false   오른쪽 피연산자 true    결과  false

왼쪽 피연산자 false   오른쪽 피연산자 false   결과  false

<hr />

ex)

"치킨 배 둘 다 먹을래?" -> "응 모두 먹을래"

"치킨 똥 둘 다 먹을래?" -> "안 먹으면 안 되겠니..."

"똥과 똥 둘 다 먹을래?" -> "안 먹으면 안 되겠니..."

### 비교연산자의 잘못된 사용

30 > 20 > 10의 결과는 무엇일까?

30 > 20 > 10

(30 > 20) > 10

true > 10

1 > 10

false

이러한 문제를 해결하려면 비교연산자와 논리연산자를 함께 사용 해야한다. 따라서 이러한 범위를 표현할 때 "반드시" 범위 연산자를 사용해야 한다.

<hr />

### 불과 논리 연산자

let hours = (new Date()).getHours();

console.log(hours < 3 || 8 < hours);

-> false

console.log(3 <= hours && hours <= 8);

-> true

## 변수

변수는 값을 저장할 때 사용하는 식별자이다. 이름은 변수지만 숫자뿐만 아니라 모든 자료형을 저장할 수 있다.

변수는 다음 두단계를 거쳐서 사용할 수 있다.

let 식별자;

다음은 변수 pi를 선언한 것 입니다.

let pi;

변수의 값을 지정하는 것을 '변수에 값을 할당한다'고 표현합니다.

ex)

let pi;

pi = 3.14

변수를 선언한 후 처음 값을 할당하는 것을 '변수를 초기화한다'고 표현한다.

let pi = 3.14;

변수에 값을 저장하면 변수를 사용해 저장된 값을 활용할 수 있다.

ex) 

let pi = 3.14;

console.log(pi);

-> 3.14

<hr />

### 변수의 기본 사용방법

let pi = 3.14;

let radius = 10;

console.log(`둘레: $({2 * pi *radius}`);

console.log(`넓이 : ${pi * radius * radius}`);

둘레 : 62.8
넓이 : 314

변수에 자료형을 지정하지 않기 때문에 동일한 변수에도 여러종류의 자료형을 넣을수 있다.

하지만 이런 유연성 때문에 어떤 자료형이 들어있는지 몰라 런타임 에러가 발생할 확률이 높아지므로 하나의 변수에는 하나의 자료형만 넣어서 활용하는 것이 좋다.

### 복합 대입 연산자

ex)

  a+=10
  
복합 대입 연산자

+= 숫자 덧셈 후 대입 연산자

-= 숫자 뺄셈 후 대입 연산자

*= 숫자 곱셈 후 대입 연산자

/= 숫자 나눗셈 후 대입 연산자

문자열도 문자열 연결 연산자(+)와 = 연산자를 합쳐 복합 대입 연산자를 사용할 수 있다.

<hr />

### 문자열에 적용하는 복합 대입 연산자

+= : 문자열 연결 후 대입 연산자

### 숫자와 관련된 복합 대입 연산자

let output = 0;

output += 52;

output += 273;

output += 103;

console.log(output);

-> 428

<hr />

문자열과 관련된 복합 대입 연산자

let output = "hello";

output += "world";

output += "!"

console.log(output);

-> hello world !

### 증감연산자

변수++ : 기존 변수 값에 1을 더합니다(후위)

++변수 : 기존 변수 값에 1을 더합니다(전위)

변수-- : 기존 변수 값에서 1을 뺍니다(후위)

--변수 : 기존 변수 값에서 1을 뺍니다(전위)

ex)

let number = 10;

number++;

console.log(number);

number--;

console.log(number);

-> 11

-> 10

<hr /?

### 증감 연산자의 전위와 후위

#### 전위

let number = 10;

console.log(number);

-> 10
console.log(++number);

-> 11

console.log(--number);

-> 10

console.log(number);

-> 10

#### 후위

let number = 10;

console.log(number);

-> 10

console.log(number++);

-> 10

console.log(number--);

-> 11

console.log(number);

-> 10

<hr />

### 자료형 검사

변수의 자료형을 확인할 때는 typeof 연산자를 사용합니다.

typeof : 해당 변수의 자료형을 출력한다.

typeof 10

'number'

typeof("문자열")

'string'

보통은 연산자 뒤에 괄호를 붙혀서 사용한다.

ex)

typeof(10)

'number'

typeof("문자열")

'String'

<hr />

자바스크립트에는 여섯 가지 자료형이 있다.

// 문자열

typeof('string')

-> 'string'

// 숫자

typeof(273)

-> 'number'

// 불

typeof(true)

-> 'boolean'

// 함수

typeof(function() { })

'function'

// 객체

typeof({})

'object'

// undefined

typeof(alpha)

'undefined'

<hr />

### undefined 자료형

자바스크립트에는 초기화되지 않은 것을 표기하는 자료형이 있다. 바로 undefined 자료형이다. undefined 자료형은
변수를 선언했으나 초기화하지 않았을 때를 나타낸다.

let a 

-> undefined 

변수 a를 선언했으나 초기화하지 않았으므로 undefined 자료형이다.

<hr />

### 강제 자료형 변환

강제 자료형 변환 함수

Number() = 숫자로 자료형을 변환한다.

String() = 문자열로 자료형을 변환한다.

Boolean() = 불로 자료형을 변환한다.

String에 1,2,3.. 등의 숫자를 넣으면 문자열 '1'.'2'... 등이 출력된다.

true,false인 불을 넣으면 'true', 'false'라는 문자열로 변환된다.

<hr />

### number 함수와 NaN

문자열이나 불을 숫자로 변환할 때는 Number() 함수를 사용한다.

ex)

console.log(Number("52"));

-> 52

console.log(Number("52.273")):

-> 52.273

console.log(Number(true)):

-> 1

console.log(Number(false)):

-> 0

console.log(Number("안녕하세요")):

-> NaN

NaN은 Not a Number의 줄임말로 숫자 자료형이지만 숫자가 아닌 것을 의미한다.

NaN의 특징

- NaN은 무조건적으로 다르다.
- NaN인지 확인할 때는 isNaN() 함수를 사용한다.

ex) 

// Nan 변수를 만든다.

let nan = Number("안녕하세요");

//NaN 끼리 비교

console.log(nan == nan);

-> false

console.log(nan != nan);

-> true

//isNaN() 함수로 NaN인지 확인한다.

console.log(isNaN(nan));

-> true

<hr />

### Boolean 함수

자바스크립트에서 Boolean() 함수를 사용하면 다음 5개의 요소는 false로 반환된다.

- 0

- NaN

- ""[빈 문자열]

- null

- undefined

위에 5개 이외에는 전부 true로 변환이 된다.

ex)

// 변수를 선언한다.

let nan = Number("안녕하세요");

let undefinedVariable;

// Boolean() 함수를 사용한다.

console.log(Boolean(0));

-> false

console.log(Boolean(nan));

-> false

console.log(Boolean(""));

-> false

console.log(Boolean(null));

-> false

console.log(Boolean(undefinedVariable));

-> false

<hr />

### 자동 자료형 변환

자바스크립트는 일부 자료형을 상황에 따라 자동으로 변환한다.

<hr />

### 숫자와 문자열 자료형 자동 변환

console.log(52 + 273);

-> 325

console.log("52" + 273);

-> 52273

console.log(52 + "273");

-> 52273

console.log("52" + "273");

-> 52273

<hr />

### 불 자료형 자동 변환

ex)

// 변수를 선언한다.

let nan = Number("안녕하세요");

let undefinedVariable;

// 부정 연산자를 두 번 사용한다.

console.log(!!0);

-> false
console.log(!!nan);

-> false
console.log(!!"");

-> false

console.log(!!null);

-> false

console.log(!!undefinedVariable);

-> false

<hr />

### 일치 연산자

=== : 자료형과 값이 같은지 비교한다.

!== : 자료형과 값이 다른지 비교한다.

기존에 살펴 보았던 비교 연산자는 '최대한 자료형을 맞춰서 비교'를 수행한다. 따라서 0과 ""[빈 문자열]을 비교하면 둘 다 불로 변환하면 false가 되니까 true라는 결과가 나온다.

조금 예측하기 힘들기 때문에 자바스크립트는 '자료형까지 검사하는' 일치 연산자를 제공하는 것이다.

<hr />

### 비교연산자와 일치연산자의 차이

console.log(`52 === "52" : ${52 == "52"}`);

-> 52 == "52" : true

console.log(`52 === "52" : ${}52 === "52"}`);

-> 52 === "52" : false

console.log();

console.log()`0 == "" : ${0 == ""}`);

-> 0 == "" " true

console.log(`0 == "" : ${0 === ""}`);

-> 0 === "" : false

참고로 == 연산자와 != 연산자는 예상하지 못한 결과가 나올 수 있으므로 대부분의 자바스크립트는 === 이나 !== 연산자를 사용해 비교하는 것을 권장한다.

<hr />

##상수

ECMAScript6 부터는 const 상수 생성 키워드가 추가되었다.
const는 상수를 만드는 키워드이다. 상수는 항상 같은 수라는 의미로 변수와 반대되는 개념이다.

### 상수는 왜 사용할까?

상수는 프로그램을 조금 더 읽기 쉽고, 빠르고 안정적으로 만들려고 사용한다. 값에 이름을 붙여 읽기 쉽게 만들었다는 것은 변수도 마친가지이지만, 상수는 "변하지 않는 것"이라고 강제 한것이기

때문에 자바스크립트가 내부적으로 간단한 형태로 저장되어 있다.

또한, 프로그램을 개발하다 보면 "이걸 왜하지? "라고 생각이 들 때가 있는데 그런 짓을 막을때 사용하는것이 상수이다.

예를 들면 pi를 3.14로 지정했는데 다른 사람이 "나는 3.14보다 더 정밀한 원주율을 쓰고 싶다"는 이유로 3.141592로 바꿀수 있다.

안정성이 테스트 되지 않았으므로 값을 함부로 바꾸는 것은 매우 위험한 일이다.

따라서 상수로 값을 바꾸면 코드가 더 안전해진다.

<hr />

### 상수와 오류

// 상수를 선언한다.

const constant = "변경할 수 없습니다.";

constant = "";

//출력한다.

console.log(constant);

코드를 실행하면 Type Error: Assignment to constant variable 이라는 오류가 발생한다. 상수 값은 바꿀 수 없기 때문에 발생하는 오루이다.

<hr />

변수와 상수를 사용하고 오류가 발생하면 변수(let)으로 교체한다.

-요약

### 1. 자바스크립트 기본 용어

표현식, 문장, 프로그램 : 값을 만들어 내는 간단한 코드를 표현식이라고 하며, 표현식이 모여 문장, 문장이 모여, 문장, 문장이 모여 프로그램이 된다.

키워드 : 자바스크립트를 처음 만들 때 정한 특별한 의미가 있는 단어이다.

식별자 : 이름을 붙일 때 사용하는 단어이다.

주석 : 프로그램의 진행에 전혀 영향을 주지 않고 프로그램 코드를 설명하는 목적으로 사용하는 코드이다.

### 2. 기본적인 출력을 할 때는 console.log() 메소드를 사용한다.

3. 기본 자료형 : 자바스크립트에는 다음 기본 자료형이 있다.

숫자 : 1,2,3,4 같은 숫자를 나타낸다. 기본적인 사칙 연산자와 나머지 연산자를 사용할 수 있다.

문자열 : 문자로 구성된 것을 의미한다. 문자열 연결 연산자를 사용할 수 있다.

불 : 참(true) 또는 거짓(false)을 나타낸다. 불을 생성할 때는 비교 연산자를 사용하고, 불끼리는 논리 연자를 사용할 수 있다.

4. 변수와 상수

변수 : 값을 저장할 목적으로 사용하며, 이후에 변경할 수 있는 값이다.

let <식별자> = <자료>

상수 : 값을 저장할 목적으로 사용하며, 이후에 변경할 수 없는 값이다. 상수를 선언할때는 const 키워드를 사용한다.

const <식별자> = <자료>

### 자료형 변환

-숫자로 변환할 때는 Number() 함수를 사용한다. 숫자로 변환할 수 없는 값을 강제로 숫자로 변환하면 NaN(Not a Number)이 됩니다.

-문자열로 변환할 때는 String() 함수를 사용한다.

-불로 변환할 때는 Boolean() 함수를 사용한다.

-불로 변환할 때 false로 변환되는 것은 O. NaN, ""[빈 문자열], null, undefined이다.


