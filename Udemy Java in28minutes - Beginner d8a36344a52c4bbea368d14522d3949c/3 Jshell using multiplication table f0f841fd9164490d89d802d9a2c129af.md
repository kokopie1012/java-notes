# 3: Jshell using multiplication table

[Questions: 3](3%20Jshell%20using%20multiplication%20table%20f0f841fd9164490d89d802d9a2c129af/Questions%203%202055bc732b61415eb0252ea19d2eee1b.md)

Break down problems into smaller parts. Then **design** a solution.

```java
/exit
// TO exit from jshell '/' included
```

```java
// Random value between 0 and 1
Math.random();

// Takes only 2 arguments
Math.min();
```

```java
// Generates a print stream
System.out.printf("%d \n", 25/3);

// To actually run it in jshell:
System.out.printf("%d \n", 25/3).println();
```

```java
// TYPE variable_name = value.
int var = 13;
```

```java
// Integer data types
byte // 1 byte
int // 4 byte
short // 2 byte
long // 8 byte
```

```java
float f1 = 4.23f; // 8 bytes
double d1 = 55.78; // 8 bytes
```

A floating point value by **default is a double.** We put the 'f' to signify that the value is float instead of double.

Both float and double are not very precise. We won't use them for financial calculations or other important stuff. We would use BigDecimal or something else.

```java
char ch = 'a';
boolean bool = true;
```

```java
"1" + 2 = "12"
```

```java
int i, j = 10;
//
for (int i = 0, int j = 0; i < 10, j < 10; ++i, ++j) {}
//
for (;;); // INFINITE LOOP

```