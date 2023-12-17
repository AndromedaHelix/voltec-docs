Loops and Flow Control
=======

Flow Control
--------

**If Statements**

An if statement is used to check if a condition is true. 
If it is true, the code inside the if statement will be executed. 
If it is not true, the code will be skipped, but we can use an else if statement to check another condition that could execute different code. 
If none of the conditions are true, we can use an else statement.

**Operators**

In order to check if a condition is true, we can use any of the following operators:

+--------+-------------------+-------------------+
| Operator |       Meaning     |      Example    |
+========+===================+===================+
| ==     | Equal to          | 1 == 2  (False)   |
+--------+-------------------+-------------------+
| !=     | Not equal to      | 1 != 2  (True)    |
+--------+-------------------+-------------------+
| >      | Greater than      | 1 > 2   (False)   |
+--------+-------------------+-------------------+
| <      | Less than         | 1 < 2   (True)    |
+--------+-------------------+-------------------+
| >=     | Greater than or   | 1 >= 2  (False)   |
+        | equal to          |                   |
+--------+-------------------+-------------------+
| <=     | Less than or      | 1 <= 2  (True)    |
+        | equal to          |                   |
+--------+-------------------+-------------------+

**Example**

.. code-block:: java

    if (x > 0) {
        System.out.println("x is positive");
    } else if (x < 0) {
        System.out.println("x is negative");
    } else {
        System.out.println("x is zero");
    }


**AND, OR, NOT**

* AND && is used to check if two conditions are true
* OR || is used to check if one of two conditions are true
* NOT ! is used to check if a condition is false

.. code-block:: java

    //Any number between 0 AND 10 will enter the condition
    if (x > 0 && x < 10) {
        System.out.println("x is between 0 and 10");
    } 

    //If the number is 0 OR 10, it will enter the condition
    if (x == 0 || x == 10) {
        System.out.println("x is either 0 or 10");
    }

    //If the number is NOT 0, it will enter the condition
    if (!(x == 0)) {
        System.out.println("x is not 0");
    }

**Switch**




Loops
-------

**While**

**Do-While**

**For**




