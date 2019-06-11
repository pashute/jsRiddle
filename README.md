# jsRiddle
Answers to Dmitry Barnovskiy's javascript riddles
See [Dmitry Barnovskiy's web log](http://dmitry.baranovskiy.com/post/91403200)

## Riddle number 1

    if (!("a" in window)) {
    var a = 1;
    }
    alert(a);
    
### Answer 1

**Result:** Alerts: `Undefined`

`window` is the browser's "display" object.     
Every variable globally defined (not in a var) is inside the window object.     
       
`"a"` is a constant string object, so it is defined in the window.     
Defining a function locally is when a variable is defined with the `var` keyword INSIDE a function. 
`var a` is defined globaly, although it is defined within an `if` block, it is NOT defined in a function, therefore it does not lose its value outside the `if` block. 

    if (!("a" in window)) {  // equivalent of if(!true) {  - always returns false
      var a = 1; // would be defined globally when the clause would be true. But this does not happen. 
    }
    alert(a);  // so a is undefined
    
 
   
   ## Riddle number 2

     here goes
    
### Answer 2

To be continued...
