Part VI: Modifiers
=========================

The variable modifiers are:
  * public
  * private
  * protected
  * final
  * abstract
  * static
  * native
  * const

Public
------
Public is the default modifier. A `public` variable can be accessed by an class in any package.
```java
public int = 0;
public class Xyz{}
public int method(String args){
  return 0;
}
```

Private
-------
A `private` variable or method can only be accessed by the class that it is defined in.
```java
class Foo{
  public int foo = 0; //Can be accessed by any class in any package
  private String foobar = "FOOBAR"; //Can only be accessed by an instance of the Foo class
}
```

Protected
---------
A `protected` variable can only be accessed by a class in the same package.
```java
package foo;
class Bar{
  protected int = 0; // Can only be accessed by classes in the foo package
  public void foobar(){}
}
```

Final
-----
A `final` variable cannot be changed. It is `const`ant. It is the replacement of the `const` modifier. A `final` class cannot be ionherited.
```java
final class Foo{
  final int bar = 1; // Cannot be changed
  public String foobar = "foobar"; // Can be changed
}
```

Abstract
--------
An `abstract` variable can only be in an abstract class. Abstract methods have to overriden as in they have to be rewritten if the class is tho extend an abstract class. Non-abstract variables can be declared in an abstract class as well. An abstract class can not be instantiated much like the System class.
```java
abstract class Hello{
  abstract int world = 0
}
```

Static
------

A `static` variable can be accessed without having to make an instance of the class. The same applies for methods and even static nested classes. A static import allows to use static items without having to name their original class.
```java
static class Hello{
    static int num = 0;
    static void prints(String str){
        System.out.println(str);
    }
}
// Now we can call Hello.num or Hello.prints without having to make ans instance of the Hello class
```

Native
------
A `native` method is written in a different language to Java.
