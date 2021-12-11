### 배열에서의 equals와 deepEquals
```Java
Integer[] a1 = {1,2,3,4,5};
Integer[] a2 = {1,2,3,4,5};

System.out.println(a1==a2); // false (a1 배열과 a2 배열의 주소값을 비교)
System.out.println(a1.equals(a2)); // false (a1 배열과 a2 배열의 주소값을 비교)
System.out.println(Arrays.equals(a1,a2)); // true (a1 배열 내부의 값과 a2 배열 내부의 값끼리 비교)
System.out.println(Arrays.deepEquals(a1,a2)); // true (a1 배열 가장 내부의 값과 a2 배열 가장 내부의 값끼리 비교)

Integer[][] a1 = {{1,2,3,4,5}, {1,2}};
Integer[][] a2 = {{1,2,3,4,5}, {1,2}};

System.out.println(a1==a2); // false (a1 배열과 a2 배열의 주소값을 비교)
System.out.println(a1.equals(a2)); // false (a1 배열과 a2 배열의 주소값을 비교)
System.out.println(Arrays.equals(a1,a2)); // false (a1 배열 내부의 값과 a2 배열 내부의 값끼리 비교 -> 이때 a1 배열과 a2 배열의 내부의 값은 배열이므로 해당 배열의 주소값끼리 비교하게 된다.)
System.out.println(Arrays.deepEquals(a1,a2)); // true (a1 배열 가장 내부의 값 과 a2 배열 가장 내부의 값끼리 비교)
```
