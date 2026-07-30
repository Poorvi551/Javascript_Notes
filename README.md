# Javascript_Notes-Interview_Prep

### * History of Javscript :

  * In 1995 javascript was developed by Brendan Eich.
  * He was working at Netscape Communication(Web Browser Company).
  * He named javascript firstly as MOCHA.
  * MOCHA -> livescript -> ECMA International(European Computer Manufacturer Association). -> ECMA script -> Javascript.

## * Javascript :-

  * Javascript is used to add functionality for the web pages.
  * Javascript is a light-weight object based programming or scripting language used by several websites for scripting the webpages.
  * Javascript is a client-side(frontend) language.      Python(server-side)

### * Features of Javascript:-

  * Javascript is a interpreted language.
  * Javascript is dynamically typed language.
  * JIT(Just In Time) is present.
  * Client side language.
  * Supports - cross platform.
  * Event - driven Architecture.

#### * Applications of Javascript:-

  * Javascript can be used for wide range of applications.
    
    1. Frontend development.
    2. Backend development using node.js
    3. Mobile App development using React native.
    4. Game development using libraries like Three.js, phaser.js(2D Games).
    5. Desktop App development using electron.js(vs code).
    6. Machine Learning using tensorflow.js

## * Javascript Engine:-

  * Javascript Engine is responsible for executing javascript code.
  * Each and every browser will have javascript engine with different names such as chrome - V8, Edge - Chakra, Firefox - SpiderMonkey, Safari - JS Core.

 ## Working of Javascript Engine:

   * Parser takes the javascript code and it generates AST.
   * AST - AST stands for Abstract Syntax Tree - It is a structured representation of a code.
   * Interpreter converts this AST it into a byte code(Intermediate or Instruction).
   * Compiler - Compiler takes byte code and converts it into a Machine code and produces output.

  * *Javascript uses JIT(Just In Time) Compiler to optimize the process of code execution.*

### Ways of writing javascript code:

  * ***NOTE : There are two ways of writing javascript code.***
    
     * Types are:

        1. Internal method
        2. External method

     1. Internal method:
        ________________________________________________________________________________________________________________
    
             <!DOCTYPE html>
             <html>
             <head>
                <meta>
                <title></title>
             </head>
             <body>
                <h1>Hello! welcome to javascript session</h1>
                <script>
                    console.log("Hello")
                </script>
             </body>
             </html>
        __________________________________________________________________________________________________________________

    2. External method :
    _______________________________________________________________________________________________________________________

    index.html
    
          <!DOCTYPE html>
             <html>
             <head>
                <meta>
                <title></title>
             </head>
             <body>
                <h1>Hello! welcome to javascript session</h1>
                <script src="index.js"></script>
             </body>
             </html>
  __________________________________________________________________________________________________________________________
  
    
  __________________________________________________________________________________________________________________________

   index.js
                  
                  console.log("Hello")
  __________________________________________________________________________________________________________________________

* ***NOTE : Javascript code should always be written before closing the body tag(</body>) at the  end of the html file because first HTML Elements and CSS Elements should be rendered before executing the javascript code.***

* ***NOTE : We can write the script tag anywhere but we have to use keywords called async or defer, this method will work only in external method of writing javascript code.***
  
  * **ASYNC** - Async will execute both HTML and Javascript code parallely.
  * **DEFER** - Defer will execute first HTML code than executes the javascript code.


* Output method :

  1. console.log() - prints the statement in the console
  2. alert() - alerts with one button as OK
  3. confirm() - alerts with two buttons as OK and cancel
  4. document.write() - prints the statement on the browser without any space.
  5. document.writeln() - prints the statement on the browser with one space.

* Tokens - Tokens are the smallest individual unit of javascript program.
* Keywords are predefined reserved words which have its own meaning.
* Identifiers - Identifiers are the name given to the javascript program.
* Literals - Literals are the values used in javascript program.

### Reserved Words:

1. Abstract
2. Boolean
3. Break
4. Byte
5. Case
6. Catch
7. Char
8. Class
9. Const
10. Continue
11. Debugger
12. Default
13. Delete
14. Do
15. Double
16. Else
17. Enum
18. Export
19. Extends
20. False
21. Final
22. Finally
23. Float
24. For
25. Function
26. Goto
27. If
28. implements
29. Import
30. In
31. Instanceof
32. Int
33. Interface
34. Long
35. Native
36. New
37. Null
38. Package
39. Private
40. Protected
41. Public
42. Return
43. Short
44. Static
45. Super
46. Switch
47. Synchronized
48. This
49. Throw
50. Throws
51. Transient
52. True
53. Try
54. Typeof
55. Var
56. Void
57. Volatile
58. While
59. With

## * Literals -

  They are of two types-
  
   1. Primitive Datatype  - Immutable(Object- Dereferencing) -> number,string,boolean,null,undefined,bigInt
   2. Non Primitive Datatype - Mutable(Object- Referencing) -> functions, arrays(filter,map,reduce), object(date,time,math)

