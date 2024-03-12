# Lab - Explore Python Classes
Objectives
Part 1: Launch the DEVASC VM
Part 2: Review Functions, Methods, and Classes
Part 3: Define a Function
Part 4: Define a Class with Methods
Part 5: Review the circleClass.py Script
Background / Scenario
This lab is designed to help you review Python methods, functions, and classes. You'll create a class and instantiate it with various values. Additionally, you'll review the Circle class example used in the course.

Required Resources
1 PC with the operating system of your choice
Virtual Box or VMWare
DEVASC Virtual Machine
Instructions
Part 1: Launch the DEVASC VM
If you have not already completed the Lab - Install the Virtual Machine Lab Environment, do so now. If you have already completed that lab, launch the DEVASC VM now.

Part 2: Review Functions, Methods, and Classes
In this part, you'll review the difference between functions and methods, as well as the basic structure of a class.

Step 1: What is a function?

A function is an independently defined block of code that is called by name.

# Define the function
def functionName:
  ...blocks of code...
# Call the function
functionName()

Step 2: What is a method?

A method cannot be called by itself; it is dependent on the object in which it is defined.

# Define the class
class className
 # Define a method
 def method1Name
    ...blocks of code
 # Define another method
 def method2Name
   ...blocks of code
 # Define yet another method
 def method3Name
   ...blocks of code
# Instantiate the class
myClass = className()
# Call the instantiation and associated methods
myClass.method1Name()
myClass.method2Name()
myClass.method3Name()

Part 3: Define a Function
In this part, you'll define a function with arguments and then call the function.

Step a: Define the function myCity with the argument city for city name.

Step b-d: Call the function myCity passing it different values for city.

def mycity(city):
    print("I live in " + city + ".")

mycity("New York")
mycity("Los Angeles")
mycity("Chicago")



Part 4: Define a Class with Methods
In this part, you'll define a class, use the __init__() function to define a method for the class, and then create instances of the class.

Step 1: Define and then instantiate a class with the __init__() method.
class Location:
    def __init__(self, name, country):
        self.name = name
        self.country = country
   
loc = Location("Ozzie", "Dominican Republic")
loc.myLocation()

Step 2: Add a method to the Location class.
class Location:
    def __init__(self, name, country):
        self.name = name
        self.country = country
    def myLocation(self):
        print("Hi, my name is " + self.name + " and I live in " + self.country + ".")

loc = Location("Ozzie", "Dominican Republic")
#print(loc.name)
#print(loc.country)
#print(type(loc))

# First instantion of the class Location
loc1 = Location("Tomas", "Portugal")
# Call a method from the instantiated class
loc1.myLocation()


Step 3: Instantiate the Location class multiple times and call the myLocation method.

loc2 = Location("Ying", "China")
loc3 = Location("Amare", "Kenya")
loc2.myLocation()
loc3.myLocation()
your_loc = Location("Your_Name", "Your_Country")
loc.myLocation()

Part 4: Full Script

class Location:
    def __init__(self, name, country):
        self.name = name
        self.country = country
    def myLocation(self):
        print("Hi, my name is " + self.name + " and I live in " + self.country + ".")

loc = Location("Ozzie", "Dominican Republic")
#print(loc.name)
#print(loc.country)
#print(type(loc))

# First instantion of the class Location
loc1 = Location("Tomas", "Portugal")
# Call a method from the instantiated class
loc1.myLocation()
# Three more instantiations and method calls for the Location class
loc2 = Location("Ying", "China")
loc3 = Location("Amare", "Kenya")
loc2.myLocation()
loc3.myLocation()
your_loc = Location("Your_Name", "Your_Country")
loc.myLocation()

Part 5: Review the circleClass.py Script
This part involves reviewing the circleClass.py script, which demonstrates how to create a class that calculates the circumference of a circle and prints the result.

# Given a radius value, print the circumference of a circle.
# Formula for a circumference is c = pi * 2 * radius


class Circle:
    def __init__(self, radius):
        self.radius = radius
    def circumference(self):
        pi = 3.14
        circumferenceValue = pi * self.radius * 2
        return circumferenceValue
    def printCircumference(self):
        myCircumference = self.circumference()
        print ("Circumference of a circle with a radius of " + str(self.radius) + " is " + str(myCircumference))

# First instantiation of the Circle class.
circle1 = Circle(2)
# Call the printCircumference for the instantiated circle1 class.
circle1.printCircumference()
# Two more instantiations and method calls for the Circle class.
circle2 = Circle(5)
circle2.printCircumference()
circle3 = Circle(7)
circle3.printCircumference()

