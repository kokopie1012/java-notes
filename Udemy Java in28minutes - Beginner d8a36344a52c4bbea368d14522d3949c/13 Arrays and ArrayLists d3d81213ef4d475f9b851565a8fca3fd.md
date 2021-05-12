# 13: Arrays and ArrayLists

[Questions: 13](13%20Arrays%20and%20ArrayLists%20d3d81213ef4d475f9b851565a8fca3fd/Questions%2013%2097996a698a5643d3be4c79420526db16.md)

```java
int[] marks = {88, 98, 78};

// Default values are 0s for int arrays
int[] marks = new int[3]; // => {0, 0, 0}
marks[0] = 1;

marks.length; // => 3
```

arrayName.**length** is a **property**, not a method. Array length is a property.

default values of `**char[]**` is `**'\000'**`.

New class objects have a default value of `**null` in an array.**

```java
// To print all the elements of an array
System.out.println(Arrays.**toString**(marks)); // toString is a static method.
```

```java
// Fill an array with some value
int[] arr = new int[5];
Arrays.**fill**(arr, 1000);
```

```java
// Check wheter to arrays have same elements or not
int[] arr1 = {1,2,3};
int[] arr2 = {1,2,3};
Arrays.**equals**(arr1, arr2);
```

```java
// Sort arrays
int[] arrNew = {32,22,9,78,54};
arrNew.**sort**();
```

If you want to pass an array as an argument directly:

```java
Student student = new Student("Ranga", new int[] {22,34,35});
```

---

**Variable Arguments (`type...`)**

Variable arguments should always be the last argument inside the argument.

```java
void someFunction(int... numbers) {
	// Code
}
```

Adding and deleting items from an array is v v difficult. For that we have arraylist

### **ArrayList**

To get the size of an arrayList .**length** does not work. We use `**size()**` instead.

```java
ArrayList<String> arrList = new ArrayList<String>();
arrList.**add**("Apple");
arrList.**add**("Banana");

arrList.**size**();

arrList.**remove**("Apple");
```

```java
ArrayList<Integer> intList = new ArrayList<Integer>();

// Finding the max value in a collection
**Collections**.*max*(intList);
**Collections**.*min*(intList);
```