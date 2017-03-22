# Switch 문

Switch문은 Switch\(  \)괄호 안에 결과 값에 대해 case문으로 경우를 나누어 조건을 실행하는 조건문

Switch\(i%2\)

{

case : 0

printf\("짝수 입니다"\);  

break;

case : 1

printf\("홀수 입니다."\);

break;

default:

printf\("정확히 입력해주세요"\);

break;

}

라는 구조를 가지고 있다.

만약 break;문을 실행하지 않는다면 반복문은 차례대로 수행되어 전체 케이스문을 하나씩 한다.

하지만 break; 문이 있을 시 케이스문을 탈출하여 다음 문장으로 넘어간다.

# Do while 

do while문은 do에 해당하는 바디문장을 먼저 실행하고 그리고 while에 해당하는 반복문을 실행하는 구조

만약  do { printf\("Hello"\)}while\(1\); 을 실행할때 printf문장을 실행하고 do while문을 실행할 때  중괄호가 없을 때 세미콜론을 붙여줘야함

![](/assets/스크린샷 2017-03-22 오후 1.53.55.png)   

# 이중 반복문

while 문 안에 while이 존재할 때 가장 바깥에 있는 반복문이 먼저 수행되고 안에 있는 반복문이 실행되는 구조 

![](/assets/스크린샷 2017-03-22 오후 1.56.40.png) 

이렇게 될때 총 100번 수행된다. 

# For문

for \(i=1;i&lt;=10;i=i++\)

{

if\(i%2 == 0\) printf\("%d \n", i \); 

}





