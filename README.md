# 개요
> 스프링 프레임워크(Spring Framework) 관련 공부 내용을 정리
# 1. Spring Framework
Spring Framework는 JAVA 기반으로 Web Application 개발을 위해 DI, AOP, MVC, JDBC 등을 주요기능으로 제공한다.
  
* DI(Dependency Injection)
  * 주입기능
  * 어떤 기능을 필요할 때마다 주입하여 그 기능을 사용
* AOP(Aspect-Oriented Programming)
  * 관점지향 프로그래밍
  * 공통된 부분을 뽑아내서 주요 부분만 작업하고 공통된 부분은 별도로 존재하게 하여 필요에 의해 뗏다 붙였다 하는 기능
* MVC(Model-View-Controller)
  * 소스 코드를 분리하여 구조화시키는 방법
* JDBC(JAVA DataBase Connectivity)
  * JAVA를 이용하여 Database와 통신하는 방법
    
# 2. Spring Framework Module
Spring Framework에서 제공하고 있는 모듈을 사용하기 위해서는 모듈에 대한 의존설정을 개발 프로젝트의 XML파일 등을 이용하여 명시하면 프로젝트에서 해당 모듈을 자동으로 다운받으므로 개발자가 import 하지 않아도 된다.
* Spring-Core
  * DI와 IoC(Inversion of Control)을 제공
* Spring-AOP
* Spring-JDBC
* Spring-TX
* Spring-WebMVC
  
# 3. Spring Framework Container(IoC)
Spring Framework에서 객체를 생성하고 조립하는 컨테이너(Container)로 이를 통해 생성된 객체를 빈(Bean)이라고 한다.
* XML파일 등을 이용하여 객체 생성 & 속성데이터 작성
* 위에 생성된 객체(Bean)를 스프링 컨테이너가 담고 있음
* JAVA파일의 스프링 컨테이너에서 필요할 때마다 꺼내서 사용하여 Application을 구현
