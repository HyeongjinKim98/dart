# Dart


#### 1) nullable , non-nullable
- 변수형 뒤에 " ? " 를 붙이면 nullable
- nullable 변수 뒤에 !를 붙임 => nullable,but not null

````
String name1 = 'non_nullable';
print(name1);
  
String? name2= 'nullable';
print(name2!);
  
name2 = null;
print(name2);
````

#### 2) final, const
- 한번 선언 하면 값을 변경할 수 없음
- 자료형 선언(var) 또한 생략 가능!

````
final String name3 = 'final';
print(name3);
  
const String name4 = 'const';
print(name4);
````
````
final name5= 'final';
print(name5);
  
const name6 = 'const';
print(name6);
````

- final : build time 필요x
- const : build time 필요o
````
final DateTime now1 = DateTime.now(); // 가능

const DateTime now2 = DateTime.now(); // 불가능
````
#### 3) null operator
````
double? number = 4.0;

number ?? = 3.0;
print(number);

number = null;

number ?? = 3.0;
print(number);
````
- "??=" null일 때 변수값을 변경하는 operator
