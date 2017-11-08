## callbacks
`var calculateArea = function (a,  b) {`<br/>
`var area = a * b;`<br/>
`console.log("Calculated area is equal to: " + area);`<br/>
`return area;`<br/>
`}`<br/>
`var calculatePerimeter = function (a, b) {`<br/>
`var perimeter = 2 * (a + b);`<br/>
`console.log("Calculated perimeter is equal to: " + perimeter);`<br/>
`return perimeter;`<br/>
`}`<br/>
`function rectangleCalculation(a, b, calculateFunction){`<br/>
`console.log("Input parameters: a = " + a + "; b = " + b + ";");`<br/>
`calculateFunction(a, b);`<br/>
`}`<br/>
`rectangleCalculation(5, 4, calculateArea);`<br/>
`rectangleCalculation(5, 4, calculatePerimeter);`<br/>


callback functions:

   In the above example `rectangleCalculation(5, 4, calculateArea);` is invoking a function called `rectangleCalculation` with options 5,4,`calculateArea`. 
  
   In the function `rectangleCalculation` there is a parameter for the callback function i.e `calculateFunction`.

   The parameter `calculateFunction` is a callback function where it calls back a function called `calculateArea` which has been passes as a callback function.
