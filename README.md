### 🔹 JDK vs JRE vs JVM
### 🔹 primitive types?
### 🔹 С чего начинается запуск программы на java
### 🔹 Какими значениями инициализируются переменные по умолчанию?
### 🔹 String - primitive type?
    String s1 = "String";
    String s2 = new String("String");
    s1 == s2   // ??
    s1.equals(s2) // ??
<details><summary>Answer</summary>

      false
      true
</details>

### 🔹 Как добавить строку в пулл?
<details><summary>Answer</summary>

      метод "smthng".intern()
</details>

### 🔹 abstract. Can abstract class not have absctract methods and vice versa.
### 🔹 final. What is it used with
### 🔹 static.
### 🔹 Override vs Overload.
### 🔹 Can we Overload static methods in Java?
<details><summary>Answer</summary>

  ```
  Yes
  ```
</details>

### 🔹 Can we Override static methods in Java
<details><summary>Answer</summary>

  ```
  No
  ```
</details>

### 🔹 What is a static block?
    В каком порядке выполняются блоки в классе? static / non-static
### 🔹 What is a static class?
<details><summary>Answer</summary>

  ```
  In Java only nested classes are allowed to be declared as static, a top level class cannot be declared as static.
  ```
</details>
  
### 🔹 OOP основные принципы.

Используйте следующее вместе с наследованием

    Делегация — перепоручение задачи от внешнего объекта внутреннему;
    Композиция — включение объектом-контейнером объекта-содержимого и управление его поведением; последний не может существовать вне первого;
    Агрегация — включение объектом-контейнером ссылки на объект-содержимое; при уничтожении первого последний продолжает существование.

### 🔹 Inner vs nested classes
<details><summary>Answer</summary>
  
      A nested class is a static class defined inside another class. It is not bound to a specific instance of the outer class. 
      An inner class is a non-static class defined inside another class. it is bound to a specific instance of the outer class.
</details>

### 🔹 Can abstract method be static?
<details><summary>Answer</summary>
  
      No.
</details>
  
### 🔹 Есть ли доступ у static метода к nonStatic полям и наоборот?
### 🔹 this keyword.
### 🔹 super keyword.
### 🔹 Output?    
``` java
public class Myclass {
  Myclass() {
        System.out.println("CONSTRUCTOR");
  }

  static void m1() {
        System.out.println("STATIC METHOD");
  }

  void m2(){
        System.out.println("INSTANCE METHOD");
  }

  static {
        System.out.println("STATIC BLOCK");
  }

  {
        System.out.println("INSTANCE BLOCK");
  }

  public static void main(String[] args) {
      Myclass obj = new Myclass();
      m1();
      obj.m2();
     }
}
```
<details><summary>Answer</summary>
  
      STATIC BLOCK, INSTANCE BLOCK, CONSTRUCTOR, STATIC METHOD, INSTANCE METHOD.
</details>

### 🔹 interfaces.
    Can interface have methods with body, if yes what methods.
### 🔹 lambdas. What is it + examples.
<details><summary>Answer</summary>
  
```
Runnable 	→
BiConsumer(T, U) 	T, U →
BiFunction(T, U, R) 	T, U → R
BinaryOperator 	T, T → R
BiPredicate<T, U> 	T, U → boolean
BooleanSupplier 	→ boolean
Consumer 	T →
DoubleBinaryOperator 	double, double → double
DoubleConsumer 	double →
DoubleFunction 	double → R
DoublePredicate 	double → boolean
DoubleSupplier 	boolean →
DoubleToIntFunction 	double → int
DoubleToLongFunction 	double → long
DoubleUnaryOperator 	double → double
Function<T, R> 	T → R
IntBinaryOperator 	int → int
IntConsumer 	int →
IntFunction 	int → R
IntPredicate 	int → boolean
IntSupplier 	→ int
IntToDoubleFunction 	int → double
IntToLongFunction 	int → long
IntUnaryOperator 	int → int
LongBinaryOperator 	long, long → long
LongConsumer 	long →
LongFunction 	long → R
LongPredicate 	long → boolean
LongSupplier 	→ long
LongToDoubleFunction 	long → double
LongToIntFunction 	long → int
LongUnaryOperator 	long → long
ObjDoubleConsumer 	T, double →
ObjIntConsumer 	T, int →
ObjLongConsumer 	T, long →
Predicate 	T → boolean
Supplier 	→ T
ToDoubleBiFunction<T, U> 	T, U → double
ToDoubleFunction 	T → double
ToIntBiFunction<T, U> 	T, U → int
ToIntFunction 	T → int
ToLongBiFunction<T, U> 	T, U → long
ToLongFunction 	T → long
UnaryOperator 	T → T
```
</details>


### 🔹 Class Object и его методы.
<details><summary>Answer</summary>
  
  ```
    tostring() method
    hashCode() method
    equals(Object obj) method
    finalize() method
    getClass() method
    clone() method
    wait(), notify() notifyAll() methods
```
</details>
  
### 🔹 Optional class.
### 🔹 Stream API. Типы методов стримов и их примеры.
 [Stream API](https://docs.oracle.com/javase/8/docs/api/java/util/stream/Stream.html)
### 🔹 Exceptions in Java.
    Иерархия исключений?
    Отличия checked и unchecked.
<details><summary>Answer</summary>
  
![image](https://github.com/Vlarfich/JavaQuestions/assets/106491695/cdec1a3a-32a6-4caf-a950-6f5069f3982d)
</details>

### 🔹 How can we _throw_ an exception?
### 🔹 How can we _catch_ an exception?
### 🔹 Может ли быть try without catch. // только если с finally
### 🔹 Can we catch multiple types of exceptions?
### 🔹 Надо ли обрабатывать unchecked?
### 🔹 try catch finally.
```java
try {
  throw new Exception();
  return 1;
}
catch (Exception e) {
  return 2;
}
finally {
  return 3
}
```
<details><summary>Answer</summary>

    3
</details>

### 🔹 try with resources.
    Closable
    AutoClosable
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
### 🔹
