# 15: Collections

[Questions: 15](15%20Collections%20bfa590c0fa4c42119ab352e1cb053a69/Questions%2015%20a30e56d7e88744d4b035b171d8debb80.md)

---

Don't focus on your low level data structures, focus on your business logic.

# List

Any collection creates with `.of()` method is immutable. Like `List.of();` and `Map.of();`

```java
// List.of(); is a **static method**
List<String> words = List.of("Apple", "Bees", "Cat");
words.**size**(); // 3
words.**isEmpty**();

// Access specific element from the list
words.**get**(1); // Bees

words.**contains**("Dog");

words.indexOf("Bees"); // 1

words.indexOf("Ele"); // -1 => because it doesn't exist.
```

Creating other collections from List structure. ArrayList, LinkedList and Vector are mutable, so you can add and remove items from them.

ArrayLists allow duplicates.

```java
List<String> wordsArrayList = new ArrayList<String>(words);

List<String> wordsLinkedList = new LinkedList<String>(words);

List<String> wordsVector = new Vector<String>(words);

**// All these methods are the same for vector arraylist and linkedlist**

wordsArrayList.**add**("New Element");

// Add element at a specific index
wordsArrayList.**add**(2, "Ball");

// Add a list to another list using addall
List<String> newList = new List.of("Yak", "Bull");
wordsArrayList.**addAll**(newList);

// Change an element at a specific position
wordsArrayList.**set**(6, "Fish");

// Delete an element - by index and by name
wordArrayList.remove(2); // remove element at index 2
wordArrayList.remove("Fish"); // remove fish from the array list

```

The underlying data structure beneath an ArrayList is an Array and a LinkedList is a *Doubly* LinkedList.

---

**Vector** class is `**synchronised**`. That means vector is thread-safe, in the sense that you can use vector in situation where you are sharing data between multiple threads.

If you want thread-safety then you will use vector.

If an instance of the vector class is shared between multiple threads, then only one of those threads can be executing any of these methods.

Finish CS-APP You won't get the concurrent stuff otherwise.

ArrayList is not thread-safe.