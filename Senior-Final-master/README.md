# Senior Final Project

This project completes the password checking password program that we saw in class.  Your program must check that your password is the correct length (already done), has both uppercase and lowercase characters, has numerical characters, and has special characters !@#$%^&* (shift characters 1 through 8);


## string.js

You have 6 functions to completes.
-  PasswordMessage()
-  inRange()
-  exports.containsUpper = function()
-  exports.containsLower = function()
-  exports.containsNumerical = function()
-  exports.containsSpecial = function()

#### Password message
This function is an object constructor outside of a class; you SHOULD NOT use the word "class" or "constructor", it's all good.
-  This function has one input m.
-  This constructors has two instance variables
    -  name: automatically assign it the string value "Password Message".
    -  message: assign it the parameter m


#### inRange
-  This function has three inputs char, min, and max.  I have a pre-made variable unicode for you in the function.
    -  char represents the character in a string.
    -  min represents to lowest number in a range.
    -  max represents the highest number in a range.
-  This function will either return true or false based off of the value of unicode.
    -  Your function should return true if it is inclusively in the range of min and max.
    -  Your function should return false otherwise.

#### contains upper
-  This function uses one input, str, which represents a string variable.
-  Create a variable named hasUpper and assign it the boolean false.
-  Write a typical try-catch-block statement
    -  Inside the try statement write a for-loop which scans through the string str.  The range of uppercase characters is 65 to 90 inclusively.
    -  If the loop finds one, assign hasUpper the boolean true.
    -  If it finds an uppercase character, throw a new PasswordMessage: has uppercase character.
    -  After the for-loop, throw a new PasswordMessage: does not have uppercase character if the variable hasUpper is false;
    -  Inside the catch statement, console.log the message.
    -  Inside the catch statement, return hasUpper.

#### contains lowercase
-  This function has all of the same logic as contains upper.
-  Change the variable names and values so that you are looking for lowercase characters.
-  The range of lowercase numbers is 97 to 122 inclusively.

#### contains numerical
-  This function has all of the same logic as contains upper.
-  Change the variable names and values so that you are looking for numerical characters.
-  The range of lowercase numbers is 48 to 57 inclusively.

#### contains special
-  This function should declare a variable, hasSpecial and initialize it to false;
-  Declare an array special = [33,64,35,36,37,94,38,42]
-  Loop through the special list, throwing and returning the correct values.

## passwordGUI
This file glues all of the code together and makes the terminal cycle through its options.  Much of it as already made for you.  We will learn how this process works next year.

-  Inside of the question you should write some conditional statements which assigns the boolean false to passesAllChecks if each contains function is not true.

-  You must critically think about how to write the conditional statements so it checks all conditions and will not skip any.
