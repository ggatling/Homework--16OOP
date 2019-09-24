---
title: OOP Review
type: Homework
duration: "1:00"
creator:
    name: Charlie Drews
---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) OOP Review

## Requirements

Respond to the following questions based on what we've learned (and maybe what we haven't covered yet).

---

## Questions

1. What's the difference between **member variables** (also called **instance variables**) and **class variables** (with the `static` keyword)? Which can be accessed without creating an instance of the class?
- Instance variables use the keyword new and created when the object is created and destroyed when the object is destroyed and must be referenced more than once. Class variables have the keyword static and declared public and are only referenced once within the class and are stored in static memory.
when the program started and destroyed when the program stops.
2. Does it make sense to write **getter** and **setter** methods for a `public` member variable? What about `private` variables?
- It only makes sense to use getter and setter methods for a private variable because that that is the only what you can access or modify it outside of the class.
3. What are some benefits of making member variables `private`?
- Private provides data security and better control over your variables because they can only be accessed by getter and setter methods.
4. If Class A extends Class B, which is the superclass and which is the subclass? Which would you call the parent, and which would you call the child?
- Class B is the superclass and parent Class A is the subclass and child.
5. What does it mean for a class to **inherit** methods or variables (or both) from its parent class?
- Inherit essentially means that we want to reuse certain code for a class that has similar attributes.
6. Consider the following code, where the `Refrigerator` class extends the `Appliance` class, and `getTemperature()` is a method in `Refrigerator`, but **not** in `Appliance`:

    ```
    Appliance myAppliance = new Refrigerator();
    double temperature = myAppliance.getTemperature();
    ```

   Why will this call to `getTemperature()` cause an error? How will **casting** help solve this issue?

   - Since temperature is not a variable in Appliance, we are unable to assign the method getTemperature to the temperature variable in Refrigerator.
   - Casting would give us more funtionality to the Appliance object.
7. In a normal class (also called a **concrete** class), do you need to **implement** all the methods, or can you simply **declare** some? What about in an `abstract` class?
- In a normal class you dont need to implement all the methods and some can just be declared while in an abstract class you force implementation onto the classes that extend from it.
8. What about an `interface`? Can you implement any methods in an `interface`? Can you declare methods in an `interface`?
- You have to implement all the methods from an interface or else it has to be made an abstract class. Yes you can declare methods in an interface.
9. Can you create an instance of an `abstract` class? Also, look up the Java keyword `final` and see if you can explain why a class **cannot** be both `abstract` and `final`.
- You cant create an instance of an abstract class because it doesnt have complete implementation. A class cant be abstract and final because final classes cant be extended.
10. What happens when a method **overrides** another method? If parent and child classes have methods with the same name, when you call that method on an instance of the child class, which implementation of the method will be executed?
- When you override a method you are able to set the value of the method locally in the child class.
11. What's the relationship between `List`, `LinkedList`, and `ArrayList`? Why do we call a method **polymorphic** if it takes an input of type `List` rather than an input of type `LinkedList` or `Arraylist`? Why is that useful?
- Linkedlist provide easy and fast ways for insertion and removal, ArrayList takes up less memory. When using search, it is better to use ArrayList because
elements are accessed by index. We call a method polymorphic because it has many different stages, a List is broad and can be seen and the parent of the subcategories of lists that differ.
Polymorphism is useful because it allows you to perform a single action in different ways, one interface and many implementations.
### Deliverable

This file, with your answers added.

---

## Additional Resources

Refer to the "Classes and Objects" lesson, the "Subclasses" lesson, and the "Abstract Classes and Interfaces" lesson.

Feel free to do a Google search for these concepts as well. There are plenty of Java tutorial websites and Stack Overflow posts that can help you. But be sure to write up your answers in your own words — copying and pasting some text does **not** help you actually learn (and is, in fact, cheating).
