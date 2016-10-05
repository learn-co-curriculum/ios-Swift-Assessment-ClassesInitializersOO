# iOS Week 2 Objective-C Assessment
A short assessment to test a student's comprehension of basic object orientation. 

## Instructions


### 1. Create the `Pet` class
1. Create a `Pet` class.

2. Declare a `name` property of type `String` 

3. Declare and define a default and designated initializer for the class
  * The designated initializer should include a `name` argument and assign the value to the `name` property
  * The default initializer should set `"Jane Doggy"` as the default value

4. Declare and define a `printPetSound()` function  that takes one argument of type `String`
  * The method should print the `String` argument to the console

### 2. Create the `Person` class

1. Declare a `pet` property of type `Pet`

### 3. Create instances of both classes in the `AppDelegate`

1. Create two variables in the `application:didFinishLaunchingWithOptions()` method of the `AppDelegate` class

  * Declare a variable of type `Person` using the designated initializer
  
  * Declare a variable of type `Pet` using the default initializer
  
  * Assign the value of the `Pet` object to the `pet` property of the `Person` object
  
  * Call the `printPetSound()` method on the `pet` property of the `Person` object
