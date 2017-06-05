# 구조체 Struct

구조체는 하나의 자료형이다. c나 c++의 경우 구조체가 존재하고 c\#이나 자바는 구조체가 없다.

아직 객체지향이 되기 전에 언어에서 많이 쓰이는 것으로  여러가지 복잡한 변수들을 구조체로 하나로 묶어서 쓸 수 있어서 간단하게 쓸 수 있다.

구조체 안에는 여러 자료형과 배열까지 넣을 수 있다. 또 구조체를 배열로 선언도 가능하다.



```
struct student{
    int x;
    int y;
} // 이렇게 선언을 한다.
```

주로 이런 형식으로 사용된다. 

# 포인터 변수 

struct  point pixel;

struct point \* p = &pixel;

\(\*p\).x = 10;

p -&gt; x = 10; 으로 간추릴 수 있다. 

이렇게 쓰는 방법은 나도 그렇게 써본적이 없다. \*p를 하는 이유는 포인터 변수인 p가 x보다 우선순위를 가져야하기 때문이다. 

특히 call by reference로 받을 때 많이 사용된다.

# Call By Value

```
void printCallbyValue(struct student s){
    //Call by value형식으로 다시 저장되는 형태 
   printf("%d %20s %d \n", s.id, s.name , s.grade);
}
```

# Call By Reference

```
void printCallbyValue(struct student *p){
    printf("%d %20s %d \n", p->id, p->name , p->grade);
    
}
```



