CLOSURES
Closures are function that used locally but has access to external function's variables.
It has access to its own scope, outer function's variable and has access to global variables.
It can also access the outer Function's parameters and call them directly.

Example:
 function data(name,age)
 {
     var n="your name";
     var a="age";                       // local variable created by function data ()
     function fulldata()            // this function has access to outer function's 
                                       variable including parameters.
     {
       return n+"n"+Name+a+":"+age;  // uses variable that declared in parent function
         
     }
     return fulldata();
 }
 data("john","36")
 
 -  Even after the outer function has returned, the inner function still has access to outer 
    function's variables.
-   closures store references to outer function's variable not the actual values.

References:
https://developer.mozilla.org
http://eloquentjavascript.net/
http://stackoverflow.com/