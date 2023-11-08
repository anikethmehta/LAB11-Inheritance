### ***Title*** : LAB13
### ***Aim*** : Inheritance
### ***Algorithm*** : 

Algorithm for Constructor Calling in Inheritance:

The base class constructor is called first.

The derived class constructor is called after the base class constructor.

The constructors are called in the order of inheritance, meaning the base class constructor is called before the derived class constructor.

### ***Explanation*** :

Base Class Constructor Call:

When a derived class object is created, the constructor of the base class is called first. This is because the derived class inherits the properties and behavior of the base class, and before any additional initialization specific to the derived class, the base class needs to be properly constructed. If the base class has a parameterized constructor, the derived class's constructor must call it explicitly, passing the required arguments.

Derived Class Constructor Call:

After the base class constructor has been executed, the derived class constructor is called. The derived class constructor can perform its own initialization and may also call the base class constructor explicitly using the base class's constructor within its member initializer list.

Order of Inheritance:

The order in which constructors are called is determined by the order of inheritance. In the example above, Derived publicly inherits from Base, so the Base class constructor is called before the Derived class constructor. If there were multiple base classes, they would be initialized in the order they are listed in the inheritance declaration.

In summary, when a derived class object is defined in C++, the constructors are called in a well-defined order: first the base class constructor(s), in the order of inheritance, and then the derived class constructor. You can use member initializer lists to explicitly call base class constructors if needed. This ensures proper initialization and allows you to set up the derived class's specific behavior while inheriting the characteristics of the base class.

### ***Output Screenshot*** :
