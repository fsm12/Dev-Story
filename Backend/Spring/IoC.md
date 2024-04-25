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

#### IoC를 제대로 설명하면?
IoC는 스프링이 갖는 핵심적인 기능.  
자바의 객체 생성이나 의존관계는 보통 개발자가 만들고 제어했지만, 대부분은 `Servlet Container`에게 넘어갔음. 단, `Servlet`과 `EJB`에 대한 제어권을 제외하곤 개발자가 제어권을 가진다.
스프링에서도 객체의 생성과 생명주기를 관리하는 기능을 담당하는 `Spring Continer`가 있는데 `IoC Container`라 부르기도 한다.

</br></br>
