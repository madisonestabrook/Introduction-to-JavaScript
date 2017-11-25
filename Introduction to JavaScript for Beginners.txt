# Introduction to JavaScript for Beginners # 

JavaScript helps make webpages interactive. JavaScript's official name is ECMAScript. The latest version of JavaScript is ECMAScript 7. JavaScript, Hypertext Markup Language (HTML), and Cascading Style Sheets (CSS) are used together to create interactive and visually appealing web pages. 

In JavaScript, **having both the opening and closing brackets is very important**. Without matching brackets, your code contains errors and will not compile. 

[CodePen](www.Codepen.io) is a free online editor that supports HTML, CSS, and JavaScript. You can use CodePen to follow along in this lesson. 

In this lesson, you will learn will about:

* Variables      
   * Numerical Variables   
   * Strings     
* Arrays,  
   * Numerical Arrays 
   * Arrays of Strings      
* Conditionals, and      
  * If 
  * Else
  * Else If   
* Loops
  * For Loops   
  * For/In Loops   
  * While Loops  
  * Do/While Loops   

## Variables ##
Variables are containers in which you can store values. By default, variables are **undefined**, which means they do not have a value. For example, consider the variables x and y: 
> var x;    
> var y = 1; 

The variable x is undefined; x does not have a value. However, y has a value of 1. Therefore, y is defined. 

You can perform mathematical operations on variables. Some of these operations would not make algebraical sense. For example, consider the variables x, y, and z: 

> var x= 1;  
> var x = x+1;   
> var y = x+1;   
> var z = x + y   

Assigning the second instance of x the value of x plus 1 does not make algebraic sense. In JavaScript, the second statement (var x = x+1) means x is assigned the value of itself plus 1 or one plus one, which equals 2. The variable y is also assigned the value of x plus one or two plus one, which equals three. The variable x is assigned the value of y + z or three plus two, which equals five. 

You can assign a short or long name, such as p or priceofcars, to a variable. You cannot assign a variable a name that is a JavaScript keyword, such as for. Variable names in JavaScript are **not** case-sensitive, which means x does **not** equal X.

### Strings ### 
We have worked with numerical variables; however, JavaScript also allows for strings. Strings are text. For example, 
> var s = "I am a string!" 

Strings can be enclosed in single ' or double " quotation marks: 
> var x = "Another string"  
> var y = 'One more string' 

### Initialization After Declaration ### 
Variables can be initialized, or assigned a value, after they are declared. For example, the following code declares and initializes the var x in different lines: 
> var x;   
> x = 1;   

This produces the same output as 

> var x = 1; 

### Many Variables in One Line ### 
In JavaScript, you can declare and initialize more than one variable in just one line. For example, the following code declares and initializes the variables x, y, and z in the same line: 
> var x = 1, y = 2, z = 3; 