## Variable :-

  * Variable is a named memory location which is used to store some data or value and that can be changed n number of times during execution.

  * There are 3 types  of variables :

       1. Var -> global scope
       2. let   ---\ Function scope, block scope,
       3. const ---/ script scope, local scope

 * There are 4 operations to be performed :

    1. Declaration
    2. Declaration and Initialization
    3. Re-Initialization
    4. Re-Declaration

 1. Declaration :

    * var - possible
    * let - possible
    * const - not possible

 2. Declaration and Initialization :

    * var - possible
    * let - possible
    * const - possible

 3. Re-Initialization :

    * var - possible
    * let - possible
    * const - not possible
       
 4. Re-Declaration :

    * var - possible
    * let - not possible
    * const - not possible

### * Hoisting :

* Utilising the variable before the initialization line is called hoisting.

* Ex : console.log(a)
       var a = 10;

* var -> possible - o/p -> undefined
* let, const -> Referrence Error -> TDz - Temporal Dead Zone

* Temporal Dead Zone :

   * The time gap between utilization and initialization line is called Temporal Dead Zone.

GEC Execution :

 * GEC - GEC stands for Global Execution Context.
 *  Whenever the javascript program is given to javascript Engine a new memory is created that memory is called Global Execution Context(GEC).

* GEC has 2 stages:

   1. Variable phase
   2. Function/Execution Phase
* GEC has 2 steps :

  1. Memory is created or allocated.
  2. Execution happens from top to bottom, left to right and by default all the values are assigned as undefined.

Typecasting :

* Converting one type of data into another type of data is called typecasting.

  * They are of 2 types :

     1. Implicit Typecasting
     2. Explicit Typecasting

  1. Implicit Typecasting -

     * Converting one type of data into another type of data internally or implicitly is called Implicit typecasting.
     *  Ex: console.log(1+3);

  2. Explicit Typecasting -

     * Converting one type of data into another type of data externally or explicitly is called Explicit typecasting.
     * There are 3 in-built methods. They are :
          1. Number()
          2. String()
          3. BigInt()

Inputs :

* Inputs are of 2 types :
     1. static inputs
     2. dynamic inputs

1. Static inputs :
 
      code : ex: var a=10;
                 var b=20;
                 console.log(a+b);
     
     * EX: source code : Assignment 3 folder in this repo.

2. Dynamic inputs :
 
      code : ex: var a=prompt("Enter a:");
                 var b=prompt("Enter b:");
                 console.log(a+b);  // a-> 10, b-> 20 o/p -> 1020     to overcome this use Number(prompt()) except subtract bcz subtract sign will defaultly convert it into number.
     
     * EX: source code : Assignment 3 folder in this repo.

## Literals :

1. Primitive :-

    * They are Immutable.
    * They are object Dereferencing.

  i. String Literals:

   * They are Immutable.
   * They are object Dereferencing.

      1. " " - double quotes
      2. ' ' - single quotes
      3. ` ` - Backticks
            1. Template string
            2. String Interpolation
               * Ex : source code - stringliterals.html
   
       * ***NOTE - To print the the string with double quotes like("hello") we use '"hello"' - singel quotes, to print with single quotes like('hello') we use "'hello'" and to print with backticks like(`hi`) we can use either single quotes or double quotes("`hi`") or ('`hi`').***
                 
        * String Methods :

          * Ex : source code - stringliterals.html
          * str.length - length of string
          * str.toLowerCase() - converts to lowercase
          * str.toUpperCase() - converts to uppercase
          * str.toLocaleLowerCase() - converts to lowercase
          * str.toLocaleUpperCase() - converts to uppercase
          * str.charAt(0) - prints letter at the index 0 if the space is not occupied returns blank
          * str.indexof(H) - prints index of the letter H
          * str.lastIndexOf(l) - prints from last index of the letter l where it finds the first l
          * str.slice()- prints the n-1 letter, 2 parameters (strat index, end index)
          * str.replace("H","R") - replace letter H to R.
          * str.startsWith("H") - returns boolean val( true/false) if present or not.
          * str.endsWith("o") - returns boolean val( true/false) if present or not.
          * str.trim() - removes the space at both start and end sides.
          * str.trimStart() - removes spcae at start
          * str.trimEnd() - removes spcae at end
          * str.concat(str2) - concatenates the 2 strings.
          * str.split("") - converts whole string to array.
            
     ii. Number:
     
      * They are Immutable.
      * They are object Dereferencing.
      * Ex: Source Code -number.html
           <script>
             var a=10;
             var b=10.5;
             var c=1/0;
             var d=-1/0;
             console.log(a);
             console.log(b);
             console.log(c);
             console.log(d);
             console.log(typeof a);
             console.log(typeof b);  
           </script>
          
     iii. Boolean:

      * They are Immutable.
      * They are object Dereferencing.
      * Ex: Source Code- boolean.html
           <script>
              console.log(Boolean (" "));
           </script>
        
     iv. BigInt:

      * They are Immutable.
      * They are object Dereferencing.
      * Ex: Sourcecode - BigInt.html
          <script>
             let a=1n;
             let b=BigInt(124437869860483756352);
             let c=BigInt("080912356789953243456789");
             console.log(typeof a);
             console.log(typeof b);
             console.log(typeof c);
           </script>
        
     v. Undefined:

     * They are Immutable.
     * They are object Dereferencing.
     * Ex: Source code - undefined.html
         <script>
            var a;
            console.log(a);
         </script>
       
     vi. Null:

     * They are Immutable.
     * They are object Dereferencing.
     * In null memory is created/allocated explicitly.
     * It is a defect in javascript because if check for the typeof a variable gives object (it will consider everything as an object).
     * Ex: Source code - null.html
         <script>
            var a = null;
            console.log(a);
            console.log(typeof a);  //object
         </script>

