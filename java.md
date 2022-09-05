
Java 버전별 특징
------------
+ java 8
```
1.Lambda
2.stream
3.interface default method
4.Optional
5.new Date and Time API(LocalDateTime, …)
```

String, StringBuffer, StringBuilder
------------
<!--+ String, StringBuffer, StringBuilder-->
```
String은 불변(immutable)의 속성을 갖는다

String str = "A";
str = str + "B";

위와 같이 실행했을때 두번째 줄이 실행될때 새로운 메모리영역을 가리키게 변경되고 
처음 선언했던 "A"로 값이 할당되어 있던 메모리 영역은 Garbage로 남아있다가 
GC(garbage collection)에 의해 삭제된다. 
String 클래스는 불변하기 때문에 문자열 수정시점에 새로운 String 인스턴스가 생성된다.

값이 변경이 되는 경우 가변(mutable)성을 가지는 StringBuffer 또는 StringBuilder을
사용한다.
StringBuffer, StringBuilder의 차이점은 동기화의 유무로써 StringBuffer는 동기화 지원하여 
멀티쓰레드 환경에서 안전하다는 점(thread-safe)이다. 
동기화로 인해 속도면에서는 StringBuilder가 빠르다
```
