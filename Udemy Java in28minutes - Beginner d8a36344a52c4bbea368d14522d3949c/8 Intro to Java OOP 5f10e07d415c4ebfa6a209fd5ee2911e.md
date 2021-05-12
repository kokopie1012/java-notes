# 8: Intro to Java OOP

[Questions: 8](8%20Intro%20to%20Java%20OOP%205f10e07d415c4ebfa6a209fd5ee2911e/Questions%208%2047424180623f4e7cb650be85d53bd24f.md)

Data ⇒ State | Actions ⇒ Behaviour

- $data/member/state/field$
- $actions/behaviour/methods/member-functions$

**Encapsulation** : Only the specific class should have access to the data of that class. Other classes should not be able to access data of another class *directly*. If one class can access the data from another class, it breaks *encapsulation*. 

If a class wants to access data from another class, it should do it with *getters*, *setters*, behaviour methods, actions etc.

```java
private int speed.
```

Now, this speed variable is not available outside the class. we added the `private` label to make this, otherwise the data variable is available to all other classes.

```java
**this.speed = speedArg;**

// The method inside the class would look like:
void setSpeed(int speed) {
	this.speed = speed;
}
```

We use `this` to access the member variable inside a method.

EXAMPLE:

```java
ducati.setSpeed(250);
int ducatiSpeed = ducati.getSpeed();
ducatiSpeed += 100;
ducati.setSpeed(ducatiSpeed);
```

**Eclipse Trick** : RightClick >> Source >> Generate Getters and Setters.

Always check data (data validation) before setting member variables. To prevent bad data to get into our objects. Good Practice.

**Abstraction :** I don't have to understand how a motorbike works in order to use it. We hide all the implementation complexities and only expose a simple API to work with the object/system.

**Java Constructor :** Name of the constructor is same as that of the class.

```java
MotorBike(int speedInit) {
	this.speed = speedInit;
}
```

*You can have multiple constructors of a class, just like how we overload methods*

Calling a constructor from another constructor: **** using **`this()`**

```java
MotorBike() {
	this(5);
}

MotorBike(int speedInit) {
	this.speed = speedInit;
}
```