2. Non Primitive datatype:-

 * It is Mutable.
 * It is object referencing.
 * They are of 3 types :
     1. Functions
     2. Arrays
     3. Object
        
 ## 1. Functions :

   * Function is a block of statement which is excuted whenever we call or invoke.
   * Function is a non primitive datatype.
   * Function is mutable.
   * Function is object referencing.
   * There are 10 types of functions :
       1. Anonymous Function
       2. Named Function
       3. Functional Expression
       4. First class Function
       5. Arrow Function
       6. High-order Function
       7. Call-Back Function
       8. Nested Function
       9. Generator Function
       10. Immediate Invoking Function(IIF)
           
  1. Anonymous Function:

   * A function without any name is called as anonymous function.
   * Directly executing anonymous function is nor possible.
   * We can convert anonymous function into -> named, functional expression and first-class functions.
   * Syntax:-

         function()
         {
          console.log("Hello");
         }

  2. Named Function :

   * A function with any name is called as named function.
   * Syntax:-

         function demo()   // demo is the function name
         {
          console.log("Hello");
         }
         demo()   //calling function
     
  3. Functional Expression :

   * Storing the entire function into a variable is called functional expression.
   * Syntax:-

         Let x = function ()   // x is the variable name storing the function
         {
          console.log("Hello");
         }
         x()   //calling function

 4. First-class Function :

   * The function is passed as a value to a variable is called as a First-class Function.
   * Syntax:-

         Let x = function ()   // function() is passed as value to variable x this function is called first class function
         {
          console.log("Hello");
         }
         x()   //calling function

  5. Arrow Function :

   * Arrow function is used to reduce the syntax of a normal function.
   * Arrow function was introduced in ECMAScript 2015(ES6)
   * Syntax :

         let x = () =>console.log("Hello");
         x();
     
      or   

         let x = () =>{
         console.log("Hello");
         console.log("Hello! Welcome to javascript learnings");
         }
         x();
     
   * Rules for Arrow function :
     1. If the function contains more than 1 statement than the curly braces{} is mandatory.
     2. If return keyword is used than the curly braces{} is mandatory.
     3. this keyword will work different inside arrow function.
     4. If there is only one parameter we can remove paranthesis().
        * Ex:

              let x = () =>{
              return 1234;
              }
              x();
          
  6. High-order Function:

   * The function which is accepting another function as a parameter is called higher-order function.
   * Higher order function is used to perform generic task in an application.
   * Ex :
     
         function reels(auth(),home())
         {

         }

         function auth()
         {

         }

         function home()
         {

         }
     
7. Call Back Function :

 * The Function which is passed as a parameter to higher-order function is called as call back function.
 * Ex :
     
         function reels(auth(),home())   // auth() and home() are call back function
         {

         }

         function auth()
         {

         }

         function home()
         {

         }
   
 8. Nested Function : (continued further -)

   * A function inside another function is called nested function.

 10. Immediate Invoking Function(IIF) :

   * If we want to execute a function immediately we use IIF Function.
   * Ex:

         (function ()
         {
          console.log(144);
         })
         ();
     
* Return Keyword :
 
 * Return keyword is used to return some value from the function.
 * Ex:-

       function sample(){
       return 1234;
       }
       console.log(sample())
   
 * Return keyword terminates the function and comes out of the functions

## * Function Execution Context (FEC):

* Whenever a new function is called inside a javascript engine it will create a new execution context called as FEC.
* When a new FEC is created older GEC will go to garbage and the memory address of that GEC will be stored in a temporary memory called as closure.

* Closure : Closure is a temporary memory which is used to store some data and memory address for execution.

* Nested Function (Contd-):

 * Function inside another function is called Nested function.
 * Ex:

       function one(){
         var a =10;
         console.log(a);
         function two(){
           var b=20;
           console.log(b);
         }
         return two;
       }
       one()();

## * Lexical Scope :

* The ability of javascript engine to search for a variable outer scope or global scope if the variable is not present in the local scope is called as lexical scope.

