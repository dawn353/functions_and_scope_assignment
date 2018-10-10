# Function Exercies
_NOTE:_ I am not asking for a specific ES syntax, but please note that you need to be able to do both.

1. What will the following code log? Why?
  ```js
let greeting = 'hi'

function hello(){
  greeting = 'bye'
}

hello()
console.log(greeting)

  ```
  it will log bye because the function is being called right above the console.log line

 2. Write a function that returns the largest of two numbers. If they are equal, return the second one.

 const returnGreater = (num1,num2) => {
   if (num1 < num2){
     console.log(num2)
   }
   else if (num2 = num1){
     console.log(num2)
   }
   else{
     console.log(num1)
   }
 }

 returnGreater(2,5)



 3. Write a function named getDogAge that takes one argument: a dog's age in human years. The function returns the dog's age in dog years. The conversion rate is 1 human year to 7 dog years.

    * Call the function and log the result.


    const getDogAge = (age) => {

    return age + 7

    }





    getDogAge(19)








4. Create two functions that calculate properties of a circle, using the definitions [here](http://math2.org/math/geometry/circles.htm)

  * Create a function called calcCircumfrence that takes the radius as an argument and return the circumference. Call the function and log the circumference:
  * Create a function called calcArea that takes the radius as an argument and returns the area.

Create a third function circleProps that takes the radius as an argument, calls the two other functions, and logs the area and circumference. The output should look like this:

"The circumference is ___".

 "The area is ___".




 let R = 2

 const calcCircumfrence = () => {

 return Math.PI * R
 }




 const calcArea = () => {
 return Math.PI*R*R
 }






 const circleProps = () => {
 console.log("the circumference is " + calcCircumfrence())
 console.log("the area is " + calcArea() )
 }




 circleProps()









5. Make a temperature converter. Use google to find the conversion formulas.

  * Create a function called celciusToFahrenheit that takes a temperature in Celsius and returns it in Fahrenheit.
  * Create a function called fahrenheitToCelcius that takes a temperature in Fahrenheit and returns it in Celsius.
  * Create a function called convertTemperature that takes two arguments: a temperature and a string. If the string is 'C', use fahrenheitToCelcius to return the temperature to Celsius. If the string is 'F', use celciusToFahrenheit to convert the temperature to Fahrenheit.





  const celciusToFahrenheit = (C) => {
    return (C * (9/5)) + 32
  }

  const fahrenheitToCelcius = (F) => {
    return (F - 32) * 5/9
  }


  const convertTemperature = (num,temp) => {
    if (temp === "C" ){
     return  celciusToFahrenheit(num)
    } else if (temp === "F") {
      return fahrenheitToCelcius(num)
    } else{
      console.log("enter F or C")
    }
  }


  convertTemperature(78, "C")








6. The Calculator:

  * Write a function `square` that returns the square of a number.
  * Write a function `half` that returns half the value of a number.
  * Write a function `percentOf` that takes two numbers. Calculate what percent the first number is of the second number, and return the result as a string. For example, 2 is 50% precent of 4, so the function returns '50%'.
  * Write a function called `areaOfCircle` that takes one argument (the radius), and return the area of a circle with that radius.
  * Bonus: Round the result so there are only two digits after the decimal.
  * Write a function doStuff that takes one argument (a number) and does the following (using the functions you wrote earlier):
      1. Calculates and saves the square of the number.
      2. Calculates and saves half the value of the result of #1.
      3. Calculate the area of a circle with the result of #2 as the radius.
      4. Calculate and returns the percentage the squared result (#1) is of the area (#3)


      const square = (num) => {
      return num * num
      }

      const half = (num) => {
        return num / 2
      }


      const percentOf = (num1,num2) => {
        return Math.round(num1 * num2)/ 100
      }

      const areaOfCircle = (num) => {
      return Math.round(Math.PI * (num * num))
      }

      console.log(areaOfCircle(7))












7. Write a function `arraySum` that takes in one argument and returns the sum of all the elements.
