### Calendar
+ Calendar 클래스는 java.util 패키지에 있으므로 사용 시 import가 필요하다.
+ Calendar 클래스를 이용하면 Date형 날짜의 년, 월, 일을 더하고 뺄 수 있다.
> ```Java
> import java.text.DateFormat;
> import java.text.SimpleDateFormat;
> import java.util.Calendar;
> import java.util.Date;
> 
> public class Example {
>     public static void main(String args[]) {
>         Calendar cal = Calendar.getInstance(); // Calendar 클래스의 인스턴스 생성
>         cal.setTime(new Date()); // 현재 날짜 설정
>         DateFormat df = new SimpleDateFormat("yyyy-MM-dd");
>         System.out.println("current: " + df.format(cal.getTime())); // 설정된 날짜 불러오기
> 
>         cal.add(Calendar.MONTH, 2); // 설정된 날짜 수정하기
>         cal.add(Calendar.DATE, -3); // 설정된 날짜 수정하기
>         // cal.add(Calendar.YEAR, 1);
>         // cal.add(Calendar.HOUR_OF_DAY , 1);
>         // cal.add(Calendar.MINUTE, 20);
>         // cal.add(Calendar.SECOND, 10);
>         System.out.println("after: " + df.format(cal.getTime())); // 설정된 날짜 불러오기
>     }
> }
> ```
