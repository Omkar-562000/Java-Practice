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

2. Arithmetic operators : are used to perform basic mathematical operations like addition , subtraction , multiplication and division 

Eg: 
public static void main(String args[]) {
	int numOne = 10;
	int numTwo = 5;
	System.out.println(numOne + numTwo); //Output will be 15
	System.out.println(numOne - numTwo); //Output will be 5
	System.out.println(numOne * numTwo); //Output will be 50
	System.out.println(numOne / numTwo); //Output will be 2
	System.out.println(numOne % numTwo); //Output will be 0
}

3. Relational operators : are use to compare two values . The result of all the relational operations is either true or false .

Eg :
public static void main(String args[]) {
	int numOne = 10;
	int numTwo = 5;
	System.out.println(numOne > numTwo); //Output will be true
}

4. Logical Operators : are used to combine two or more relational expressions or to negate the result of a relational expression 

Eg: 
public static void main(String args[]) {
	int numOne = 100;
	int numTwo = 20;
	int numThree = 30;
	System.out.println(numOne > numTwo && numOne > numThree); //Output will be true
}

5. Ternary operator : is use as single line replacement for if-then-else statements and acts upon three operands.

Syntax: 
<condition>? <value if condition is true>: <value if condition is false>

Eg: 
public static void main(String args[]) {
	int numOne = 10;
	int numTwo = 5;
	int min = (numOne < numTwo) ? numOne : numTwo;
	System.out.println(min); //Output will be 5
}

6. Assignment operator : is used to assign the value on the right hand side to the valriable on the left hand side of the operator 

Eg : 
public static void main(String args[]) {
	int numOne = 10; //The value 10 is assigned to numOne
	System.out.println(numOne); //Output will be 10
	numOne += 5;
	System.out.println(numOne); //Output will be 15
	numOne -= 5;
	System.out.println(numOne); //Output will be 10
	numOne *= 5;
	System.out.println(numOne); //Output will be 50
	numOne /= 5;
	System.out.println(numOne); //Output will be 10
}

7. Bitwise operators are used to perform manipulation of individual bits of a number.

Before we take a look at the different bitwise operators, let us understand how to convert a decimal number to binary number and vice versa.

The decimal or the base 10 number system is used in everyday life but the binary number system is the basis for representing data in computing systems.

You will now see how to convert a decimal number to binary number.

Step 1:

Divide the decimal number by 2.

Step 2:

Write the number on the right hand side. This will be either 1 or 0.

Step 3:

Divide the result of the division and again by 2 and write the remainder.

Step 4:

Continue this process until the result of the division is 0.

Step 5:

The first remainder that you received is the least significant bit and the last remainder is the most significant bit.



 

You will now see how to convert the binary number back to decimal number.

The decimal number is equal to the sum of binary digits (dn) times their power of 2 (2n).

Lets take the example of 11001.

11001 = 1*24+1*23+0*22+0*21+1*20=16+8+0+0+1=25

Data Type Compatibility 

When you assign the value of one data type to another or when you perform operation on two operands, their types mut be compatible with each other . If the data types are not compatible, then the data type of an operand needs to be converted . 

This conversion is of two types :

1. Implicit 
2. Explicit 

Implicit Type Conversion is also known as Widening conversion. It happens in the below scenarios: 

When a value of a data type with smaller range is assigned to a variable of a compatible data type with larger range. 

When two variables of different data types are involved in an expression, the value of smaller range datatype is converted to a value of larger range datatype and then the operation is performed. 

E.g.: 
int discountPercentage = 10; 
double newDiscountPercentage = discountPercentage; 

Explicit Conversion is used when you want to assign a value of larger range data type to a smaller range data type. This conversion is not done by the compiler implicitly as there can be loss of data in some cases. Hence, programmer has to be cautious about such conversions. This is also known as Narrowing conversion. 

E.g.: 
double totalPrice = 200;  
int newPrice = totalPrice;  

This will lead to an error because a value of larger range data type, in this case double, cannot be directly assigned to a smaller range data type, in this case int. Here, you need to explicitly typecast double to int as shown below.

int newPrice = (int)totalPrice;

