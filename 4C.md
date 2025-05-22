
# EX 4C Constructor Chaining
## DATE:
## AIM:
To create a class named 'Animal' which includes its constructor. [constructor will print " I am an Animal"]

Create a child class of 'Animal' named 'Dog' and add a its constructor [constructor will call its super-class constructor and print " I am a Dog"] 

Create a instance of Dog class and invoke the constructor using object.











## Algorithm

1.Create a class Animal with a constructor that prints "I am an animal".

2.Create a subclass Dog that extends Animal and has a constructor which calls super() and prints "I am a dog".

3.Use super() in the Dog constructor to invoke the parent class (Animal) constructor.

4.In the main() method, create an object of the Dog class.

5.Observe the output showing the sequence of constructor calls from parent to child.








## Program:

Developed by: Kancharla Narmadha
Register Number: 212222110016
```
class Animal {
    Animal() {
        System.out.println("I am an animal");
    }
}

class Dog extends Animal {
    Dog() {
        super();
        System.out.println("I am a dog");
    }
}

public class Main {
    public static void main(String[] args) {
        Dog d = new Dog(); 
    }
}



    
```

## Output:
![image](https://github.com/user-attachments/assets/1728d42f-84f0-48ff-82f0-51ed0c475fea)


## Result:
The program successfully demonstrates constructor chaining using inheritance. When a Dog object is created, the Animal constructor executes first, followed by the Dog constructor.