## Arrays:

 * Array is a collection of homogeneous and heterogeneous type of data.
 * Homogeneous stands for same type of data.
 * Heterogeneous stands for different type of data.
 * We can create the array in 2 ways:

    1. Literal Method
    2. Array Constructor Method(should not use)
       
  1. Literal Method :

   * Ex: let colors=["black","pink","orange","green"];

  2. Array Constructor Method(should not use in real time) :

   * Ex: let arr = new Array("black","pink","orange","green");

  * Homogeneous :-
   * Ex: let arr=[10,20,30.40];
  * Heterogeneous :-
   * Ex: let arr=[10,null,undefined,"hello",true];

  * Fetching a value from a Array using index :-
   
   * Ex:

         console.log(arr[1]); //prints value at index 1
  * Array methods:-

    1. Push - Adding element in the last of array.
       * Ex:-

             let arr=[10,20,30.40];
             arr.push(50);   //10,20,30,40,50
         
    2. Pop - Removes element in the last of array.
       * Ex:-

             let arr=[10,20,30.40];
             arr.pop();   //10,20,30,40

    3. Unshift - Adding element in the last of array.
       * Ex:-

             let arr=[10,20,30.40];
             arr.unshift(5);   //5,10,20,30,40
    4. Shift - Remove element in the first of array.
       * Ex:-

             let arr=[10,20,30.40];
             arr.shift();   //10,20,30,40

  * Code to Reverse an array and convert to string :

        let arr = [10,20,30,40,50]
        console.log(arr.reverse());        // reverse array
        console.log(arr.join(""));                     // converts to string
        console.log(arr.indexOf(10));                  // prints indef of value 10
        console.log(Array.isArray);            // prints boolean values checks whether it is an array or not
        console.log(arr.slice(0,2));          // part of array
        console.log(arr.splice(0,2,"hello");  // deletes and replace values in array

    * for in: fetches index

          for (index in arr){
             console.log(index);
          }
      
     * for of: fetches value only

           for (values of arr){
             console.log(values);
           }

     * for each: fetches both index and values.

           let arr=[10,20,30];
           arr.forEach(function(val,index){
             console.log(`${index} is the index of ${val}`);
           });

    * for each: fetches both index and values(arrow function).

           let arr=[10,20,30];
           arr.forEach(val,index)=>
          {
             console.log(val,index);
           });
      
    * Splice :
   
    * Ex:

          let names=["Virat","MSD","Rohit","ABD"];
          names.splice(2,0,"Baber");   // adds value
          names.splice(2,1,"Pandya");  //replace value
          names.splice(1,2);    // deletes value

 ## * Filter(), Map() and Reduce():-

  * **Filter():**

   *  Filter is a built in higher order function, it is used to remove unwanted elements from an array.
   *  Filter will return a new array.
   *  Inside filter should not use arithmetic operators because we compare values.
   *  Ex:

          let num=[10,20,30,40,50,60];
          let result=num.filter((x)=>{
                       return x>30;
          })
          console.log(result);   //40,50,60

 * **Map():**

  * Map is a built-in higher order function it applies the given function to each and every element in an array[one-to-one mapping].
  * Transforms each element where we use arithmetic operators.
  * Ex:

        let num=[1,2,3,4,5];
        let result=num.map((x)=>{
                       return x*2;
          })
          console.log(result);
    
 * **Reduce():**

  * Reduce is a built in higher order function, it takes multiple elements and it reduces it into a single value.
  * Ex:

        let num=[10,20,30,40,50,60];
        let result=num.reduce((acc,val)=>{
                       return acc+val;
          },0)
          console.log(result);
    
* Array Destructuring:

 * Array Destructuring was introduced in ECMAscript 2015(ES6).
 * Array Destructuring means unpacking the values from an array and storing it in a separate variable.
 * Ex:

       let user=["Kanmani",19,"BCOM","Chennai"]
       let [name,age,dept,city]=user
       console.log(name);
       console.log(age);
       console.log(dept);
       console.log(city);

## Objects:

 * Object is a real world entity used to store dat in the form of key & value pair.
 * There are two types to declare an object.
     1. Literal Method.
     2. Object Constructor.

 1. Literal Method:-

   * Ex:

         let user={
                 name:"Kannu",
                 age:19,
                 skills:["Accounts","cooking","Rangoli", "dancing"],
                 address:{
                    city:"Chennai",
                    state:"TN"
                 }
         }
         console.log(user);

 2. Object constructor:

   * Ex :

          let user=new Object({
                 name:"Kannu",
                 age:19,
                 skills:["Accounts","cooking","Rangoli", "dancing"],
                 address:{
                    city:"Chennai",
                    state:"TN"
                 }
         })
         console.log(user);

