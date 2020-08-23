#Factory Pattern
##https://www.tutorialspoint.com/design_pattern/factory_pattern.htm
##https://springframework.guru/gang-of-four-design-patterns/factory-method-design-pattern/


- creational pattern

- In the factory method pattern, you provide an interface, which can be a Java interface or an abstract class to create objects. A factory method in the interface defers the object creation to one or more concrete subclasses at run time. The subclasses implement the factory method to select the class whose objects need to be created.

- Just as in any pizza store, a customer can only order a pizza and not make it.

- In Factory pattern, we create object without exposing the creation logic to the client and refer to newly created object using a common interface.


##Example

The components of the factory method pattern in the context of the pizza store can be summarized as:

- Product (Pizza): Is an interface or an abstract class whose subclasses are instantiated by the factory method.
- ConcreteProduct (CheesePizza, PepperoniPizza, and VeggiePizza): Are the concrete subclasses that implement/extend Product. The factory method instantiates these subclasses.
- Creator (BasePizzaFactory): Is an interface or an abstract class that declares the factory method, which returns an object of type Product.
- ConcreteCreator (PizzaFactory): Is a concrete class that implements the factory method to create and return a ConcreteProduct to Client.
- Client: Asks the Creator for a Product.