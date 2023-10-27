# A. Concept of Object-Oriented Programming
## Definition
An object can be described as entities that are clearly defined.
For example: students, cars, desks.

Objects in programming language must have method, property, type, and identity. 

All data and methods are wrapped in classes and objects

OOP provides us the ability to change these objects

Advantages of OOP
1. Allows the use of real-world modeling
2. Support the reuse of existing code
3. Provide flexibility in modifying existing applications
4. Assist with ease of maintenance of existing code

## Four Pillars of Object-Oriented Programming
### 1. Concept of Abstraction
The ability of a program to bypass aspects of the information processed by it, namely the ability to focus on the core.
### 2. Concept of Encapsulation
Details of the implementation shown in the summary are hidden from the user

User objects can not change the situation in a way that is not feasible, only the method by which objects are given permission to access the situation

### 3. Concept of Inheritance
Inheritance of properties from another class, so having the characteristic or nature of the class

Each class could only have one superclass, on the other hand, the parent class could have limitless subclasses.

### 4. Concept of Polymorphism
One method has many implementations of behavior

The ability of an object to become a variety of forms depending on the situation

## Defining Class for Object
OOP involves programming using objects

Class is the template of the object, which defines the properties of the objects, and provides constructors to create objects and methods to manipulate objects

A class is also a type of data, that can be used to express the object referenced by the variable

An object of the class has
1. Unique identity
2. State - data field, properties
3. Behaviour - one or a set of methods or functions

```
Circle object = new Circle();
System.out.println("Area: " + object.getArea());
```

## Constructors
Constructors are a special kind of method. They have three peculiarities:
1. The constructor must have the same name as the class itself
2. Constructor does not have a return type (Not even void)
3. Constructors are invoked using the new operator

```
Circle obj = new Circle();
```

## Access Modifiers
1. Private: hide the class members so they are not accessible from outside the class
2. Protected: allows members of the class to be accessed by the class or its derivatives int the same packages
3. Public: allows members of the class to be accessed by other classes
4. Package: used to organize classes. if the class was created without using the package statement, the class will be placed in the default package.

| Access Modifiers  | Same Class | Same Package | Subclass | Other Packages | 
| ----------------- | ---------- | ------------ | -------- | -------------- |
| Public            | Y          | Y            | Y        | Y              |
| Protected         | Y          | Y            | Y        | N              |
| No access modifier| Y          | Y            | N        | N              |
| Private           | Y          | N            | N        | N              |

# B. Inheritance
## Definition
Inheritance can be defined as the process where one object acquires the properties of another with keyword extends and implements.

## Superclass and Subclass
The class that received from another class is called the subclass

Superclass is also called parent class

Constructor is not a member so it is not inherited by subclasses

A subclass inherited all rights to access both public and protected  data from its superclass, regardless of where the package from subclass is located

If the subclass and parent class are on the same package it will also inherit the package-private member from its superclass

Keyword extends is used to access the parent class

Multiple inheritance from parent classes is not allowed

## Super Keyword
Keyword this refers to an object in the class

The keyword super refers to superclass from its called class

2 ways of using super:
1. Call superclass constructor
   super() or super(parameter)
2. Call superclass method
   super.method(parameter)

```
public void printRadius(){
  System.out.println("Radius: " + super.getRadius);
}
```

## Advantages of Inheritance
When a method is declared in a superclass, that behavior is automatically inherited by the subclass

Could only encode the method once and the method could be used by all subclass

A subclass only need to implement difference between itself and its parents

























