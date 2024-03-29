# cash

Implement, in a file called cash.c a program that first asks the user how much change is owed and then prints the minimum number of coins with which that change can be made.

Assume that the only coins available are quarters (25¢), dimes (10¢), nickels (5¢), and pennies (1¢).

![Alt text](Screenshot0.png?raw=true "credit card")

you can handle dollars and cents, albeit sans dollar sign. In other words, if some customer is owed $9.75 (as in the case where a newspaper costs 25¢ but the customer pays with a $10 bill), assume that your program’s input will be 9.75 and not $9.75 or 975. 

However, if some customer is owed $9 exactly, assume that your program’s input will be 9.00 or just 9 but, again, not $9 or 900. Of course, by nature of floating-point values, your program will likely work with inputs like 9.0 and 9.000 as well; you need not worry about checking whether the user’s input is “formatted” like money should be.

You need not try to check whether a user’s input is too large to fit in a float. Using alone will ensure that the user’s input is indeed a floating-point (or integral) value but not that it is non-negative.

If the user fails to provide a non-negative value, your program should re-prompt the user for a valid amount again and again until the user complies.

Be sure that your program’s last line of output is only the minimum number of coins possible: an integer followed by \n.

Beware the inherent imprecision of floating-point values. Recall floats.c from class, wherein, if x is 2, and y is 10, x / y is not precisely two tenths! 

To test:

gcc cash.c cs50.c && ./a.out

![Alt text](Screenshot.png?raw=true "credit card")