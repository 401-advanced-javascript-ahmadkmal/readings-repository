## advantages to Test Driven Development

1. The Best Level Acceptance:

TDD implementation helps the developers to understand the requirements from the perspective experience of clients. The test cases are designed without the constraints of architecture design or traditional programming approaches. TDD maximizes the possibility of developing the best quality product fulfilling the communicated needs of all the stakeholders.

2. TDD - Customer-Centric Agile Process:

TDD process gets fit into the customer-centric agile methodology. The iteration for quality improvement is defined as the incorporation of new functionality against the model set of traditional practices or problem statements.

3. Prompt Feedback:

The streamlined TDD process helps the project development team members to improve their delivering capability because of providing the immediate feedback on the developed components. The shorter feedback sharing loop squeezes the turnaround period for the elimination of identified defects; and, the outcome is comparatively much better than it is in traditional waterfall methodology.

## afterEach and beforEach

afterEach runs after every Runnable instance; in your case, an it() block. If you do not want the nested behavior, don't nest your tests. Altering this behavior is not on the table.

## downside of Test Driven Development

The test suite itself has to be maintained; tests may not be completely deterministic (i.e. reliant on external dependencies).

The tests may be hard to write, esp. beyond the unit testing level.

Initially, it slows down development; for rapidly iterative startup environments the implementation code may not be ready for some time due to spending time writing tests first. (But in the long run, it actually speeds up development)

Class-based vs. prototype-based languages
Class-based object-oriented languages, such as Java and C++, are founded on the concept of two distinct entities: classes and instances.

## class vs constructor

A class defines all of the properties that characterize a certain set of objects (considering methods and fields in Java, or members in C++, to be properties). A class is abstract rather than any particular member in a set of objects it describes. For example, the Employee class could represent the set of all employees.
An instance, on the other hand, is the instantiation of a class; that is. For example, Victoria could be an instance of the Employee class, representing a particular individual as an employee. An instance has exactly the same properties of its parent class (no more, no less).
A prototype-based language, such as JavaScript, does not make this distinction: it simply has objects. A prototype-based language has the notion of a prototypical object, an object used as a template from which to get the initial properties for a new object. Any object can specify its own properties, either when you create it or at run time. In addition, any object can be associated as the prototype for another object, allowing the second object to share the first object's properties.
so in es6 they develop class to make developer more comfortable when they use js

## Static methods

Static methods are called without instantiating their class and are also not callable when the class is instantiated. Static methods are often used to create utility functions for an application. In other words, static methods have no access to data stored in specific objects.

## example of higher order function

higher order function mean that you use some function in another function
and here an exaple of higher order function

const double = n => n * 2

[1, 2, 3, 4].map(double) // [ 2, 4, 6, 8 ]

it duoble the elemen in array  
