# Object Oriented Principles

## Inheritance

Inheritance enables you to create new classes that reuse, extend, and modify the behavior defined in other classes. The class whose members are inherited is called the base class, and the class that inherits those members is called the derived class.

## Abstract

An abstract class cannot be instantiated. The purpose of an abstract class is to provide a common definition of a base class that multiple derived classes can share.

## Polymorphism

Polymorphism is a Greek word that means "many-shaped" and it has two distinct aspects:

1. At run time, objects of a derived class may be treated as objects of a base class in places.
2. Base classes may define and implement virtual methods, and derived classes can override them, which means they provide their own definition and implementation.

## Object-oriented

C# is an object-oriented programming language. The four basic principles of object-oriented programming are:

1. Abstraction: You used abstraction when you defined classes for each of the different account types. Those classes described the behavior for that type of account.
2. Encapsulation: You used encapsulation when you kept many details private in each class.
3. Inheritance: You used inheritance when you leveraged the implementation already created in the `BankAccount` class to save code.
4. Polymorphism: You used polymorphism when you created virtual methods that derived classes could override to create specific behavior for that account type.

These techniques are commonly used in Object-Oriented programming.
