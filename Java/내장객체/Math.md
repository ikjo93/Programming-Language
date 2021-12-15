### Math
+ Math 클래스는 java.lang 패키지에 있으므로 별도 import가 필요 없다.
+ Math의 변수나 메서드는 일회성으로 사용하는 경우가 많아 생성자가 없다.
+ 이때 생성자란 객체를 생성할 때 자동으로 호출되는 것으로 기본적인 변수를 선언하거나 함수를 호출된다.
+ 또한 정적(static) 속성 및 메서드이므로 객체를 생성하지 않고 바로 클래스명으로 접근하여 사용할 수 있다.

### Math의 속성과 메서드
+ Math.PI : 3.141592653589793
+ Math.pow(10, 4) : 10의 4 제곱근(10000)
+ Math.floor() : 소수점 내림(소수점 이하 숫자 모두 0으로 변환)
+ Math.ceil() : 소수점 올림(소수점 이하 숫자 존재 시 모두 0으로 변환 후 일의 자리 숫자 + 1)
+ Math.round(실수) : 가장 가까운 정수(반올림) ※ Math.round() 함수는 소수점 아래가 0일 경우 절삭하여 출력한다.
>  + (응용) 소수점 n번째 자리까지 표현하기
> ```Java
> double pie = 3.14159265358979;
> System.out.println(Math.round(pie)); // 3
> System.out.println(Math.round(pie*100)/100.0); // 3.14
> System.out.println(Math.round(pie*1000)/1000.0); // 3.142
> double money = 5000.000;
> System.out.println(Math.round(money*1000)/1000); // 5000
> System.out.println(String.format("%.3f", money)); // 5000.000
> ```
+ Math.random() : 0.0 이상, 1.0 미만의 double 값의 난수를 균일한 분포로 반환하며 0 ~ 9 사이의 정수형 난수를 만들고 싶다면 double 형 난수에 10을 곱한 후 정수로 캐스팅 하면 된다. 또는 알파벳을 랜덤하게 발생시킬 수도 있다.
> ```Java
> for(int i = 0; i < 100; i++) {
>   double dValue = Math.random();
>   int iValue = (int)(dValue * 10);
>   System.out.println(iValue);
> }
> 
> for(int i = 0; i < 100; i++) {
>     double dValue = Math.random();
>     // 대문자
>     char cValue = (char)((dValue * 26) + 65);
>     // 소문자
>     char cValue = (char)((dValue * 26) + 97); 
>     System.out.println(cValue);
> }
> ```
