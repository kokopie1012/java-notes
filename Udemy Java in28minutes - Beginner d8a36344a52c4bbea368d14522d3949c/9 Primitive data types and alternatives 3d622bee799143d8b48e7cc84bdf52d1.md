# 9: Primitive data types and alternatives

[Questions: 9](9%20Primitive%20data%20types%20and%20alternatives%203d622bee799143d8b48e7cc84bdf52d1/Questions%209%202d4a3de575b84c8a8be3eefeace28ac7.md)

**Wrapper** classes contain the details about these types. Like **size**.

```java
// Inside jshell:
Byte.SIZE
Byte.BYTES
Byte.MAX_VALUE
Byte.MIN_VALUE

// Same for Short, Integer, Long
Short.SIZE
Integer.BYTES
Long.MAX_VALUE
```

*By default all number literals are considered **Integers*.** If you want to make it a long literal you have to add an 'l' to it.

```java
long longNumber = 500000000l;
```

**Explicit Cast :** 

```java
int longToInt = (int) longVariable;
float floatValue = (float) doubleValue;
```

`l = i` is **Implicit Cast** because the values of a bigger container can fit inside a smaller one.

```java
// **Octal** eight
int eight = 010;

// Hexadecimal sixteen
int sixteen = 0x10;
```

Java also has *pre* and *post* increment, decrement operators.

In Eclipse : press `**CMD + 1**` (Command + One) for getting automatic reformatting.

### BigDecimal

Floating point representations (float, double) do not allow accurate representations.

You pass in a string as an argument to the BigDecimal class. BigDecimal objects are immutable.

```java
//Importing BigDecimal
import java.math.BigDecimal;

// Precision and rounding modes are the second and third argument.
BigDecimal number1 = new BigDecimal("7129.1231231238", 3, RoundingMode.UP);
BigDecimal number2 = new BigDecimal("89.129090");

number1.add(number2);
```

```java
// Adding an integer to a BigDecimal
int i = 5;
number1.add(new BigDecimal(i));
```

---

### Boolean Values

```java
>> int i = 19;
>> i >=15 && i <= 25
```

`&&` `||` are **and** and **or** in Java. `&&` and `||` are also called Short Circuit operators. If the first expression is false it does not even evaluate the other expression (in case of `&&`).

 `^` is **XOR.** `!` is **Not**. 

Single `&` and `|` are also an **and** and **or** but they do not short circuit. It evaluates all the expressions.

They way you write code, expressions etc should not have side effects.

### Character Values

If you need a cent or a rupee sign, don't hard code it. Use a character.

```java
char ch = '\u00224'; // $ sign
```

```java
char ch = 65; // 'A'
ch++; // 'B'
++ch; // 'C'
```

Adding an integer to a character returns an integer (because the integer is the larger value).

`toUpperCase()` `toLowerCase()` in the `Character` class.

```java
>> char ch = 'a';
>> Character.toUpperCase(ch);
```

**Methods having the keyword `static` don't need to be instantiated to be called. You can call them using the classname.**

A character based for loop:

```java
for (char ch = 'a'; ch <= 'a'; ++ch) {
	// CODE
}
```