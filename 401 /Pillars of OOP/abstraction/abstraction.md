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
            this.accountNumber = accountNu ber;
            //underscore to show indicater "protected" data
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

```