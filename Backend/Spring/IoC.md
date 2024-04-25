마지막 학습 날짜 : 2024.04.25.

</br></br>

# IoC (Inversion Of Control) : 제어의 역행
#### IoC는 새로운 개념이 아님
스프링을 써보지 않아도 IoC를 경험해볼 수 있는데 바로 `DB Connection Pool`을 사용할 때이다. 

</br>

보통 우리는 A 클래스를 사용하다가 B 클래스가 필요하면
``` java
B b = new B();
```
방식으로 호출했겠지만, `DB Connection Pool`에서는 미리 만들어놓고 필요할 때 가져다 쓰는 방식을 채택했다.
이것이 `IoC`의 기본.

</br></br>
