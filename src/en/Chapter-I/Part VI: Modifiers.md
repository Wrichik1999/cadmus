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