### * Accessing object properties :

   1. Dot notation
   2. Square brackets

   * Ex:

         let user={
                 name:"Kiran",
                 age:25,
                 address:{
                    city:"Benagluru",
                    state:"Karnataka"
                 }
         }
         // Dot Notation
         console.log(user.age);
         // Square Brackets
         console.log(user["name"];
         console.log(user["address"]["state"]);
     
 ### * Modifying the objects:

   * Ex:

          let user={
                 name:"Yogesh",
                 dept:"CSE",
                 course:"PFS",
         }
         // adding the property
         user.gender="Male";
         console.log(user);
         // updating
         user.name="Sunil";
         user.gender="M";
         console.log(user);
         // deletes
         delete user.dept
         console.log(user);

 * Object Methods:-

  * Ex:

         let user={
                 name:"Yogesh",
                 dept:"CSE",
                 course:"PFS",
         }
         // object methods
         console.log(Object.keys(user));  //returns array of keys
         console.log(Object.values(user));  //returns array of values
         console.log(Object.entries(user));  //returns both array of keys and values

### * Object Sealing and Freezing:

  * Both sealing and Freezing means protecting an object.

* **Sealing:**

 * Whenever the object is sealed we cannot add, delete, but we can update.
 * Synatx:
       Object.seal(object_name);
   
 * Ex:

       let user={
                 name:"Yogesh",
                 dept:"CSE",
                 course:"PFS",
         }
         console.log(user);
         // object sealing
         Object.seal(user)
         // adding
         user.gender="Male";
         console.log(user);
         //updating
         user.name="Sunil";
         console.log(user);
         console.log(Object.isSealed(user))  // returns boolean values

* **Freezing :**

  * Whenever an object is freezed we cannot modify the object(read-only)or immutable.
  * Ex:-
 
        let user={
                 name:"Yogesh",
                 dept:"CSE",
                 course:"PFS",
         }
         console.log(user);
         Object.freeze(user);
        // updating
         user.dept="Civil";   // updation not possible
         console.log(user);
        console.log(Object.isFrozen(user)); // true

 ### * Object Destructuring:

   *  Object Destructuring means unpacking the values from an array and storing it in a separate variable.
   * Ex:

         let user={
                 name:"Yogesh",
                 dept:"CSE",
                 course:"PFS",
         }
         let {name:Name,dept:Dept,course:Course}=user //removes key values
         console.log(Name);
         console.log(Dept);
         console.log(Course);

 ##  Web Storage API:

 * Each and every browser provides in built storage to store data upto 10Mb(text,number,letters,etc..)but not images and videos.
 * There are two types of storages :

    1. Local Storage(Permanent)
    2. Session Storage(Temporary) - if web page is closed memoray will be deleted.

 **1. Local Storage:**

  * To store data.
  * Syntax:

        localStorage.setItem("Key",value);

  * Example:-

        let username="Sunil";
        let email="sunil@gmail.com";
        localStorage.setItem("user",username);
        localStorage.setItem("email",email);

 * To Fetch data:

   * Syntax:

         localStorage.getItem("Key");

   * Example:-

         let username="Sunil";
         let email="sunil@gmail.com";
         localStorage.setItem("user",username);
         localStorage.setItem("email",email);
         let a=localStorage.getItem("user");
         let b=localStorage.getItem("email");
         console.log(a);
         console.log(b);

* Remove Items:

 * To remove particular data

       localStorage.removeItem("email");
 * To clear all the data

       localStorage.clear();
   
 * Ex:

       localStorage.setItem("user",username);
       localStorage.setItem("email",email);
       localStorage.setItem("password",password);
       localStorage.removeItem("email");
       localStorage.clear() // removes all the items

**2. Session Storage:**

  * Ex:

        sessionStorage.setItem("name","yash");
  * Ex :

        sessionStorage.setItem("user",username);
        sessionStorage.setItem("email",email);
        sessionStorage.setItem("password",password);
        sessionStorage.removeItem("email");
        sessionStorage.clear() // removes all the items

## DOM (Document Object Model):-

* DOM is a programming interface provided by the browser that allows javascript to interact with HTML and CSS of a web page.
* Ex:

      <body>
      <h1 id="head">Kanmani</h1>
      <script>
        let head = document.getElementById("head")
        console.log(typeof head);
        head.innerText="Patanjali";
      </script>
      </body>

## BOM (Browser Object Model):-

* BOM allows javascript to interact with browser[outside the page content], like browser windows,location,history etc.
  
* BOM Objects:-

  1. Window (Global Object).
  2. Navigator (Information about browser).
  3. Screen(Info about screen resolution).
  4. History (Browser history).
  5. Location (Info about urls).

* Features of DOM:-

  1. To modify HTML Elements.
  2. To change styles.
  3. To add,delete & edit the elements.
  4. To handle events.

* Note: DOM is inside BOM.

## DOM Tree :

* Whenever the browser loads on HTML elements, browser creates a tree like structure this structure is called *DOM Tree*.
* Ex :-

      <!DOCTYPE html>                                       
      <html>
        <head>
          <meta>
            <title></title>
        </head>
      <body>
         <p>hello</p>
         <h1>Welcome</h1>
      </body>
      </html>

* Tree structure
   
      document
         |____html
           |____head
           |       |____meta
           |       |____title
           |             |___DOM
           |
           |
           |__body
                |____p
                |    |____hello
                |
                |____h1
                      |____Welcome

 ##  DOM Selectors :

 * DOM Selectors are methods provided by javascript to target elements.
 * Types :-

   1. document.getElementById()
   2. document.getElementByClassName()
   3. document.getElementByTagName()
   4. document.querySelector()
   5. document.querySelectorAll()

 ### 1. document.getElementById() :-

 * It is used to target the element based on the id and it returns a single element.
 c

       <body id="body">
         <h1 id="head">Hello</h1>
         <button onClick="change()">Click</button>
       <script>
          function change(){
          let head = document.getElementById("head")
          let body = document.getElementById("body")
            head.innerText="Welcome"
            head.style.color="powderblue"
            head.style.backgroundColor="black"
            body.style.margin="0px"
            body.style.padding="0px"
         }
       </script>
       </body>

### 2. document.getElementByClassName() :-

* It is used to target the multiple elements based on the class name and it returns html collections.
* Ex:-

       <body>
          <h1 class="head">Dharan</h1>
          <h1 class="head">Rossy</h1>
          <h1 class="head">Reshma</h1>
       <script>
          let head = document.getElementByClassName("head")
          head[1].innerText="Roshni"
          head[2].stylecolor="pink"
       </script>
      </body>

### 3. dcument.getElementByTagName() :-

* It is used to target the multiple elements based on the tag name and it returns html collections.
* Ex:-

      <body>
         <h1>HTML</h1>
         <h1>CSS</h1>
         <h1>Javascript</h1>
        <script>
           let head = document.getElementBytagName("h1")
           head[2].innertext="React.js"
        </script>
      </body>

### 4. document.querySelector() :-

* querySelector method is used to target html elements CSS selectors and it returns a single element.
* Ex :-

      <body>
        <h1></h1>
        <script>
          let head = document.querySelector("#head")
          head.style.color="red"
        </script>
      </body>

### 5. document.querySelectorAll() :-

* It is used to target multiple elements using CSS selectors and it returns nodelist.
* Ex :-

      <body>
        <h1 class="head">Hello</h1>
        <h1 class="head">Welcome</h1>
       <script>
         let head = document.querySelectorAll("head")
         head[1].innertext="Bye"
       </script>
      </body>

## Event Handling :-

* Event handling allows us to execute javascript code in response to user action.
* Types of events:

  1. Mouse events :
         click,dbclick,moverover,mouseup,mousedown etc..
     
  2. Keyboard events :
         keydown,keyup,keypress
     
  3. Form events :-
         submit,focus,input etc..
     
  4. Window event :-
         scroll,resize,load etc..

 * There are two ways to handle events
    1. Inline event handler
    2. addEventListener()

 1. Inline event handler :-

        <body>
          <button onClick="a()".onClick="b()">click</button>
        <script>
          function a(){
            console.log("This is task A");
          }
          function b(){
            console.log("This is task B");
          }
        </script>
        </body>

* Drawbacks :

* We cannot attach events having same event name.
* It maxes both HTML and JS code.

## Add Eventlistener :

* It provides flexible way to handle events.
* We can attach multiple events for a single element.

### * Syntax :-

     element_name.addEventListener("event",function)

     <button id="btn">click</button>
     <script>
        let button = document.getElementById("btn")
        button.addEventListener("click",()=>{
        console.log("This is task B")
       })
     </script>

 ### Keyboard Events :

 * **Keydown :**

       <body>
          <input type="text" id="user">
        <script>
          let input=document.getElementById("user")
          input.addEventListener("keydown",(e)=>{
            if (e.key=="a"){
               console.log("Move left")
            }else if(e.key=="s"){
               console.log("Move right")
            }else if(e.key=="w"){
               console.log("Move up")
            }else if(e.key=="d"){
               console.log("Move down")
            }else{
              console.log("Invalid key")
            }
          }
       </script>
       </body>

* ***NOTE :- Keydown prints the value in console but not keyup. Keypress is depricated(older one).***

### Form Events :-

* By default form will reload the page.
* It tries to connect to a server.
* To stop this behaviour we prevent default method :-

       <form action=" " id="handleForm">
       <input type="text" id="user">
       <button>click</button>
       <script>
       let form = document.getElementById("handleForm")
       form.addEventListener("submit"(e)=>{
          e.preventDefault()
          let user = document.getElementById("user").value
          console.log(user);
       })
      </script>

## Event Bubbling :-

 *  Event Bubbling is a default behaviour in DOM where an event starts from targeted element and bubbles through its parent element.
 *  To stop the event buubling we make use of *stopPropagation()*.
 *  Ex :-

        <div id="parent" style="padding:20px ; background-color:lightblue;">
          <button id="child">Click</button>
        </div>
          <script>
             let parent = document.getElementById("parent")
             let child = document.getElementById("child")
             parent.addEventListener("click",()=>{
             alert("Parent clicked...");
             })
            child.addEventListener("click",(e)=>{
            e.stopPropagation()
            alert("child clicked...")
           })
        </script>

## Promises :-

* Promises are used to handle asynchronous task like making API calls (fetching data from an API).
* Ther are 3 states in promises
   1. pending
   2. fulfilled - then()----| ( similar as exception handling in python like try()
   3. reject  - catch()-----|       catch() )

* **API's :**
   1. https://api.github.com/users
   2. https://dummyjson.com/products

* Ex:-

      <script>
        fetch("https://dummyjson.com/products")
        .then(x=>x.json())
        .then(y=>console.log(y))
        .catch(err=>console.log("Something went wrong"));
      </script>

  ***NOTE : If console is used it will not show the value it will print response.***

* **Synchronous:-**

* Synchronous blocks the other task to get executed . It is a line by line execution.
* Promises are used to execute asynchronous operations.

* **Asynchronous:-**

* Executes based on the events no line by line execution.

## * this Keyword:

- `this` refers to the object that is currently executing the code.
- Value of `this` depends on how the function is called (not where it is defined).

1. Global context :

  - Ex:
```
console.log(this); // window object (in browser)
```

2. Inside normal function :

  - `this` refers to window object (in non-strict mode) or undefined (strict mode).
  - Ex:
```
function show(){
  console.log(this);
}
show(); // window
```

3. Inside object method :

  - `this` refers to the object which called the method.
  - Ex:
```
let user={
  name:"Poorvi",
  greet(){
    console.log(this.name);
  }
}
user.greet(); // Poorvi
```

4. Inside Arrow function :

  - Arrow function does not have its own `this`.
  - It takes `this` from its lexical (surrounding) scope.
  - Ex:
```
let user={
  name:"Poorvi",
  greet:()=>{
    console.log(this.name); // undefined, this = window/outer scope
  }
}
user.greet();
```

- ***NOTE : This is a very common interview trap question - normal function vs arrow function behaviour of `this`.***

---

## Closures (in depth):

- A Closure is formed when a function remembers and continues to access variables from its outer(lexical) scope even after the outer function has finished executing.
- Closures are formed every time a function is created.

- Ex: Counter using Closure

```
function counter(){
  let count=0;
  return function(){
    count++;
    console.log(count);
  }
}
let increment=counter();
increment(); //1
increment(); //2
increment(); //3
```

- Why Closures are used :

  1. Data hiding/Data privacy (private variables)
  2. Function currying
  3. Memoization
  4. setTimeout with loop (to preserve variable value)

- Ex: Data privacy using closure
```
function bankAccount(){
  let balance=1000;   // cannot be accessed directly from outside
  return {
    deposit(amount){
      balance+=amount;
      console.log(balance);
    },
    withdraw(amount){
      balance-=amount;
      console.log(balance);
    }
  }
}
let account=bankAccount();
account.deposit(500);  //1500
account.withdraw(200); //1300
```

---

## call(), apply() and bind():

- These 3 methods are used to manually set the value of `this` inside a function.

1. **call()** :

  - Invokes the function immediately, arguments passed one by one(comma separated).
  - Ex:
```
function greet(city){
  console.log(this.name+" from "+city);
}
let user={name:"Poorvi"};
greet.call(user,"Bengaluru");
```

2. **apply()** :

  - Invokes the function immediately, arguments passed as an array.
  - Ex:
```
greet.apply(user,["Bengaluru"]);
```

3. **bind()** :

  - Does not invoke immediately, returns a new function which we can call later.
  - Ex:
```
let newFunc=greet.bind(user,"Bengaluru");
newFunc(); // called later
```

- ***NOTE : call/apply invoke immediately, bind returns a copy of function for later use.***

---

## Event Loop, Call Stack & Web APIs:

- Javascript is single threaded - it can execute only one task at a time.
- To handle asynchronous tasks(setTimeout, API calls, events) javascript uses Event Loop.

- Components :

  1. **Call Stack** - Where javascript executes code line by line(synchronous code).
  2. **Web APIs** - Browser provided features(setTimeout, DOM events, fetch) that run outside the call stack.
  3. **Callback Queue(Task Queue)** - Stores callback functions(setTimeout, DOM events) waiting to enter call stack.
  4. **Microtask Queue** - Stores promise callbacks(.then, .catch, async/await). Has higher priority than callback queue.
  5. **Event Loop** - Continuously checks if call stack is empty, if empty it pushes tasks from microtask queue first, then callback queue.

- Ex:
```
console.log("1");

setTimeout(()=>{
  console.log("2");
},0);

Promise.resolve().then(()=>{
  console.log("3");
});

console.log("4");

// Output : 1 4 3 2
```

- ***NOTE : Even with 0ms delay, setTimeout goes to callback queue and executes after all synchronous code and microtasks(promises) are done.***

---

## Prototype & Prototypal Inheritance:

- Every javascript object has a hidden internal property called `[[Prototype]]`, accessible via `__proto__`.
- When we try to access a property/method not present in the object, javascript searches for it in the prototype chain.

- Ex:
```
let animal={
  eats:true
}
let dog={
  barks:true
}
dog.__proto__=animal;
console.log(dog.eats); // true (inherited from animal)
```

- **Object.create()** - creates a new object with given object as its prototype.

```
let animal={
  eats:true
}
let dog=Object.create(animal);
dog.barks=true;
console.log(dog.eats); //true
```

- Function's prototype :

```
function Person(name){
  this.name=name;
}
Person.prototype.sayHello=function(){
  console.log("Hello "+this.name);
}
let p1=new Person("Poorvi");
p1.sayHello(); // Hello Poorvi
```

---

## Async/Await:

- Async/Await is a modern way to write asynchronous code that looks synchronous(easier than .then chaining).
- `async` keyword before a function makes it return a promise.
- `await` keyword pauses the execution until the promise is resolved/rejected.

- Ex:
```
async function getData(){
  let response = await fetch("https://dummyjson.com/products");
  let data = await response.json();
  console.log(data);
}
getData();
```

- Error handling in async/await :

```
async function getData(){
  try{
    let response = await fetch("https://dummyjson.com/products");
    let data = await response.json();
    console.log(data);
  }catch(err){
    console.log("Something went wrong",err);
  }
}
getData();
```

- ***NOTE : await can only be used inside an async function.***

---

##  == vs === (Equality & Type Coercion):

- `==` (loose equality) - compares values only, converts type if different(type coercion).
- `===` (strict equality) - compares both value and type, no conversion.

- Ex:
```
console.log(5=="5");   // true (type converted)
console.log(5==="5");  // false (different type)
console.log(null==undefined); // true
console.log(null===undefined); // false
```

- ***NOTE : Always prefer === in real projects to avoid unexpected bugs.***

---

## Debouncing & Throttling:

- Both are used to control how many times a function executes for repeated events(scroll, resize, search input, etc).

1. **Debouncing** :

  - Executes function only after a certain delay has passed since the last call.
  - Used in : Search bar, Auto-save.

```
function debounce(func,delay){
  let timer;
  return function(...args){
    clearTimeout(timer);
    timer=setTimeout(()=>{
      func(...args);
    },delay);
  }
}
```

2. **Throttling** :

  - Executes function at most once in a given time interval, regardless of how many times event is triggered.
  - Used in : Scroll events, Button click(prevent multiple submit).

```
function throttle(func,limit){
  let flag=true;
  return function(...args){
    if(flag){
      func(...args);
      flag=false;
      setTimeout(()=>{
        flag=true;
      },limit);
    }
  }
}
```

---

## Spread & Rest Operators:

- Both use the same syntax(`...`) but work opposite to each other.

1. **Spread Operator** - Unpacks/expands elements from array or object.

```
let arr1=[1,2,3];
let arr2=[...arr1,4,5];
console.log(arr2); //1,2,3,4,5

let obj1={name:"Poorvi"};
let obj2={...obj1,age:22};
console.log(obj2);
```

2. **Rest Operator** - Packs/collects multiple values into a single array. Used in function parameters.

```
function sum(...nums){
  return nums.reduce((acc,val)=>acc+val,0);
}
console.log(sum(1,2,3,4)); //10
```

---

## Optional Chaining(?.) & Nullish Coalescing(??):

1. **Optional Chaining(?.)** - Avoids error when accessing a property of null/undefined, returns undefined instead of throwing error.

```
let user={
  address:{
    city:"Bengaluru"
  }
}
console.log(user?.address?.city); //Bengaluru
console.log(user?.contact?.phone); //undefined(no error)
```

2. **Nullish Coalescing(??)** - Returns right side value only if left side is null or undefined(not for other falsy values like 0, "").

```
let a=null;
console.log(a??"Default"); //Default

let b=0;
console.log(b??"Default"); //0 (because 0 is not null/undefined)
console.log(b||"Default"); //Default (|| treats 0 as falsy too - difference to remember)
```

## Currying :

- Currying is a technique where a function with multiple arguments is converted into a series of functions, each taking a single argument.
- Used to create reusable, specific versions of a function.

- Normal function :
```
function add(a,b,c){
  return a+b+c;
}
console.log(add(1,2,3)); //6
```

- Curried function :
```
function add(a){
  return function(b){
    return function(c){
      return a+b+c;
    }
  }
}
console.log(add(1)(2)(3)); //6
```

- Curried function using Arrow function :
```
let add=(a)=>(b)=>(c)=>a+b+c;
console.log(add(1)(2)(3)); //6
```

- Practical use case : Reusable specific function
```
function discount(percent){
  return function(price){
    return price-(price*percent/100);
  }
}
let tenPercentOff=discount(10);
console.log(tenPercentOff(500)); //450
console.log(tenPercentOff(1000)); //900
```

---

## Memoization:

- Memoization is an optimization technique where we store(cache) the result of expensive function calls and return the cached result when the same input occurs again.
- Uses Closure to store the cache.

- Ex: Without memoization(slow for repeated calls)
```
function square(n){
  console.log("Calculating...");
  return n*n;
}
console.log(square(5)); //Calculating... 25
console.log(square(5)); //Calculating... 25 (calculated again)
```

- Ex: With memoization
```
function memoizedSquare(){
  let cache={};
  return function(n){
    if(n in cache){
      console.log("From cache");
      return cache[n];
    }
    console.log("Calculating...");
    cache[n]=n*n;
    return cache[n];
  }
}
let square=memoizedSquare();
console.log(square(5)); //Calculating... 25
console.log(square(5)); //From cache 25
console.log(square(6)); //Calculating... 36
```

- ***NOTE : Memoization is commonly used in Dynamic Programming and React(useMemo, useCallback).***

---

## Polyfills:

- A Polyfill is a piece of code(usually a function) that implements a feature which is not natively supported, or to manually re-implement built-in methods to show understanding of how they work internally.
- Frequently asked in coding rounds : "Write a polyfill for map/filter/reduce/bind".

1. **Polyfill for map()** :
```
Array.prototype.myMap=function(callback){
  let result=[];
  for(let i=0;i<this.length;i++){
    result.push(callback(this[i],i,this));
  }
  return result;
}

let arr=[1,2,3];
console.log(arr.myMap((x)=>x*2)); //2,4,6
```

2. **Polyfill for filter()** :
```
Array.prototype.myFilter=function(callback){
  let result=[];
  for(let i=0;i<this.length;i++){
    if(callback(this[i],i,this)){
      result.push(this[i]);
    }
  }
  return result;
}

let arr=[1,2,3,4,5];
console.log(arr.myFilter((x)=>x>2)); //3,4,5
```

3. **Polyfill for reduce()** :
```
Array.prototype.myReduce=function(callback,initialValue){
  let acc=initialValue;
  for(let i=0;i<this.length;i++){
    acc=callback(acc,this[i],i,this);
  }
  return acc;
}

let arr=[1,2,3,4];
console.log(arr.myReduce((acc,val)=>acc+val,0)); //10
```

4. **Polyfill for bind()** :
```
Function.prototype.myBind=function(context,...args){
  let fn=this;
  return function(...newArgs){
    return fn.apply(context,[...args,...newArgs]);
  }
}

function greet(city){
  console.log(this.name+" from "+city);
}
let user={name:"Poorvi"};
let boundFunc=greet.myBind(user,"Bengaluru");
boundFunc(); //Poorvi from Bengaluru
```

- ***NOTE : While writing polyfills, always use `this` to refer to the array/function it is called on(since we attach it to prototype), and use a normal function(not arrow function) so `this` binds correctly.***
      
