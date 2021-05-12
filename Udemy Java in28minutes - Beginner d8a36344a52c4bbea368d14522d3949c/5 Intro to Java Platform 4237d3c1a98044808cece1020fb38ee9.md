# 5: Intro to Java Platform

[Questions: 5](5%20Intro%20to%20Java%20Platform%204237d3c1a98044808cece1020fb38ee9/Questions%205%20435957b092c44f3d82c69244ce7a61f9.md)

Machines only understand their implemented machine language. You have to compile code differently on different machines.

**Bytecode** helps with platform independence. **JVM**s are platform specific, bytecode is platform independent.

---

## Java Class and Objects

**Class** is a template and an **Object** is an instance of that template.

```java
class Country {
	// Method inside a class
	void getCapital() {
		System.out.println("Capital : ");
	}

}

Country India = new Country();
India.getCapital();
```

We have ***data*** and ***methods*** inside a class.

FileName should match the class name. (If top level class is Person, filename would be Person.java);

To Compile the [Person.java](http://person.java) file : 

> javac Person.java

This creates a Person.class file.

Now, to run the program : 

> java Person

---

**JVM** : Java Virtual Machine, runs java bytecode.

**JRE** : JVM + Libraries + Other Components

**JDK** : JRE + Compilers + Debuggers

---