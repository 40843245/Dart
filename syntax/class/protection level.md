# protection level
## review
Protection level in class give an ability to control the access of member in class. 

There are four common protection levels in class

+ `public`
+ `private`
+ `protected`
+ `internal`

## abstract
In Dart, there are no modifiers 

+ `public`
+ `private`
+ `protected`
+ `internal`

But don't worry, we can define the protection level.

For private members, they MUST start with underscore `_`.

For public members, they MUST NOT start with underscore and thus, MUST start with alphabet.

## example
```
class Car{
  int _id; // private member
  String name; //public member

}
```
