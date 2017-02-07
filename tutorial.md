

A closure is an inner function that has access to the outer function’s variables—scope chain. The closure has three scope chains: it has access to its own scope, 
it has access to the outer function’s variables, and it has access to the global variables.

The inner function has access not only to the outer function’s variables, but also to the outer function’s parameters. Note that the inner function cannot call the outer function’s 
arguments object, however, even though it can call the outer function’s parameters directly.


function makeFunc() {
  var name = "Mozilla";
  function displayName() {
    alert(name);
  }
  return displayName;
}

var myFunc = makeFunc();
myFunc();


MDN link
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures


W3schools
http://www.w3schools.com/js/js_function_closures.asp


javascript tutorial
http://javascript.info/tutorial/closures



youtube link
https://www.youtube.com/watch?v=71AtaJpJHw0