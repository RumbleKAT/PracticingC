unsigned Char %u - unsigned 자료형은 %u를 사용한다.

signed char - %c 

아스키코드키의 0 ~ 32는 표현되지 않는다.

내부적으로 숫자는 50번대 문자는 60 번대 이런식으로 저장됨

char ch 

ch = 65;

ch = 'a'는 동일하다.

UNICODE - 아스키로 전세계 코드가 입력이 안되자 유니코드를 사용함

문자를 입력할 때는 SPACE를 문자로 들어가기 때문에 빈칸을 두면 안됨

enter키도 문자이다. 

그럴때 fllush함수를 사용하면 stdin을 개끗하게 없애줌 

stream을 비워줘서 새로 시작할수 잇도록 할 수 있다. 

