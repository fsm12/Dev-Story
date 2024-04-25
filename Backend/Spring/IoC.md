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

객체간의 관계를 느슨하게 연결(Loose Coupling)할 수 있도록 `IoC`의 구현방법 중 하나인 `DI`를 이용함

</br></br>

#### IoC 의 유형은?
<img src = "https://github.com/fsm12/Dev-Story/assets/74345771/89826423-8904-411d-91f0-51ddafb17f97" alt="" width="50%">

`IoC`는 크게 나누면 `Dependency Lookup`과 `Dependency Injection`으로 나눌 수 있음

</br>

#### `Dependency Lookup`
컨테이너가 `lookup context`를 통해 필요한 `Resource`나 `Object`를 얻는 방식

DBCP(DBMS Connection Pooling)에서 JNDI를 미리 만들어놓고 찾아서 썼음  
이 때, `Lookup`한 `Object`를 필요한 타입으로 형변환을 해 줘야 했다.

</br>

#### `Dependency Injection`
`Object`에 `lookup` 코드를 사용하지 않고 컨테이너가 직접 의존 구조를 `Object`에 설정할 수 있도록 지정해 주는 방식  

`필드주입 / Setter 주입 / 생성자 주입 / 일반 메서드 주입` 으로 나뉜다.

</br></br>






