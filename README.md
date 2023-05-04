Download Link: https://assignmentchef.com/product/solved-cs52-problem-set-2-programming-projects
<br>
<strong>a-easter_calculator</strong>

Our current calendaring system is the Gregorian Calendar which took effect in 1583.  One thing that is very hard to determine is the date of Easter each year.  In 1876, the following algorithm was proposed for producing the date of Easter.  At a later time, Samuel Butcher, the Bishop of Meade, showed that this algorithm is, in fact, accurate for all years in our current calendaring system.

<span style="font-family: Courier New;">a = year % 19b = year / 100c = year % 100d = b / 4e = b % 4f = (b + 8) / 25g = (b – f + 1) / 3h = ((19 * a) + b – d – g + 15) % 30i = c / 4j = c % 4k = (32 + (2 * e) + (2 * i) – h – j) % 7m = (a + (11 * h) + (22 * k) ) / 451</span>Easter Month = <span style="font-family: Courier New;">( h + k – (7 * m) + 114 ) / 31</span>                     where 3 means the month of March and 4 means April<span style="font-family: Courier New;">p = ( h + k – (7 * m) + 114 ) % 31</span>Easter Date = <span style="font-family: Courier New;">p + 1</span>

In all the calculations above, / means integer division which neglects the remainder and % means the modulus operation which performs integer division and keeps only the remainder.  For both of the previous operations to translate correctly in C++, you must have declared <span style="font-family: Courier New;">int</span> datatypes on either side of the / and % sign.  Also, please remember the order of operations which demand that multiplications occur before additions, as expressed by the parentheses I have placed in these formulas.  Write a C++ program that prompts for a year and then calculates the date of Easter.  A sample program dialogue is shown below.

HINT: You might try building these calculation inside Excel and then do them step-by-step, verifying the values calculated in your program against your spreadsheet answers…

<span style="font-family: Courier New;">What’s the year: 2006Easter Month is AprilEaster Day is 16</span>

What’s the year: 2005Easter Month is MarchEaster Day is 27

<span style="font-family: Courier New;">What’s the year: 2004Easter Month is AprilEaster Day is 11</span>

Submission Guidelines

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li>Write a program which produces the same output as the examples above

    <ul>

     What’s the year: {USER INPUT}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     Easter Month is {MONTH NAME}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     Easter Day is {DAY}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;"></li>

 <li>You are given a main.cpp file.You must implement the findEasterDate() method through files you must supplement.All files must be compile with the given main without having to modify the main file itself.</li>

 <li>Your submission should follow this organization:

  <ul>

   <li>part-a

    <ul>

     <li>main.cpp</li>

     <li>my_easter_calculator.h</li>

     <li>my_easter_calculator.cpp</li>

    </ul></li>

  </ul></li>

</ul>

<hr>

<strong>b-change_calculator</strong>

Write a C++ program that prompts for a cash value and an amount of purchases made against that amount.  The program should then determine the change using US paper and coin currency. Working with the following bills and coins:Fifty Cents, Twenty-Five Cents, Ten Cents, Five Cents, One CentOne Dollar Bill, Five Dollar Bill, Ten Dollar Bill, Twenty Dollar Billdisplay how many of each would be needed to make the change.  In order to receive full credit, you must use a loop.  The program dialog would look like:

<span style="font-family: Courier New;">Enter a value:<strong><em> 32.00</em></strong>Enter an amount of purchases made against this amount: <strong><em>18.52</em></strong>The remaining change is: 13.48Twenty US Dollar Bills: 0Ten US Dollar Bills: 1Five US Dollar Bills: 0One US Dollar Bills: 3Fifty US Cents Coins: 0Twenty-Five US Cents Coins: 1Ten US Cents Coins: 2Five US Cents Coins: 0One US Cent Coins: 3</span>

<span style="font-family: Courier New;">Continue(y/n)?<strong><em>n</em></strong></span>

HINT: You really should use integer arithmetic to ensure that your calculations, down to that very last penny, are exact and accurate.HINT: The % (modulus operator) is very helpful in computing remainders but requires two <span style="font-family: Courier New;">int</span> parameters.

Submission Guidelines

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li>Write a program which produces the same output as the examples above

    <ul>

     The remaining change is: {CHANGE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     Twenty US Dollar Bills: {VALUE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     Ten US Dollar Bills: {VALUE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     Five US Dollar Bills: {VALUE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     One US Dollar Bills: {VALUE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     Fifty US Cents Coins: {VALUE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     Twenty-Five US Cents Coins: {VALUE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     Ten US Cents Coins: {VALUE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     Five US Cents Coins: {VALUE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     One US Cent Coins: {VALUE}

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li style="list-style-type: none;"></li>

 <li>You are given a main.cpp file.You must implement the calculateChange() method through files you must supplement.All files must be compile with the given main without having to modify the main file itself.</li>

 <li>Your submission should follow this organization:

  <ul>

   <li>part-b

    <ul>

     <li>main.cpp</li>

     <li>my_change_calculator.h</li>

     <li>my_change_calculator.cpp</li>

    </ul></li>

  </ul></li>

</ul>

<ul>

 <li>Currency output must output to proper precision.For example, ‘The remaining change is: 1.200000’ will result in deductions.</li>

</ul>

<hr>

REGARDING THE ENTIRE ASSIGNMENT:

<ul>

 <li>Failing to follow these guidelines will result in deductions.</li>

 <li>I will also be grading for proper style, formatting and comments.</li>

</ul>