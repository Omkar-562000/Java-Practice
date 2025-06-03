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