## Arrays ## 
Arrays are lists of objects. In JavaScript, arrays have the general form of **var** __array = [item1, item2, ...];__. Arrays can be lists of numbers or strings. For example, the following code declares and initializes two arrays: 
> var colors = array["pink", "purple", "yellow", "black, "gray"]   
> var arrayofpi = array[3, 1, 4, 1, 5, 9, 3] 

Arrays can be declared on multiple lines. For example, the following code produces the same output as arrayofpi: 
> var arrayofpi = array[3,   
> 1,   
> 4,   
> 1,  
> 5,   
> 9,  
> 3]  

### Accessing an Array's Elements ### 
To assign a variable to an element of an array, type **var name = array[elementnumber]**. The elements of an array start at **zero**. For an array with n elements, its index's last number is  **n-1**. For example, to access element zero of the array colors: 
> var name = colors[0] 

The value of name is "pink." To change the first element of colors to "brown" : 
> colors[0] = "brown"; 

Use the following code to access all an array's elements: 
> document.getElementById("text").innerHTML = array;

To add an element to an array, use the **push** method. For example, to add "pink" as the last element of the array colors, 
> colors.push("pink"); 

## Conditionals ## 
Conditional statements in JavaScript have three forms: 
* if 
* else 
* else if

### If Statements ### 
**If statements assess if a condition is true and will return only if a condition is true**. For example, the following code assigns w the value of seven if seven is greater than six: 
> if(7 > 6)  
> 	var w = 7

The variable w will only be declared and assigned a value if the conditional statement (7 > 6) is true. Consider the following code: 
> if (w > 9)    
> 	var y = 9

The variable y will not be declared nor assigned a value because w is seven and seven is less than nine. 

### Else Statements ### 
An if statement returns if the conditional statement is true; **an else statement returns if the conditional statement is false.** Consider the following code: 
>  var y  
> if( 8 > 9)  
> 	y = 9  
> else   
> 	y = 0

The conditional statement (8 > 9) is false; the variable y is assigned a value of zero. If the conditional statement were true, y would be assigned a value of nine. 

### Else If Statements ### 

An if statement returns if the conditional statement is true; an else statement returns if the conditional statement is false. **An else if adds another conditional statement, which returns if the conditional statement is true**. Code compiles from the top down. If both statements are true, both statements will be returned. Consider the following code:
>  var y  
> if(8 > 9)  
> 	y = 9  
> else   
> 	y = 0  
> else if (7 > 3)  
>	y = 1 

The first conditional statement (8 > 9) is false; the second the conditional statement (7 > 3) is true, which results in the returned value of y = 1. If the first condition were true, then y would be assigned the value of 9. If none of the conditional statements were true, y would be assigned a value of 0. 

## Loops ## 
**Loops can save you time if you need to repeat the same code with one variable changing**. For example, you need to add one to each element of the array arrayofpi, use the following code: 
> for (i = 0; i < arrayofpi.length; i ++) {  
>	arrayofpi[i] = arrayofpi[i] + 1; }

JavaScript supports four distinct types of loops: 
* For 
* For/In 
* While 
* Do/While 

### For Loops ### 
A for loop is a commonly used loop. A **for loop** has the following general structure: 
> **for (firststatment; secondstatement; thirdstatement)  
>	Code block goes here**
  
The firststatement is executed before the for loop starts and assigns a starting value to a variable. The secondstatement is the condition that the for loop is based on. The thirdstatement is executed after the code block is executed. 

An example for loop that squares the values of arrayofpi is: 

> for (i = 0; i < arrayofpi.length; i ++) {   
>	arrayofpi[i] += arrayofpi[i] * arrayofpi[i] }  

### For/In Loops ### 
A for/in  loop is similar to a for loop. A for/in only has one statement while a for loop has three. A **for/in loop** has the following general structure: 
> **for(var in array}  
>	Code block goes here;**   

An example for/in loop that assigns the var content to the values of the array colors follows: 
> var content = "";  
> var x  
> for(x in colors){   
> 	content += colors[x];  }    

## While Loops ## 
A while loop loops as long as a condition is true. A **while loop** has the following general structure: 
> **while(conditionalstatement)   
> 	Code block**

An example while loop that multiplies the elements of arrayofpi by two is: 
> while(i < arrayofpi.length){   
>	arrayofpi[i] += arrayofpi[i] * 2  
>	i++; } 

## Do/While Loops ##
A do/while loop loops through the code block as long as a condition is true. A **do/while loop** has the following general structure: 
> **do {   
>	Code block goes here   
> }   
> while(condition);**   

An example do/while loop that squares the values of arrayofpi is: 
> var i;   
> do {  
>	arrayofpi[i] += arrayofpi[i] * arrayofpi[i];   
>	i++;   
> }   
> while( i < arrayofpi.length)  

## Putting It All Together ## 
We have learned about: 

* Variables      
   * Numerical Variables   
   * Strings     
* Arrays,  
   * Numerical Arrays 
   * Arrays of Strings      
* Conditionals, and      
  * If 
  * Else
  * Else If   
* Loops
  * For Loops   
  * For/In Loops   
  * While Loops  
  * Do While Loops   
  
 Consider the following code: 
 > var x, y;  
 > x = 4;   
 > x = x * x;   
 > var numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]   
 
 **How would we multiply x by each of the elements of the array numbers?** 
 
 ## For Loop Solution ##
 This solution uses a for loop: 
 > var x, y;  
 > x = 4;   
 > x = x * x;   
 > var numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]  
 > for(y=0; y < numbers.length; y++){   
 >		numbers[i] = numbers[i] * x } 
 
 ## For/In Solution ##
This solution uses a for/in loop: 
 > var x, y;  
 > x = 4;   
 > x = x * x;   
 > var numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]  
 > for(y in numbers){   
 > numbers[y] = numbers[y] * x }   

  ## While Solution ##
This solution uses a while loop: 
 > var x, y;  
 > x = 4;   
 > x = x * x;   
 > var numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]  
 > while( y < numbers.length){   
 > 		numbers[y] = numbers[y] * x }   
 > 		y ++; } 

  ## Do/While Solution ##
  This solution uses a do/while loop: 
  > var x, y;  
 > x = 4;   
 > x = x * x;   
 > var numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]  
 > do {   
 > 		numbers[y] = numbers[y] * x }   
 > 		y ++; }  
 > 		while( y < numbers.length)
