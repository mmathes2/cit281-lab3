# cit281-lab3
## Practice refactoring JavaScript code to use more modern syntax
## Practice destructuring an object
// TODO Part 2: Create vin and year variables using object destructuring
// Comment out the original code using single line comments
/*
   Important: The instructions and the following code mix vin/year and
   make/model. You can replace car.make and car.model in the following code
   with either vin and year or make and model.
*/

// Declare a normal function that returns formatted car info
function getCarMakeModel(car) {
    return car.make + " " + car.model;
}
## Practice converting normal functions into arrow function expressions
// TODO Part 3: Create arrow function expression getCarMakeModelImplicit
// and template literal that returns the same formatted car info as
// getCarMakeModel(). The arrow function MUST NOT use a return 
// statement (use implicit return)
// Include a console.log statement similar to getCarMakeModel,
// but increment the number from 0 to 1.

// TODO Part 4: Create arrow function expression getCarMakeModelExplicit
// and template literal that returns the same formatted car info as
// getCarMakeModel(). The arrow function MUST use a return 
// statement (use explicit return)
// Include a console.log statement similar to getCarMakeModel,
// but increment the number from 0 to 2.

// TODO Part 5: Create arrow function expression getCarMakeModelDestructure
// and template literal that returns the same formatted car info as
// getCarMakeModel(). The arrow function MUST destructure the 
// car properties, which will also require using an explicit return.
// Include a console.log statement similar to getCarMakeModel,
// but increment the number from 0 to 3.
## Examine using for..in  syntax with objects
// TODO Part 6: Study the following code that will list all 
// properties of an object using for..in syntax. The
// listing will include inherited properties, so the
// hasOwnProperty() method is used to only list properties
// defined in the current object
for (let prop in car) {
    if (car.hasOwnProperty(prop)) {
        console.log(prop);
    }
}

// Display all values of an array
const primes = [2,3,5,7,11];
for (let index = 0; index < primes.length; index++) {
    console.log(primes[index]);
}
## Practice using for..of syntax with arrays
// TODO Part 7: Display all array values using for..of syntax
// Comment out the original for loop code using single line comments
## Practice creating a Node.js compatible code module using module.exports
// TODO Part 9: Add the reverseString function to the module.exports object
// for import using require()
## Practice importing a Node.js compatible code module using require
// TODO Part 11: Import reverseString() and concatenateString()
// functions from lab-03-module.js module using require()
## Examine code using the spread operator
// TODO Part 8: Reference the following website to use the spread operator
// to reverse the string for reverseString(str) function. Comment out the
// original return line of code.
// https://betterprogramming.pub/5-ways-to-reverse-a-string-in-javascript-466f62845827
function reverseString(str) {
    return str.split("").reverse().join("");
}
