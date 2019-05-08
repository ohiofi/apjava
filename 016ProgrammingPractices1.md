# P2-2

Write a GrowSquarePrinter program that constructs a Rectangle object square representing a square with top-left corner (100, 100) and side length 50, prints its location by calling System.out.println(square), applies the translate and grow methods, and calls System.out.println(square) again. The calls to translate and grow should modify the square so that it has twice the size and the same top-left corner as the original. If the squares were drawn, they would look like the figure below.

Your program will not produce a drawing. It will simply print the locations of square before and after calling the mutator methods.

Look up the description of the grow method in the API documentation.

# P2-3

Write a CenteredSquaresPrinter program that constructs a Rectangle object square representing a square with top-left corner (100, 100) and side length 200, prints its location by calling System.out.println(square), applies the grow and translatemethods, and calls System.out.println(square) again. The calls to grow and translate should modify the square so that it has half the width and is centered in the original square. If the squares were drawn, they would look like the figure below. Your program will not produce a drawing. It will simply print the locations of square before and after calling the mutator methods. Look up the description of the grow method in the API documentation.

# P2-5

In this exercise, you will explore a simple way of visualizing a Rectangle object. The setBounds method of the JFrame class moves a frame window to a given rectangle. Complete the following program to visually show the translate method of the Rectangle class:

```java
import java.awt.Rectangle;
import javax.swing.JFrame;
import javax.swing.JOptionPane;
public class TranslateDemo
{
   public static void main(String[] args)
   {
      // Construct a frame and show it
      JFrame frame = new JFrame();
      frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
      frame.setVisible(true);
      // Your work goes here: Construct a rectangle and set the frame bounds
      JOptionPane.showMessageDialog(frame, "Click OK to continue");
      // Your work goes here: Move the rectangle and set the frame bounds again
   }
}
```
# P2-6

Write a program LotteryPrinter that picks a combination in a lottery. In this lottery, players can choose 6 numbers (possibly repeated) between 1 and 49. Construct an object of the Random class (see [Exercise •• E2.12](https://jigsaw.vitalsource.com/books/9781119141594/epub/OEBPS/bjeo6_ch02-33.xhtml#_idTextAnchor257) ) and invoke an appropriate method to generate each number. (In a real lottery, repetitions aren’t allowed, but we haven’t yet discussed the programming constructs that would be required to deal with that problem.) Your program should print out a sentence such as “Play this combination—it’ll make you rich!”, followed by a lottery combination.

# P2-9

In Java 8, the LocalDate class describes a calendar date that does not depend on a location or time zone. You construct a date like this:

```java
LocalDate today = LocalDate.now(); // Today’s date 
LocalDate eckertsBirthday = LocalDate.of(1919, 4, 9);
```

The plusDays method can be used to add a number of days to a LocalDate object:

```java
LocalDate later = today.plusDays(10); // Ten days from today 
```

This method does not mutate the today object, but it returns a new object that is a given number of days away from today. To get the year of a day, call

```java
int year = today.getYear();
```

To get the weekday of a LocalDate, call

```java
String weekday = today.getDayOfWeek().toString();
```

Your task is to write a program that prints

The weekday of “Pi day”, that is, March 14, of the current year.
The date and weekday of “Programmer’s day” in the current year; that is, the 256th day of the year. (The number 256, or 28, is useful for some programming tasks.)
The date and weekday of the date that is 10,000 days earlier than today.
