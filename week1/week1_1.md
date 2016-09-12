### 메인가기 [go](https://github.com/hannazclass/JavaBasic/blob/master/README.md)
### week1
* [자바의 개념](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_1.md)
* [jdk, eclipse 설치](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_2.md)
* [주석문, 식별자, 예약어](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_3.md)
* [변수, 상수, 문자열](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_4.md)
* [자료형](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_5.md)
* [연산자](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_6.md)
* [제어문](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_7.md)
* [배열](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_8.md)

****
# 1. 자바의 개념
## 1.1. 자바의 특징

### 1. 배우기쉽다
자바는 C++를 기반으로 만들어진 언어입니다. C++에 있는 필요성이 낮고 다루기가 힘든부분을 개발자가 작업하는 영역에서 제거하였기때문에 
언어자체가 단순해져서 배우기가 좀더 쉬워졌다라고 할 수 있습니다.

### 2. 플랫폼 독립성
플랫폼이라는건 운영체제라고 보시면 되는데요.
예를 들어 게임을 하나 개발을 했다고 치면 타언어로 개발하게 되면 운영체제에 맞게 윈도우용 게임, 리눅스용 게임 이렇게 따로 만들어서 운영체제에 직접 설치를 해야 작동이 됩니다. 그래서 프로그램이 운영체제에 의존적인 관계다 라고 할 수있습니다.
타 언어와 달리 자바는 운영체제위에 JVM이라는 가상프로그램이 설치되어 있습니다. 
자바 코드는 운영체제랑 직접적으로 연결되어 있지않고 JVM을 통하여 연결되어있기때문에 우리는 java코드를 한번만 작성하면 되고 JVM만 운영체제에 맞게 설치해주면 어떤 운영체제에서도 실행이 됩니다.
똑같은 게임을 개발하는데 JVM만 운영체제에 맞는 걸로 설치해 주시면 운영체제별로 게임을 따로 개발할 필요가 없어지는 것입니다. 그래서 JAVA는 플랫폼에 독립적이다. 대신 JVM이 플랫폼에 의존적이다 라고 할 수 있습니다.
즉, 가상머신은 프로그램과 운영체제 사이에서 통역사 역할을 한다고 보시면 되겠습니다.

### 3. 객체지향프로그래밍(OOP)
이 객체지향이라는 말은 이해하기 어려운 개념입니다. 실제로 개발자들도 이 개념을 백프로 이해하는 분이 거의 드뭅니다.
간단히 풀어서 얘기하면 객체는 Object 즉 사물입니다. 
객제 지향 프로그래밍 Object Oriented Programming(사물 중심 프로그래밍)
우리 주변을 보면 사물들로 가득하고 그 사물들은 각각의 기능을 수행하고 있습니다.
자바에서는 이 현실세계의 객체개념을 프로그램으로 구현하기 위해 객체지향을 도입했다고 볼 수 있습니다.
즉 프로그램 자체를 객체화 시켜서 기능을 구현하게하고 연관있는 객체들을 모아서 하나의 완성된 프로그램을 구현하자라는 것입니다. 이게 말만 들어서는 솔직히 이해가 잘 안되는게 당연합니다. 그래서 코딩을 해보면서 이해를 할 수 있는 부분입니다.
    
### 4. 가비지컬렉션
C나 C++은 메모리를 할당하거나 다 사용한 메모리를 회수하는 일을 프로그래머가 직접 처리해야하지만 자바는 Garbage Collector가 자동으로 메모리 관리를 해줍니다.

### 5. 멀티스레드
스레드는 프로그램의 수행단위를 말합니다. 스레드인데 멀티가 붙었기 때문에 한 프로그램을 수행하는 단위가 여러개 있다는 뜻입니다. 일을 처리하는데 하나보다는 둘이상 있는게 당연히 수행 속도가 빠르겠죠.

## 1.2. 자바플랫폼
자바 플랫폼이라는 것이 있는데 자바를 실행하기 위해 필요한 프로그램입니다.
    API  - 클래스와 인터페이스들이 묶여져있는 패키지
    JVM 자바가상머신 - 명령어와 레지스터의 집합, 스택, 힙, 메서드 영역으로 구성

## 1.3. 자바 플랫폼의 종류
    SE 일반 데스크탑 PC
    EE 서버용 컴퓨터
    ME 모바일
