# **369 Game**

\#include&lt;stdio.h&gt;



/\*메인함수로 부터 NUM변수를 CALL BY VALUE형식으로 복사한다.

이 함수는 void형식으로 리턴값을 반환하지 않는다. \*/



voidThreeSixNine\(intnum\)

{

//1부터 num까지 for반복문을 돌리면 num번 소스가 반복된다.

for\(intstart = 1; start &lt;=num; start++\)

 {



if\(start / 10 == 3\)

/\*만약 값이 두자리일 경우 start변수를 10으로 나누면 10의 자리 수가 나온다. 만약 이 숫자가 3일경우 먼저 \*을 프린트한다. \*/

 {

 printf\(" \*"\);

//만약 이 숫자가 3일경우 일의 자리가 3인 경우이므로 \*을 프린트한다.

if\(start % 10 == 3\) {

 printf\("\*"\);

 }

//만약 이 숫자가 3일경우 일의 자리가 6인 경우이므로 \*을 프린트한다.

elseif\(start % 10 == 6\) {

 printf\("\*"\);

 }

//만약 이 숫자가 3일경우 일의 자리가 9인 경우이므로 \*을 프린트한다.

elseif\(start % 10 == 9\) {

 printf\("\*"\);

 }

//만약 이 숫자의 끝자리가 0일 경우 \n을 출력하여 개행한다.

elseif\(start % 10 == 0\) {

 printf\("\n"\);

 }

else{

 printf\(""\);

 }

 }

elseif\(start / 10 == 6\)

 {

 printf\(" \*"\);



if\(start % 10 == 3\)

 {

 printf\("\*"\);

 }

elseif\(start % 10 == 6\)

 {

 printf\("\*"\);



 }

elseif\(start % 10 == 9\)

 {

 printf\("\*"\);

 }

elseif\(start % 10 == 0\)

 {

 printf\("\n"\);

 }



else{

 printf\(""\);

 }



 }

elseif\(start / 10 == 9\)

 {

 printf\(" \*"\);



if\(start % 10 == 3\)

 {

 printf\("\*"\);

 }

elseif\(start % 10 == 6\)

 {

 printf\("\*"\);



 }

elseif\(start % 10 == 9\)

 {

 printf\("\*"\);

 }

elseif\(start % 10 == 0\)

 {

 printf\("\n"\);

 }



else{

 printf\(""\);

 }

 }

else{

//한자리 수일때는 변수에 10을 나눈 나머지와 3,6,9를 비교하면서 \*을 출력하였다.

if\(start % 10 == 3\) {

 printf\(" \* "\);

 }

elseif\(start % 10 == 6\)

 {

 printf\(" \* "\);



 }

elseif\(start % 10 == 9\)

 {

 printf\(" \* "\);

 }

elseif\(start % 10 == 0\)

 {

 printf\("%2d ", start\);

 printf\("\n"\);

 }

else{

 printf\("%2d ", start\);

 }

 }

 }

}





intmain\(void\) {





intnum;



 printf\("숫자를 입력해주세요! \n"\);



//scanf를 xocde에서 실행했으나 vs2015에서 scanf\_s를 쓰라는 오류로 고쳤음

 scanf\_s\("%d", &num\);

if\(num &lt;0\)//num이 음수일 경우 입력 숫자가 범위보다 작다는 조건문이 수행된다.

 {

 printf\("입력 숫자가 범위보다 작습니다. \n"\);

 }

elseif\(num &gt; 100\)//num이 100보다 클 경우 범위보다 크다는 조건문이 수행된다.

 {

 printf\("입력 숫자가 범위보다 큽니다. \n"\);

 }

//num이 제한된 숫자영역에 있을 경우를 else문으로 처리하여 ThreeSixNine함수를 호출한다.



else{

printf\("1부터 %d까지 3,6,9 게임을 시작합니다! \n", num\);

 ThreeSixNine\(num\);

 }



return0;



}





















실행결과

![](/assets/homework.PNG)

