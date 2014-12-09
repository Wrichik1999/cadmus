Part VI: Modifiers
=========================

The variable modifiers are:
  * public
  * private
  * protected
  * final
  * abstract
  * static
  * synchronised
  * volatile
  * native
  * const
  * transient

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
