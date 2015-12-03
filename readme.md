Reactive components
===================

Reactive components is a set of UI Input components which can be used to build widgets. The components are build on top of actorjs. Every component is build around an actor and only communicate by message passing. This makes that the components are total loosely coupled. 

Components are build by the following principles:
* Internal state of the components is stored by event sourcing. 
* Components publish there value on the eventbus
* The value of a component is a single value
* Every component has an unique  within the widget


Types
-----
There are different type of components. The type is correlated with the type of value the component publishes to the bus. 

**BooleanComponent**  
The output of a *BooleanComponent* is a value with true or false.

**StringComponent**  
The value of a *StringComponent* is a value with true or false.

**ObjectComponent**  
The input of an *ObjectComponent* is an array of objects or strings. The value that is published on the bus is one object or string from the array.

**Array Component**  
The input of an *StringComponent* is an array of objects or strings. The value that is published is an array of objects or strings.

Categories
----------
Components are divided in different categories. 

