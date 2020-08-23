#Abstract Factory Pattern
##https://www.tutorialspoint.com/design_pattern/abstract_factory_pattern.htm
##https://springframework.guru/gang-of-four-design-patterns/abstract-factory-design-pattern/


- creational pattern

- used to create families of objects, where the objects of a family are designed to work together

- super-factory which creates other factories

- From the client point of view, it means that a client can create a family of related objects without knowing about the object definitions and their concrete class names.

- Abstract factory adds another level of abstraction to factory method. While factory method abstracts the way objects are created, abstract factory abstracts how the factories are created. The factories in turn abstracts the way objects are created. You will often hear the abstract factory design pattern referred to as a “factory of factories“.

- mostly use when client need to create instance of different objects. this helps by abstracting each object knowledge from client and giving them a factory to generate desired object.


##Example:

Now, let us summarize the components of the abstract factory pattern in the context of the enhanced pizza store:

- AbstractProduct (Cheese and Sauce): Is an interface or an abstract class whose subclasses are instantiated by the abstract factory objects.

- ConcreteProduct (GoatCheese, MozzarellaCheese, TomatoSauce, and CaliforniaOilSauce): Are the concrete subclasses that implement/extend AbstractProduct. The abstract factory objects instantiate these subclasses.

- AbstractFactory (BaseToppingFactory): Is an interface or an abstract class whose subclasses instantiate a family of AbstractProduct objects.

- ConcreteFactory (SicillianToppingFactory and GourmetToppingFactory): Are the concrete subclasses that implement/extend AbstractFactory. An object of this subclass instantiates a family of AbstractProduct objects.

- Client: Uses AbstractFactory to get AbstractProduct objects.