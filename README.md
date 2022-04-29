# 템플릿 리터럴(Template Literal)

ES6부터 새로 도입된 문자열 표기법이다.

문자열 생성시 따옴표 대신, 백틱(`)을 사용한다.

var str_01 = `hello world`;
 


# 템플릿 리터럴의 기능

1. 줄바꿈(개행: Multi-line strings) 

▶︎ 백틱(`)으로 템플릿 리터럴을 사용하면, 줄바꿈 등을 쉽게 표현할 수 있다.

var str_01 = `
Hi!
    It's me!
             JavaScript!
So Cool!`;

▶︎ 기존 따옴표 방식에서는 줄바꿈이 허용되지 않았기 때문에,

▶︎ 백슬러시(\)로 시작하는 이스케이프 시퀀스를 사용해야 했다.

var str_01 = "Hi! \n\t It's me! \n\t\t\t JavaScript! \n So Cool!";
* \n은 개행(Line Feed), \t는 탭(수평)을 의미하는 이스케이프 시퀀스

 
2. 표현식 삽입(Expression interpolation)

▶︎ ${ } 사이에 변수나 연산 등을 삽입할 수 있게 되었다.

var name = `사과`
var price = 100
var num = 5;

console.log(`${name}의 구매가는 ${price * num}원 입니다.`)
 

<실행 결과>


* ${ } 의 결과는 문자열로 자동 변환됨.


▶︎ 기존의 따옴표 방식에서는, + 연산자로 여러번 이어 붙여야 했다.

var name = `사과`
var price = 100
var num = 5;

console.log(name + "의 구매가는 " + (price * num) + "원 입니다");
 


▶︎ 아래 코드처럼 사용도 가능하다. 

console.log(`${5+10} 입니다`)  // 15 입니다
연산결과는 문자열로 자동 변환되어 사용된다.


출처: https://curryyou.tistory.com/185 [카레유]
