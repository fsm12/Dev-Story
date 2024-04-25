마지막 학습 날짜 : 2024.04.25.

</br></br>

# Container
#### Container는 Tomcat이었다?
`Servlet`을 할 때 `Tomcat`이 `Servlet Container` 역할을 했었다.

`Servlet`은 우리가 만든 것이 아니었고, 이 친구의 `LifeCycle`은 `WAS`가 담당해서 관리했음.  
즉, `LifeCycle`을 관리해주는 것을 `Container`라 한다.

그렇기 때문에 `Spring`도 `Container`라 할 수 있다.

</br>

#### Container란
객체의 생성과 사용, 소멸에 해당하는 라이프사이클을 관리해줌
또한, 애플리케이션 사용에 필요한 주요 기능들을 제공함

정리하면, 

1. 라이프사이클 관리
2. Dependency 객체 제공
3. Thread 관리
4. 기타 애플리케이션 실행에 필요한 환경

들을 관리한다.

Container를 이용하면 
- 비즈니스 로직 외에 부가적인 기능들에 대해서 독립적으로 관리할 수 있다.
- 서비스 `look up`이나 `Configuration`에 대해 일관성을 가질 수 있다.
- 서비스 객체를 이용하기 위해 `Factory`나 `Singleton`패턴을 직접 구현하지 않아도 된다.

</br>

#### Spring DI Container는?

`Spring DI Container`가 관리하는 객체를 `Bean`이라 하는데, 이 Bean들의 생명주기를 관리한다는 뜻으로 `BeanFactory`라 한다.

`BeanFactory` : 인터페이스로 Bean을 등록, 생성, 조회, 반환 관리를 하며 `getBean()`메소드가 정의되어 있음.

`ApplicationContext` : `BeanFactory` 인터페이스의 하위 인터페이스로 각종 부가서비스를 추가로 제공한다.





