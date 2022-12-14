# Use-getters-and-setters-to-Control-Access-to-an-Object
Use getters and setters to Control Access to an Object
Problem Explanation
Getters and setters are critical parts of a class/object. They allow you to control their attributes from the outside. They will become more prominent when you get started with the Object-Oriented Programming unit (coming up!). For now, this exercise shows you how to manipulate them with ES6.

Hints
Hint 1
Create the class, Thermostat. You’re going to put your constructor, getter, and setter in here.

Hint 2
Give the constructor a parameter (which you can name anything you want). Set the parameter to an attribute of the same name. Remember, you are initially setting things in Fahrenheit temperature.

Hint 3
Create a get method that converts the Fahrenheit attribute to Celsius. Use the formula given to you.

Hint 4:
Create a set method of the same name as the get method. It should have a parameter that accepts celsius temperature. Convert it to fahrenheit, and set it to the attribute.

Solutions
Solution 1 (Click to Show/Hide)
class Thermostat {
  constructor(fahrenheit) {
    this.fahrenheit = fahrenheit;
  }
  
  get temperature() {
    return (5 / 9) * (this.fahrenheit - 32);
  }
  
  set temperature(celsius) {
    this.fahrenheit = (celsius * 9.0) / 5 + 32;
  }
}