Data Types and Operators 

Types of Control Structures
- Sequential : All the statements are executed in the order in which it is written 
- Decision / Selection : Changes the flow of execution according to a condition or decision taken 
Eg:- if,if-else,switch
- Iteration : Repeatedly executes the same set of statements based on some condition 
Eg:- for,while,do-while


**If Statement Logical theory**
An "if" statement contains a relational and logical expression followed by a block of statements. Based on the result of the expression, the corresponding statements/code blocks get executed or skipped.

Syntax:

if (<condition>) {  // Curly braces are not required if there is only one statement inside the block
    <statements>;
}

 The statements inside the "if" block gets executed only when the condition evaluates to true.

**If-Else Statement Logical theory**
 An if statement can be written along with an else statement. The condition/expression given in the if statement is checked and set of statements are executed based on the outcome of the condition. If the condition is true, the statements written in if block get executed. If the condition is false, then the statements inside else block get executed.

Syntax:

if (<condition>) { 
    <statements>; 
} 
else { 
    <statements>; 
} 

**If-else if Statement Logical theory**
You can also have else if statements. As the name suggests, it is a combination of else and if. Like else, it extends an if statement to execute a different set of statements in case the original if expression evaluates to false. Then, the conditions present inside the else if blocks are checked. Once a condition evaluates to true, remaining else if and else statements are skipped.

When all the conditions are false, the else block is executed. Coding the else block is optional.

Syntax:

if (<condition 1>) {
    <statements>;
}
else if (<condition 2>) {
    <statements>;
}
else if (<condition 3>) {
    <statements>;
}
else {
    <statements>;
}

**Nested If Statement Logical theory**
When an if statement is written within another if statement, it is known as nested if statement. It enables us to test multiple criteria. The inner if block condition gets executed only when the condition of the outer if block evaluates to true.

Syntax:

if (<condition 1>) {
    if (<condition 2>) {
        <statements>;
    }
    else {
        <statements>;
    }
}

**Switch Case Statement Logical theory**

The switch statement enables to select a block from a set of options. It allows the flow of execution to be switched according to a value.

Syntax:

switch (expression or variable) {
   case value1: <statements>;
                break;
   case value2: <statements>;
                break;
   default: <statements>;
}

During execution, the result of expression or variable written in the switch statement is compared with the constant values of cases one by one. When a match is found, the set of statements present in that case are executed until a break statement is encountered or till the end of switch block, whichever occurs first. In the absence of break statement, the flow of control falls through subsequent cases and executes the statements of all those cases until it reaches a break statement or end of switch block. 

The switch block can have a special case called default. The default case is executed when none of the cases match with the value of expression/variable. default is optional. If none of the cases match and if there is no default statement, the control comes out of switch block without executing any case.

In Java, the switch block works only for the following data types:

char and integral datatypes are supported in switch-case statement, but float or double are not supported.

String datatype is also supported in switch-case statement from Java 7 version onwards

**While -Iteration Control Structures**

Iteration control structures are used to execute a set of statements repeatedly. To terminate the repetition, a condition is required. 

Let us consider that the girl in the image should jump over the rope repetitively until she is tired. That means, a repeated action has to be performed as long as a condition (getting tired) is met. Also, the number of times the girl is going to jump over the rope cannot be estimated before. 

**While-Loop**

Similarly, in programming, when you want to repeatedly execute the statements as long as a condition is met, you can use the iteration control structure called while loop. When the condition becomes false, the while loop terminates and control goes to the statement written after the while loop. The while loop is used when the number of iterations are not known. In case of while loop, the condition is tested before entering the while loop block and hence it is known as an entry-controlled loop.  

Syntax: 

while (<condition>) { 
   <statements>; 
} 

**Do-While Loop**

When the loop has to be executed at least once before the condition is checked, do-while loop is used. After the first execution, the loop then gets repeated as long as the condition is true. In case of do-while loop, the condition is tested after executing the code block. Hence, it is called an exit-controlled loop.  

Syntax: 

do { 
   <statements>; 
} while (<condition>); 
 
 **For Loop Statement**

 The 'for' loop is used when the number of iterations are known.  

