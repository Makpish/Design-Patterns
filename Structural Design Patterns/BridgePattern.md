#Bridge Pattern
##https://springframework.guru/gang-of-four-design-patterns/bridge-pattern/


- Decouple an abstraction from its implementation so that the two can vary independently.

- the objective of the bridge pattern is to identify how to realize relationships between classes and objects

- The bridge pattern does it by separating the abstraction and the implementation in separate class hierarchies. The bridge between the class hierarchies is achieved through composition.

- With the bridge pattern, the abstraction maintains a Has-A relationship with the implementation instead of a IS-A relationship. The Has-A relationship is achieved through composition where the abstraction maintains a reference of the implementation and forwards client requests to it.