# 6: Intro to Eclipse

[Questions: 6](6%20Intro%20to%20Eclipse%20f50707f045f04d0cb59f8d9f5174cab5/Questions%206%20a4c02108bfbb4a3c823b57bfc9b7f3bf.md)

Preferences >> save >> save actions >> formatting options

Don't create modules for now we'll talk about modules later.

```java
// REFACTORING
void printTable(int x) {
		printTable(x, 1, 10);
	}

void printTable(int x, int to, int from) {
		for (int i = to; i <= from; i++) {
			System.out.printf("%d x %d = %d.\n", x, i, x * i).println();
		}
}
```

RIght Click >> Debug as >> Java app >> use perspective >> step into >> step over etc...

CMD + SHIFT + L ⇒ **Keyboard Shortcuts**

- CMD + N : **New Class**
- "main (ctrl + space)" : **Main Method**
- "sysout (ctrl + space)" : `System.out.println();`
- CMD + SHIFT + R : **Search for a class**