Syntax: 

for (<initialization>; <condition>; <increment/decrement>) { 
     <statements>; 
} 
Initialization: It is used for initializing the variables used for checking the condition. It is executed only once and gets executed when the loop starts.

Condition: It is used for checking the condition to decide whether the loop should be terminated or executed. If the condition is true, the body of the loop is executed, else the loop terminates.  

Increment / Decrement: It increments or decrements the value of the variable used for checking the condition after every iteration of the loop.  

All the three parts of for loop are optional. For instance, the for loop can also be written as for(;;) where none of the parts are provided. This for loop will result in infinite loop.

**Nested Loop**

A nested loop is a loop within another loop , an inner loop within the body of an outer one . 

class Numbers {
	public static void main(String[] args) {
		int rows = 10;
		for (int i = 1; i <= rows; ++i) {
			for (int j = 1; j <= i; ++j) {
                // print displays the text without adding a new line
				System.out.print(j + " "); 
			}
			System.out.println(""); // println displays the text along with a new line
		}
	}
}

break statement is used to terminate a loop. After terminating the loop, the next statement following the loop gets executed. In case of break statement written in nested loops, the inner most loop gets terminated and the flow of control continues with the statements of outer loop.  

break statement is also used to terminate the execution of a switch case, as already discussed.

 **Coninue Statement**

 continue statement is used to skip the current iteration of a loop and continue with the next iteration. In case of while and do-while loops, continue statement skips the remaining code of the loop and passes the control to check the loop condition. Whereas in case of for loop, the control goes to the increment section and then the condition is checked.

 **OOPS**

 Object Oriented Programming(OOP) is a type of programming approach which enables the programmers to work with real life entities like Customer, Trainee, Employee, Company, Product, Food, Book, etc.

Java, C#, Simula, JavaScript, Python, C++, Visual Basic .NET, Ruby, Scala, PHP etc. are some of the popular object-oriented programming languages.

OOP helps a programmer in breaking down the code into smaller modules. These modules (classes) will have state(represented by attributes/variables) and functionality (represented by behavior/methods).

These modules can then be used for representing the individual real life entities known as objects.

E.g. - We can have a class named Customer to represent the state and behavior of all customers. Each individual customer can then be represented using an object of the Customer class.

OOP has many advantages. Some of them are listed below:

Modularity: OOP enables programmers to create modules that do not need to be changed when an object is added.

A programmer can simply create a new object to represent a new real-life entity.

Scalability: OOP makes development and maintenance easier.

Since the design is modular, part of the system can be updated in case of issues without a need to make large scale changes.

In structured programming (like C language), it is not easy to manage the code as project size grows. These languages have functions that do not clearly segregate the functionality and attributes and makes it difficult for the programmer to understand the code.

Data hiding: OOP provides hiding and securing data.

Real life scenario: OOP provides ability to simulate real world event more effectively and efficiently.

**Important about Class and Object**

A representation specifying the characteristics and behaviors of an object is called a class. It is not a real life entity but a template for representing real life entities.

An object, which is an instance of a class is a real life entity which has some attributes and behaviors. The class determines the attributes and behaviors which an object should possess to belong to the class.

## Class 

A class can have attributes (characteristics) and methods (behaviors)

Attributes are the elements or variables which hold the values or state of a particular entity.

Update the class Customer as shown below:

class Customer {
	public String customerId;
	public String customerName;
	public long contactNumber;
	public String address;
}
In the code given above, customerId, customerName, contactNumber and address are the attributes of the class Customer.

Attributes are represented in classes by variables.

Attributes represent the state of a real life entity.

Each real life entity can have its own values for those variables. Since each instance of a class has different values for its variables, these variables are called instance variables.

Each instance variable has a data type associated with it. In the given code, String and long are the data types used.

Apart from data types, you can see another keyword being used, public. It is an access modifier.

Access modifiers help in limiting access to the members of a class. It can be used along with class, attribute and method.

There are multiple access modifiers. Let us discuss two of them now.

private - private allows members to be accessible only inside the class

public - public allows members to be accessible in other classes as well

