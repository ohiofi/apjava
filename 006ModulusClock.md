Create a program that uses integer division and modulus division to calculate the time after a specified number of hours and minutes.

Review the example on Big Java pg 138 about converting pennies to dollars using / and %.

DO NOT worry about am or pm

DO NOT use any [magic numbers](https://en.wikipedia.org/wiki/Magic_number_(programming)#Unnamed_numerical_constants)

Write your pseudocode as comments.

Prompt the user for the hour of the start time and the minutes of the start time. Then prompt for the number of hours later and the number of minutes later.

Calculate the future time.

Include this bit of code at the end of your calculation (you do not have to use the variable name futureHour):
```javascript
// Convert zero o'clock to twelve o'clock
if (futureHour == 0){
  futureHour = 12;
}
```
Tell the user what the future time will be after that many hours and minutes.

Upload to GitHub
