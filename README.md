Java Notes 
1. Variables 
2. Arithmetic Operators : Addictive operators , Subtractive operators , Multiplication operator , division operator , modulus operator 
3. Relational Operators : == equal to , < less than , > greater than , <= less than or equal to , >= greater than or equal to , != not equal to 
4. Logical Operator : && : AND operator , || : OR operator , ! : NOT operator
5. Control Structures : The statements which change the flow or order of execution of the instructions are called control structures 

There are three types of control structures : Sequential , Selection and Iteration 

Sequential : Control flow through all the statements in the order in which it is written 

Selection : Based on some conditions, control flows to different set of statements 

Iteration : Certain statements will be executed repeatedly 

Example of it : 

Input Food_Item, Quantity, Customer_Type
Unit_Price = 10
Total_Cost = Unit_Price * Quantity
if (Customer_Type == "Regular") then
	Total_Cost = Total_Cost - (Total_Cost * 5 / 100)
	Display "You are a regular customer and eligible for 5% discount"
else
	Total_Cost = Total_Cost + 5
	Display "You need to pay an additional delivery charge of $5"
end-if
Display "Order successfully placed for ", Food_Item
Display "Total cost is: ", Total_Cost

A Short program code or a pseudo-code 

display nightsky 
display moon 
display rain 
for counter
add mountain 
end for 
add tree
for counter 
add sheep
end for 

Let us try to understand the given Java program now.



The program displays a message - 'Hello World! Welcome to Java Programming!'. Here are some of the syntax rules of Java language:

The message is displayed using System.out.println which is used for displaying messages or output in Java.

Every statement in Java program must end with semicolon (;).

Every statement in Java must be present inside a method. A method is a block of code that performs a particular task.

In the code given above, the method is named as main. Every program in Java must have a main method as the code execution starts from the main method.  

The method is defined using curly braces ({}). { signifies the start of a code block and } signifies its end.

Every method in Java must be present inside a class. In the code given above, the class is named as Welcome. You will learn about classes and methods in detail later in the course.

Java is a case-sensitive programming language. E.g. - The word class should be written in lower case.