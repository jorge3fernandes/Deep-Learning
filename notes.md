
Basic Java Script


Data types:

strings
booleans
number, etc

typeof() - tells you which datatypes you're using


Variables:

var myName = "Jorge";

when changing or renaming we don't need the var prefix. that is used only when initializing variables.

How to best label your variables:

Give variable meaningful names that describes what is inside of them.
don't use actual function/keywords as name
can't be with a number.
Can't use - in names
use camel case


Strings:

Can combine with '+' sign.

Word property to get length of string - word.length

how to slice and dice strings. name.slice(x,y) where x is the first position starting at 0 and y means last position but not including the actual index. 
in order to know how many characters we will endup with, we just do y-x to get the count.

using name.toUpperCase() and name.toLowerCase()

Arithmetic:

module -  var e = 9 % 6 which is equal to 3.
use parenthesis to make it clear which operations is happening first.

how to increment/decrememnt values

x++; increment by 1
x--; decrement by 1

x+=2; increment by 2
x-=2; decrement by 2

x+=y; increment by y
x-=y; decrement by y

x/= 3; divide by 3


tricky question:
var x = 3;
var y = x++; // looks like x is assigned before being incremented
y += 1;

y is equal to 4.

Functions:

general form - 
function getMilk(input- can be left black){
	//do something;
	retun result;
}


Intermediate

Generate random numbers

var n = Math.random // only generates numbers between 0 and 0.999999999999999...

// so if we want to get get a randon number between 0 and 6, we would simply do
number = n * 6
number = Math.floor(number)

// remeber the this will not include 6. if we want
// read documentation on it.

Control flow

if(x === y){
  // do something
} else if (){
// do something
}else{
// do something
}

=== is equal to. checks for value and type
!== not equal to
== only check for value.

&& means and 
|| means or

Array

var siblings= ["jorge","jove","beto","jorgetty","betinha","joanzim",]

siblings[1] // "Jove"

siblings.includes("jorge") // True - a boolean

***************************code exercise********************************
var siblings= ["jorge","jove","beto","jorgetty","betinha","joanzim"]

var name = prompt("Are you my sibling? Enter you first name to check.")

if(siblings.includes(name)){
    alert("Hey! What's up. Let's do someting fun!")
} else{
    alert("You're not one of my siblings! Get out!")
}
************************************************************************

Adding items to array
array.push() - adds new item to the in the last position

removing items from array
array.pop()


While loop

var i;

while (i < 2){
  console.log(i);
  i++;
}

for loops:

for(start; end; increment){
  // do something;
}

for(var i = 0; i<2; i++){
  //do something;
}

When to use while loops versus for loop. while loops are checking for states(while something is true), and the for loops is looking to iterate.

####################### Tips on how to learn ############################
Retrieval is How you learn


Adding JavaScritp to Websites

DOM - Document Obejct Model

Practice element.querySelector(). Need to really understand this how to select specific elements and change styles. This piece is foundational.
Check out the DOM style documentatoin.

Separation of files:
HTML is for content only, CSS is for style only, and JS is for behavior;

using the add "document.querySelector("button").classList.add() would allows us to add the style for a class using css, but toggle it on and off using javaScript by adding the class and removing it.
getAttribute() vs setAttribute() - understand and practive
