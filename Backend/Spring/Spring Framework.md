마지막 학습 날짜 : 2024.04.25.

</br></br>

# Spring Framework
### Spring Framework는 어떻게 등장하게 되었나


#### 1) Servlet

`Servlet`을 이용하면 일반적인 웹사이트를 만들 때는 어려운 점이 딱히 없었지만 엔터프라이즈 급의 요구사항이 담긴 서비스를 만들기 위해선 `Servlet` 하나만으론 만들기 어려웠다.

</br>

#### 2) EJB
그래서 엔터프라이즈 급의 서비스를 만들 수 있는 `EJB(Enterprise JavaBean)`가 등장.

</br>

하지만 큰 문제점이 여럿 있었는데
1. `RMI`를 기반으로 하는 서버로 상당히 무거움
2. Servlet Container(Tomcat)로는 실행할 수 없고, 별도로 필요했음
3. 최소 2개의 인터페이스, 하나의 클래스, 설정할 수 있는 XML 2개가 필요함 => 배보다 배꼽이 더 크다
  <img src ="https://github.com/fsm12/Dev-Story/assets/74345771/d0620270-1d6c-44cf-8709-6c436177609e" alt="EJB" width="60%">

4. 인터페이스에 따라 코드를 작성해야해서 기존에 작성된 `POJO`를 변경해야 함 

</br>

#### 3) POJO + Framework
스프링의 모태로, `Rod Johnson`이 경량 프레임워크로 엔터프라이즈 애플리케이션을 만들수 있다 소개함.
이후 `POJO`에 경량 프레임워크를 사용하기 시작.
경량 프레임워크 : `Hibernate`, `MyBatis`, `Spring`, ... 

1. 오픈소스 프레임워크 (무료)
2. 개발에 필요한 많은 라이브러리 지원
3. 모든 플랫폼에서 스프링 프레임워크를 사용할 수 있음

