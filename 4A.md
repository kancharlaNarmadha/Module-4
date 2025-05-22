
# EX 4A Introduction to Java Constructor
## DATE:
## AIM:
To write  a Java program using copy constructor to print the circumference of rectangle.[l=5,w=6]









## Algorithm

1.Create a class Rectangle with instance variables length and breadth.

2.Define a parameterized constructor to initialize a rectangle with given dimensions.

3.Create a copy constructor that initializes a new object using the values of an existing Rectangle object.

4.Define an area() method that returns the product of length and breadth.

5.In the main() method, create one object with values, use the copy constructor to create another, and print the area of both rectangles.








## Program:

Developed by: Kancharla Narmadha
Register Number: 212222110016
```
class Rectangle { 
    int length;
    int breadth;

    Rectangle(int length, int breadth) {  
        this.length = length;
        this.breadth = breadth;
    } 

    Rectangle(Rectangle obj) { 
        this.length = obj.length;
        this.breadth = obj.breadth;
    } 

    int area() { 
        return length * breadth;
    } 
}

public class CopyConstructor { 
    public static void main(String[] args) { 
        Rectangle a = new Rectangle(11,2); 
        Rectangle b = new Rectangle(a);

        System.out.println("Area  of First Rectangle : " + a.area());
        System.out.println("Area of First Second Rectangle : " + b.area());
    } 
}

    
```

## Output:
![image](https://github.com/user-attachments/assets/4d1e5a69-66eb-4bee-9ed7-bdf8cacd542f)


## Result:
The program successfully demonstrates the use of a copy constructor in Java. It creates a new object with the same values as another and calculates the area for both.

