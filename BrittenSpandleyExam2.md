# Britten Spandley Exam 2 Review

## Chapter 1, 2, 3, 4, and 5

### Make a:

print statement,
int,
double,
string

```java

public class test_file {

	public static void main(String[] args) {
		int steve = 42;
		double stevie = 42.0;
		String steverson = "Steve stevie steverson.";
		System.out.println("Steve equals " + steve + " but Stevie equals " + stevie + " so " + steverson);
	}

}
```

## Use

an if statement

```java

public class test_file {

	public static void main(String[] args) {
	
		int steve = 42;
		if (steve == 42) {
			System.out.println("Neato burrito.");
		}
	}

}
```
for loop

```java

public class test_file {

	public static void main(String[] args) {
	
		System.out.println("Count to 100!");
		for (int i = 0; i < 101; i++) {
			System.out.println(i);
		}
		
	}

}
```
Math.random() to make a coin toss

```java

public class test_file {

	public static void main(String[] args) {
	
		int coin = 0;
		int heads = 0;
		int tails = 0;
		
		for (int i = 0; i < 100; i++) {
			coin = (int)(Math.random() * 2);
			
		if (coin == 1) {
			heads++;
		} else {
			tails++;
			}
		}
		System.out.println("The coin landed on heads " + heads + " times and landed on tails " + tails + " times.");
	}

}
```
Math.random() to make an integer between 1 and 1,000

```java

public class test_file {

	public static void main(String[] args) {
	
		int randomInt = 0;
		
		for (int i = 0; i <= 1000; i++) {
			randomInt = (int)(Math.random() * 1000);
		}
		
		System.out.println("Here's a random interger: " + randomInt);
		
	}

}
```
a trig function

```java

public class test_file {

	public static void main(String[] args) {
		
		double num;
		double num1 = 5;
		
		num = Math.cos(num1);
		System.out.println("Answer: " + num);
		
		
	}

}
```
a comparison of two strings

```java

public class test_file {

	public static void main(String[] args) {
		
		String nice = new String("cool.");
		String nicer = new String("cool.");
		
		if (nice == nicer) {
			System.out.println("Nice.");
		}
	}

}
```
a comparison of two strings that ignores case

```java

public class test_file {

	public static void main(String[] args) {
		
		String s1 = "yo";
		String s2 = "YO";
		
		int com1 = s1.compareToIgnoreCase(s2);
		System.out.println("String 1 and String 2 comparison: " + com1);	
		
	}

}
```
use a scanner

```java
import java.util.Scanner;

public class test_file {

	public static void main(String[] args) {
		
		Scanner input = new Scanner(System.in);
		System.out.println("Enter your number: ");
		int enterYourNumber = input.nextInt();
		System.out.println(enterYourNumber + " is a sick number, bro.");
		
		
	}

}
```

## Chapter 6: Custom methods

### make a custom method that:

returns nothing (void) and accepts nothing();

```java

public class test_file {

	public static void main(String[] args) {

		returnNothing();
		
	}

	private static void returnNothing() {
		System.out.println("This method does nothing.");
		
	}

}
```
returns nothing and accepts an integer

```java

public class test_file {

	public static void main(String[] args) {
		
		int steve = 0;
		returnAnInt(steve);
		
	}

	private static void returnAnInt(int steve) {
		System.out.println(steve);
	}

}
```
returns nothing and accepts a string

```java

public class test_file {

	public static void main(String[] args) {
		
		String steve = "wow";
		returnAString(steve);
		
	}

	private static void returnAString(String steve) {
		System.out.println(steve);
	}

}
```
returns an int and accepts nothing

```java

public class test_file {

	public static void main(String[] args) {

		returnAnInt();
		
	}

	private static int returnAnInt() {
		int steve = 5;
		return steve;
		
	}

}
```
returns a double and accepts an int

```java

public class test_file {

	public static void main(String[] args) {

		returnADouble();
		
	}

	private static double returnADouble() {
		double steve = 5.0;
		return steve;
		
	}

}
```
returns a string and accepts two ints

```java

public class test_file {

	public static void main(String[] args) {

		int steve = 0;
		int bob = 0;
		returnAString(steve, bob);
		
	}

	private static String returnAString(int steve, int bob) {
		String nice = "That's two ints.";
		return nice;
		
	}

}
```
returns a double and accepts an array

```java

public class test_file {

	public static void main(String[] args) {

		int[] array = {0,1,2,3,4,5};
		returnADouble(array);
		
	}

	private static double returnADouble(int[] array) {
		double nice = 5.0;
		return nice;
		
	}

}
```
returns an array and accepts an array

```java

public class test_file {

	public static void main(String[] args) {

		int[] array = {0,1,2,3,4,5};
		returnAnArray(array);
		
	}

	private static int[] returnAnArray(int[] array) {
		int[] nice = {0,1,2,3,4,5};
		return nice;
		
	}

}
```

## Arrays

### Make a

Single dimensional array

```java
import java.util.Arrays;

public class test_file {

	public static void main(String[] args) {

		int[] singleArray = {0,1,2,3,4,5};
		System.out.println(Arrays.toString(singleArray));

	}

}
```
Multi dimensional array

```java
import java.util.Arrays;

public class test_file {

	public static void main(String[] args) {

		int[][] multiDimesionalArray = {{0,1,2,3,4,5}, {0,2,4,6,8,10}};
		System.out.println(Arrays.toString(multiDimensionalArray));

	}

}
```
Sort an array

```java
import java.util.Arrays;

public class test_file {

	public static void main(String[] args) {

		int[] sortedArray = {0,1,2,3,4,5,6,7,8,9,10};
		Arrays.sort(sortedArray);
		System.out.println(Arrays.toString(sortedArray));
		
	}

}
```
Make a jagged array

```java
import java.util.Arrays;

public class test_file {

	public static void main(String[] args) {

		int[][] jaggedArray = {{0,1,2}, {52,69}};
		System.out.println(Arrays.toString(jaggedArray)); 
	}

}
```
