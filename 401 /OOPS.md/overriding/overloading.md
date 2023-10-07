# Overloading & Overriding

The concept of overriding is when we allow the subclass to override a method that is also available in the superclass, However we do this so the subclass can have its own version of this method. This is **Polymorphism**

```java
    class Animal{
        void makeSound(){
            System.out.printIn("Some generic sound an anima, makes")
        }
    }

    class Dog extends Animal{
        //override
        void makeSound(){
            System.out.printIn("Bark")
        }
    }

```

You will notice that the subclass has the same "signature" (name, paramters, and return type) as the superclass, this is essential so the compiler will know that this is a form of "Overriding".

## Overloading

Overloading is when we have a class that has different methods with the *same* name however take a different paramenters list.
These methods are considered overloading because they have the same name but they perform different tasks based off of the *number* **OR** *types*  of args.

Overloading gives us a way to create methods that have similar functionality but can operate on different types of data, or they can accept different combinations of arguments.

```js
    class Person {
        constructor(name, age){
            this.name = name;
            this.age = age;
        }

    constructor(..args){
        if(args.length === 1){
            this.name = args[0];
        } else if (args.length === 2){
            this.name = args [0];
            this.age = args [1];
        }
    } else {
        throw new Error("Invalide number of arguments");
    }

    }

```

In thias example we creat a constructor that allows us to create a `Person` object. We use rest operator to place in our arguments.

Inside the constructor we check the `args.length` for the specific number of arguments. If we place in one argument it was stand for the persons name and if we place in two arguments we will have both our `Persons` "name" and  " age" and if we get less than one arguement we also have error handling.

This is an example of overloading because this allows the class to be flexible in accepting different arguments while keep a clean interface.
