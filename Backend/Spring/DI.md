마지막 학습 날짜 : 2024.04.25.

# DI (Dependency Injection) : 의존성 주입
#### DI를 한 문장으로 요약하면?
> 너 없이 못살아

예를들어 `A 클래스`에서 `B 클래스`를 `b`로 선언한 뒤 b의 메소드인 `action()`을 호출했다고 생각해보자.
``` java
class A{
  B b = new B();
  b.action();
}
```
여기서 A는 B를 선언하지 않고는 `b.action()`을 실행할 수 없다.  

그런데 `Spring Boot`는 직접적으로 객체 생성을 하지 않음.
그래서 B라는 객체를 만들고 가져다 쓰는(IoC)가 아닌 주입(DI)을 시킴.

따라서 Spring 객체인 `Bean`에서 `new`가 사라지게 됨. B라는 아이를 어디서든지 찾아올 수 있게 되는 것.


#### DI를 그러면 어떻게 설정해?
크게 3가지 방법이 있다.

> 1. XML
> 2. Annotation
> 3. XML과 Annotation을 합쳐서 Java Configuration이라는 java file
