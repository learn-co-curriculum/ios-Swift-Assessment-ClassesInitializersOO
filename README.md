# iOS Week 2 Swift Assessment
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

### 3. Create an enum for each pets `Condition`. 
1. This enum should have two cases `sick` and `healthy`

### 2. Create the `Person` class

1. Declare a `pet` property of type `Pet`

2. Declare and define a  `adoptPet()` function 

### 3. Create a  `Vet` struct

1. Declare a `patients` property of type `Pet` array

2. Declare and define a `treatPatient` function that takes a variable `patient` of type string as an argument
   * The `treatPatient` function should change that pet's condition from sick to healthy.
   * This function should remove that pet from the patients array

### 3. Create instances of both classes in the `ViewController.swift`

1. Create two variables in the `viewDidLoad` method of the `ViewController` class

  * Declare a variable of type `Person` using the designated initializer

  * Declare a variable of type `Pet` using the default initializer

  * Assign the value of the `Pet` object to the `pet` property of the `Person` object

  * Call the `printPetSound()` method on the `pet` property of the `Person` object


