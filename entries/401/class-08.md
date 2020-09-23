# Object Oriented Design

> S O L I D

S.O.L.I.D stands for:

S - Single-responsiblity principle
O - Open-closed principle
L - Liskov substitution principle
I - Interface segregation principle
D - Dependency Inversion Principle

> A class should have one and only one reason to change, meaning that a class should have only one job

## Open-Closed Principle

> Objects or entities should be open for extension, but closed for modification

- a class should be easily extendable without modifying the class itself

Coding to an interface is an integral part of **S.O.L.I.D**


## Liskov Substitution Principle

> Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a subtype of T.

- every subclass/derived class should be substitutable for their base/parent class.

## Interface segregation principle

> A client should never be forced to implement an interface that it doesn’t use or clients shouldn’t be forced to depend on methods they do not use.

## Dependency Inversion principle

> Entities must depend on abstractions not on concretions. It states that the high level module must not depend on the low level module, but they should depend on abstractions.

