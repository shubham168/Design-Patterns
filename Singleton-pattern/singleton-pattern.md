# Singleton Pattern

`Singleton is a creational design pattern that lets you ensure that a class has only one instance, while providing a global access point to this instance.`

Consider example of Database instance. We would need only one instance of database which is shared by all parts of the application. 

All implementations of the Singleton have these two steps in common:

Make the default constructor private, to prevent other objects from using the new operator with the Singleton class.
Create a static creation method that acts as a constructor. Under the hood, this method calls the private constructor to create an object and saves it in a static field. All following calls to this method return the cached object.

![Singleton](./Singleton-pattern.png)