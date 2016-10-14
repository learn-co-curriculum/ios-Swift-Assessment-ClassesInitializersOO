# iOS Assessment on Swift Classes, Structs, Initializers, and OOP
A short assessment to test a student's comprehension of basic object orientation.
The student may use a ViewController or a Playground file

## Instructions

### 1. Create the `Pet` class
1. Create a `Pet` class.
2. Declare a `name` property of type `String`

3. Declare and define a default and designated initializer for the class
  * The designated initializer should include a `name` argument and assign the value to the `name` property
  * The default initializer should set `"Jane Doggy"` as the default value

### 2. Create an enum for each kind of Pet `PetType`
1. This enum should have three cases `dog`, `cat` and `bird`

### 3. Create an enum for each pets `Condition`.
1. This enum should have three cases `sick`, `healthy` and `critical`

### 4. Complete the Pet class
1. Declare an instance property named `condition` property of type `Condition`
2. Declare an instance property named `type` property of type `PetType`
3. Set the default value for `condition` to `healthy` (at the point of declaration)
4. Change the designated initializer to also accept an argument called `type` of `PetType`
5. Update the default initializer to assign the value `.dog` to `type`.

### 5. Create the `Vet` class
1. Create the function `treat(_:)` that takes one argument named `pet` of type `Pet`
  * This function should check the pet's condition.
  * If the pet is healthy the vet should do nothing but print "This pet is doing well. Good Job".
  * If the pet is `sick` the vet should change the pet's condition to `healthy`
  * If the pet is  `critical` the vet will need a surgeon. You will define this class next

### 6. Create the `Surgeon` class  
1. The `Surgeon` class should inherit from the `Vet` class
2. Declare a function `performSurgery` that takes an argument of type `Pet`. This function should change a pet's condition from `critical` to `sick`
3. Override the `treat` function and call the `performSurgery`

### 7. Declare a `Hospital` class
1. The `Hospital` class should have a single class function called `referSurgeon` that returns a Surgeon object

### 8. Complete the `Vet` class
1. In the `Vet` class, if the pet being treated is in critical condition you will need a surgeon. Create a new variable in the treat funtion that's assigned to the return of the `referSurgeon` function
2. Use this variable which should be of type `Surgeon` to treat the pet

### 9. Create an `Owner` struct
1. Declare an instance property named `pet` of type optional `Pet`
2. Declare and define a designated initializer for this struct
3. Declare and define a function `takeCare(of:)` that takes in one argument named `pet` of type `Pet`. This funcion checks the pet's condition. If the pet is sick in any way, a vet instance should be initialized/instantiated and should treat the pet.

### 10. Create an `AdoptionClinic` struct
1. Declare a empty array called `strays` of type `Pet`array
2. Create a few random `Pet` objects
3. Declare and define a default initializer that populates the strays array with the random pets you created
4. Declare and define a function `allowAdoption` that returns an optional Pet
  * This function should remove the pet it returns from the `strays` array

### 11. Create instances of classes in the `ViewController.swift` or `.playground` file
  * Create an `Owner` object
  * Create an `AdoptionClinic` object
  * Use the `AdoptionClinic` object to add a pet to the `Owner` object.
  * Call the `takeCareOfPet` method on the `Owner` object
