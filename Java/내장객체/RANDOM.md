### RANDOM
+ Random 클래스는 java.util 패키지에 있으므로 사용시 import가 필요하다.
+ 이때 기본 생성자를 사용해서 생성하면 자동으로 현재 시스템 시간을 seed 값(long형)으로 가지는 Ramdom 객체를 생성한다.
> ```Java
> Random rand = new Random();
> /* 위와 동
> long seed = System.currentTimeMillis();
> Random rand = new Random(seed);
> */
> 
> rand.setSeed(System.currentTimeMillis()); // seed 변경
> ```

### Random 클래스의 난수 발생 메서드
+ boolean nextBoolean() : 균일한 분포의 boolean 형 난수 발생
+ int nextInt() : 균일한 분포의 int 형 난수 발생(int 전 범위에서 난수가 발생)
+ long nextLong() : 균일한 분포의 long형 난수 발생(long 점 범위에서 난수가 발생)
+ int nextInt(int n) : 균일한 분포의 0이상 n 미만의 int형 난수 발생
+ float nextFloat() : 균일한 분포의 0.0이상 1.0 미만의 float형 난수 발생
+ double nextDouble() : 균일한 분포의 0.0이상 1.0 미만의 double형 난수 발생
+ double nextGaussian() : 정규 분포의 난수를 발생(평균이 0이고, 표준편차가 1인 분포)
