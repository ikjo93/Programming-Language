### Integer.bitCount()
+ () 안 수를 이진수로 변환했을 때 1의 개수를 반환함
> ```Java
> int a = Integer.bitCount(4); // 4는 이진수로 변환하면 100이므로 a는 1
> int b = Integer.bitCount(10); // 10는 이진수로 변환하면 1010이므로 b는 2
> ```

### Integer.MAX_VALUE & Integer.MIN_VALUE
+ Integer 클래스의 MAX_VALUE와 MIN_VALUE를 사용하면 정수의 최대값(2,147,483,647)과 최소값(-2,147,483,648)을 바로 출력할 수 있다.
  + Int 정수의 범위는 -2,147,483,648 ~ 2,147,483,647
  + ※ Integer 클래스 외 Long, Short 등의 클래스도 같은 메소드를 제공한다.
