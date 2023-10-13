# Abstraction

In OOPS we use "abstraction" to simplify some complex systems,This is where we model our classes based on their *essential* characteristics while **hiding** the unnecessary details.
This allows us to manage complexity and create a clear distinction between what the object does (behavior) and HOW it achieves its behavior (the implementation details). This allows us to focus on the "what" rather the "how".

We have Key aspects of *abstraction* 

## Class Modeling

- This involves defining classes and their methods / properties,this captures the essential characteristics and behaviors of objects within a domain. This lets us create a blueprint for objects without specifying how the objects work interally.

## Data Hiding

- This is also known as "Encapsulation". This is a fundamental principle in OOP, This is a way of restricting direct access to certain attributes of a class, this is  a way we controll access of data through the methods. This is how we control the integrity of the objects state and control how the data is manipluated.

```js
    class BankAccount{
        constructor(accountNumber, balance){
            this.accountNumber = accountNumber;
            //underscore to show indicater "protected" data its a convention.

            this._balance = balance;
        }
        // Get method to access balance
        get balance(){
            return this._balance;
        }
        // Method to deposit money
        deposit(amount){
            if(amount>0){
                this._balance += amount;
                console.log(`deposited ${amount}.New Balance is :  ${this._balance}`);
            } else {
                console.log("invalid deposite amount.")
            }
        }
        // Method to withdraw money
        withdraw(amount){
            if(amount > 0 && amount <= this._balance){
                this._balance -= amount;
                console.log(`withdrawn ${amount}. New Balance is ${this._balance}`);
            } else{
                console.log("Invalid withdrawal amount or insufficient balance.");
            }
        }
    }

    const account - new BankAccount("12345", 1000);

    //direct access to balance is restricted
    //access is constrolled through the getter method
    console.log(account.balance);//1000

    //Modiying the balance is not allowed

    account.deposit(500);// deposited $500
    account.withdraw(200);//withdrawn $200

```

## Simplification

- This is the concept that allows us to break down big complex systems into smaller understandable components. This allows us to work with higher-level concepts, making the design and maintenance of software more manageable.

## Focus on Relevant Details

- Abstraction helps Devs focus on the relevant details while hiding the less important ones. This is very powerful and important when working on large complex code bases.

## Reusability

- Abstraction promotes reusablity. By defining abstract classes and interfaces, You can create common structures that multiple classes can implement, with this we can reduce code duplication.

## Polymorphism

- Abstraction is closely related to polymorphism, as it allows you to interact with objects in a generic way,based on their common interfaces. This enables you to write code that can work with objects of different classes as long as they conform to the same abstraction.
