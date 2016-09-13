### 메인가기 [go](https://github.com/hannazclass/JavaBasic/blob/master/README.md)
### week1
* [자바의 개념](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_1.md)
* [jdk, eclipse 설치](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_2.md)
* [자바개발순서, 주석문, 식별자, 예약어](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_3.md)
* [변수, 상수, 문자열](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_4.md)
* [자료형](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_5.md)
* [연산자](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_6.md)
* [제어문](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_7.md)
* [배열](https://github.com/hannazclass/JavaBasic/blob/master/week1/week1_8.md)

****
# 3. 자바개발순서, 주석문, 식별자, 예약어

## 3.1. 자바개발순서
코드를 작성=>코드 컴파일=>JVM으로 실행

```
Java코드는 사람이 인식할 수 있도록 작성되어있는데 이는 컴퓨터가 인식을 할 수 없습니다.
javac.exe자바컴파일은 자바 가상머신이 인식할 수 있도록 java코드를 기계어로 바꾸어 줍니다.
기계어로 바꾸다(=>바이트코드로 바꾸다)
실제 가상머신에 올리는 파일은 .java가 아닌 .class입니다.
java.exe 런처(발사대), 실질적인 프로그램의 실행

명령프롬프트에서 java.exe(자바런처)와 javac.exe(자바컴파일러)를 통하여 실행할 수 있습니다. 
명령프롬프트는 자바코드를 실행하게 되면 현재 디렉토리에서 실행파일을 찾게되는데 
window에 등록된 path를 참조에서 path에 등록되어있는 디렉토리 위치에서도 실행파일을 찾게 됩니다.
우리는 환경변수 설정에서 path에 자바가 설치되어있는 경로를 등록해놓았기 때문에 java, javac는 어디곳에서도 실행할 수 있습니다.
그러나 우리가 작성한 코드를 실행하기 위해서는 작성한 코드가 있는 경로로 이동하여 
그 경로상에서 java 파일명으로 실행해야 결과값이 출력이 됩니다.
(환경변수는 java를 실행하기위한 설정이고 작성한 코드의 실행과는 관련이 없습니다.)
```

## 3.2. HelloWorld출력하기
  +실습)HelloWorld.java
```
그럼 간단하게 코드를 작성해보겠습니다.
우선 C드라이브에 작업폴더를 만들어줍니다.
폴더명 : JavaClass

두가지 방법을 이용해서 HelloWorld라는 단어를 출력해보겠습니다.
```
### 콘솔(cmd)에서 출력
```
첫번째는 cmd창을 이용해서 출력을 해보겠습니다.
작업폴더로 이동하셔서 메모장을 여시고 HelloWorld.java 확장자로 저장해주시고 코드작성을 합니다.
이때 파일명은 대소문자를 구별하니 잘 입력해야합니다.

경로를 우선 작업폴더로 변경해야합니다. 
windows+R 키를 누르고 'cmd'를 입력하면 콘솔창이 하나 뜹니다.
c드라이브 최상위 경로로 변경해봅시다.
cd..를 하게 되면 한단계 위의 경로로 이동하게 됩니다.
* 주의! '>' 는 경로를 생략해서 표기한 것으로 입력하면 안됩니다.
>cd..
그리고 c드라이브 최상위 경로로 왔을때 우리가 새로 생성한 폴더로 이동합시다.
>cd JavaClass
```
<img src="/images/3_1.JPG" width="" height=""></img>

```
여기에서 이제 코드를 컴파일 시켜 보겠습니다.
컴파일은 javac(java compiler)라는 명령어를 사용하면됩니다.
Javac HelloWorld.java라고 치시고 dir를 입력해서 디렉토리를 확인해보면 아까는 없었던 HelloWorld.class가 생성된 것을 볼 수 있습니다.

이제 우리가 만든 자바파일을 출력해보겠습니다. 
Java HelloWorld
=>메인 메소드가 없어서 에러가 발생함.

똑같은 과정을 이클립스에서 코드를 작성해서 실행해보도록 하겠습니다.
일단 우리가 코드를 작성하기 위해서는 프로젝트를 생성해야합니다.
javaProject를 눌러서 생성하시고 이름을 first로 주겠습니다.
src디렉토리에서 =>new-class=>HelloWorld라고 만들어줍니다.
Main을 체크하시면 자동으로 메인 메소드가 생성됩니다.
코드를 작성하고 저장을 누르면 자동으로 컴파일이 됩니다.
bin디렉토리안에 클래스가 만들어집니다.
코드를 실행하는 방법은 파일을 선택하시고 rus as => java application(ctrl+f11)을 실행하시면 됩니다.
```
