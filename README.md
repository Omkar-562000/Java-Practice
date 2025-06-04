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

Keywords:

abstract : else : return
break : final : static 
case : for : switch 
class : if : throw
continue : import : try 
default : interface : this 
do : new : while 

Example of how the variable is been stored into the program an how it is been written properly 

public static void main(String[] args) {
	int discount = 10; // discount is a variable
	double totalPrice = 200; // totalPrice is a variable
	double priceAfterDiscount = totalPrice * (1 - ((double) discount / 100)); // priceAfterDiscount is a variable
	System.out.println("Customer has paid a bill of amount: "+ priceAfterDiscount);
}

Data Type :
1. Primitive : Variables of Primitive Data Types hold the value of the data item 
2. Non - primitive : Variables of Non-Primitive Data Types hold the reference of the memory location where the data object is stored . Also known as Reference Data Types 

Here are some of the important points about primitive data types:

1. Numeric and boolean (true, false) values are written without quotes. E.g. int score = 85; boolean isQualified = true;

2. The character value must be written in single quotes while assigning it to a character variable. E.g. char gender = 'M';

3. A long value is assigned to the variable, suffixed with L (uppercase letter or lower case letter L can be used). E.g. long salary = 500000L; 

4. A float value must be suffixed with F or f while assigning to the variable. E.g. float average = 78.6f;

5. ou will learn about different places in the program where the variables can be declared. As of now, note that the default values are not applicable to the variables declared inside a method. The variables declared inside a method must be initialized with a value before printing their value or performing any operation on them. E.g.

class Demo {
	public static void main(String[] args) {
		int quantity;
		float totalCost = 10 * quantity; // error on this line
		System.out.println(totalCost);
	}
}

Non-primitive Data type includes classes , arrays , interfaces etc . These can be predefined in java library or user-defined in the programs. These will be covered in detail later in the course.

Eg :- String is a predefined class in Java library which is used to store a sequence of characters : 

			String custName:"Omkar";

In Java, variable names should be nouns starting with lowercase letter. If it contains multiple words, then every inner word must start with capital letter. This type of casing is called camel casing.

Some examples of variables are given below:

1. mobileNumber
2. name
3. unitPrice
4. paymentMode
5. age

Comments are those statements which are not executed by the compiler. Comments can be used to provide information about a variables or statement.

There are two types of comments in Java:

Single line comment

It is used to comment only one line

Syntax : //This is a single line comment

Eg : public static void main(String args[]) {
	int age = 25; // Here age is a variable
	System.out.println(age);
}

Multi-line comment

It is used to comment multiple lines of code

Syntax : /*This is a
​multi-line comment*/
​
Eg : public static void main(String args[]) {
	/*
	  Given below is a variable age 
      and a print statement to print age
	 */
	int age = 25;
	System.out.println(age);
}

Operators : Operators are the symbols used to perform specific operations. There are various operators that can be used for different purposes.

The operators are categorized as: 

1. Unary 
2. Arithmetic  
3. Relational 
4. Logical 
5. Ternary 
6. Assignment 
7. Bitwise

You will now see the different types of operators in detail

1. Unary operators act upon only one operand and perform operations such as increment, decrement, negating an expression or inverting a boolean value. 

Eg: 
public static void main(String args[]) {
	int numOne = 10;
	int numTwo = 5;
	boolean isTrue = true;
	System.out.println(numOne++ + " " + ++numOne); //Output will be 10 12
	System.out.println(numTwo-- + " " + --numTwo); //Output will be 5 3
	System.out.println(!isTrue + " " + ~numOne); //Output will be false -13
}

