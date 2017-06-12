## Scope, hoisting and compartmentalization

### Answer the following:
In you own words, explain the concepts of scope, hoisting, compartmentalization.

Scope is the constrants in which you can see variables and functions. You can have global scope--var and func viewable to all, or local scope--var and functions available to that area only.

Hoisting is what the JS program does to variables and declared functions (not function expressions). It moves the declaration of these items to the top of whatever scope they are in (vars and functions defined witin a function are moved to the top of that function, if defined globally are moved to the top of the file)

compartmentalization: keeping your functions and variables confined to one area (function)

### Provide examples for all three, below:

#### Scope:

var x = 0;

function whatIsX(){
  var x = 1;
  console.log(x);
}
console.log(x);

in this example x is defined globally as 0, and locally as 1. inside the function x will be 1, but the console.log outside the function will return 0.



#### Hoisting:

some lines of code here......
var x = 0;

var variableName = someFunction() {
  var y;
  if (y = 0){
    var number = 5;
  };

  function findY() {
    if (var y = 0) {
      console.log("Y does not exist");
    }
  }
}

In the code above, var x is moved by the program to the top of the file. Function findY is also moved to the top of the file. These are stored in memory and available when the computer runs across them the next time it runs through the code (it runs through twice, once to pull var and funct to top of screen)

#### Compartmentalization:
keeping variables in local scope so that they are not accessible to other programs or functions. This means that you could have two variables named the same thing, but that's not recommended.
