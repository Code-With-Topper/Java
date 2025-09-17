# 📘 Java Programs (1–42) with Outputs

---

## **1. Hello World**

```java
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```

**Output**

```
Hello World
```

---

## **2. Arithmetic Operations**

```java
class Arithmetic {
    public static void main(String[] args) {
        int a = 10, b = 5;
        System.out.println("Addition = " + (a + b));
        System.out.println("Subtraction = " + (a - b));
        System.out.println("Multiplication = " + (a * b));
        System.out.println("Division = " + (a / b));
    }
}
```

**Output**

```
Addition = 15
Subtraction = 5
Multiplication = 50
Division = 2
```

---

## **3. Simple Interest**

```java
class SimpleInterest {
    public static void main(String[] args) {
        double p = 1000, r = 5, t = 2;
        double si = (p * r * t) / 100;
        System.out.println("Simple Interest = " + si);
    }
}
```

**Output**

```
Simple Interest = 100.0
```

---

## **4. Odd or Even**

```java
class OddEven {
    public static void main(String[] args) {
        int num = 7;
        if (num % 2 == 0)
            System.out.println(num + " is Even");
        else
            System.out.println(num + " is Odd");
    }
}
```

**Output**

```
7 is Odd
```

---

## **5. Area of Circle**

```java
class AreaCircle {
    public static void main(String[] args) {
        double r = 5.0;
        double area = Math.PI * r * r;
        System.out.println("Area of Circle = " + area);
    }
}
```

**Output**

```
Area of Circle = 78.53981633974483
```

---

## **6. Largest of Three Numbers**

```java
class LargestThree {
    public static void main(String[] args) {
        int a = 10, b = 25, c = 15;

        if (a >= b && a >= c)
            System.out.println("Largest = " + a);
        else if (b >= a && b >= c)
            System.out.println("Largest = " + b);
        else
            System.out.println("Largest = " + c);
    }
}
```

**Output**

```
Largest = 25
```

---

## **7. Pattern Printing**

```java
class Pattern {
    public static void main(String[] args) {
        int n = 5;
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```

**Output**

```
* 
* * 
* * * 
* * * * 
* * * * * 
```

---

## **8. Simple If Statement**

```java
class SimpleIf {
    public static void main(String[] args) {
        int age = 20;
        if (age > 18) {
            System.out.println("You are eligible to vote.");
        }
    }
}
```

**Output**

```
You are eligible to vote.
```

---

## **9. If..Else Statement**

```java
class IfElse {
    public static void main(String[] args) {
        int num = 15;
        if (num % 2 == 0)
            System.out.println("Even Number");
        else
            System.out.println("Odd Number");
    }
}
```

**Output**

```
Odd Number
```

---

## **10. Nested If Statement**

```java
class NestedIf {
    public static void main(String[] args) {
        int num = 25;

        if (num > 0) {
            if (num % 2 == 0)
                System.out.println(num + " is Positive Even");
            else
                System.out.println(num + " is Positive Odd");
        }
    }
}
```

**Output**

```
25 is Positive Odd
```

---

## **11. If..Else..If Statement**

```java
class IfElseIf {
    public static void main(String[] args) {
        int marks = 75;

        if (marks >= 90)
            System.out.println("Grade A");
        else if (marks >= 75)
            System.out.println("Grade B");
        else if (marks >= 50)
            System.out.println("Grade C");
        else
            System.out.println("Fail");
    }
}
```

**Output**

```
Grade B
```

---

## **12. While Loop**

```java
class WhileLoop {
    public static void main(String[] args) {
        int i = 1;
        while (i <= 5) {
            System.out.println(i);
            i++;
        }
    }
}
```

**Output**

```
1
2
3
4
5
```

---

## **13. For Loop**

```java
class ForLoop {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            System.out.println(i);
        }
    }
}
```

**Output**

```
1
2
3
4
5
```

---

## **14. Do While Loop**

```java
class DoWhileLoop {
    public static void main(String[] args) {
        int i = 1;
        do {
            System.out.println(i);
            i++;
        } while (i <= 5);
    }
}
```

**Output**

```
1
2
3
4
5
```

---

## **15. Switch Case**

```java
class SwitchCase {
    public static void main(String[] args) {
        int day = 3;

        switch (day) {
            case 1: System.out.println("Monday"); break;
            case 2: System.out.println("Tuesday"); break;
            case 3: System.out.println("Wednesday"); break;
            case 4: System.out.println("Thursday"); break;
            case 5: System.out.println("Friday"); break;
            case 6: System.out.println("Saturday"); break;
            case 7: System.out.println("Sunday"); break;
            default: System.out.println("Invalid Day");
        }
    }
}
```

**Output**

```
Wednesday
```

---

## **16. Constructor**

```java
class Student {
    String name;
    int age;

    Student(String n, int a) {
        name = n;
        age = a;
    }

    void display() {
        System.out.println("Name: " + name + ", Age: " + age);
    }

    public static void main(String[] args) {
        Student s1 = new Student("Rahul", 20);
        s1.display();
    }
}
```

**Output**

```
Name: Rahul, Age: 20
```

---

## **17. Constructor Overloading**

```java
class Student {
    String name;
    int age;

    Student() {
        name = "Unknown";
        age = 0;
    }

    Student(String n, int a) {
        name = n;
        age = a;
    }

    void display() {
        System.out.println("Name: " + name + ", Age: " + age);
    }

    public static void main(String[] args) {
        Student s1 = new Student();
        Student s2 = new Student("Riya", 22);
        s1.display();
        s2.display();
    }
}
```

**Output**

```
Name: Unknown, Age: 0
Name: Riya, Age: 22
```

---

## **18. Single Inheritance**

```java
class Animal {
    void eat() { System.out.println("Animal eats food."); }
}

class Dog extends Animal {
    void bark() { System.out.println("Dog barks."); }

    public static void main(String[] args) {
        Dog d = new Dog();
        d.eat();
        d.bark();
    }
}
```

**Output**

```
Animal eats food.
Dog barks.
```

---

## **19. Multilevel Inheritance**

```java
class Animal {
    void eat() { System.out.println("Animal eats food."); }
}

class Dog extends Animal {
    void bark() { System.out.println("Dog barks."); }
}

class Puppy extends Dog {
    void weep() { System.out.println("Puppy weeps."); }

    public static void main(String[] args) {
        Puppy p = new Puppy();
        p.eat();
        p.bark();
        p.weep();
    }
}
```

**Output**

```
Animal eats food.
Dog barks.
Puppy weeps.
```

---

## **20. Hierarchical Inheritance**

```java
class Animal {
    void eat() { System.out.println("Animal eats food."); }
}

class Dog extends Animal {
    void bark() { System.out.println("Dog barks."); }
}

class Cat extends Animal {
    void meow() { System.out.println("Cat meows."); }
}

public class TestInheritance {
    public static void main(String[] args) {
        Dog d = new Dog();
        d.eat(); d.bark();

        Cat c = new Cat();
        c.eat(); c.meow();
    }
}
```

**Output**

```
Animal eats food.
Dog barks.
Animal eats food.
Cat meows.
```

---

## **21. Method Overloading (Area)**

```java
class Area {
    void findArea(double r) {
        System.out.println("Area of Circle: " + (3.14 * r * r));
    }

    void findArea(int s) {
        System.out.println("Area of Square: " + (s * s));
    }

    void findArea(int l, int b) {
        System.out.println("Area of Rectangle: " + (l * b));
    }

    public static void main(String[] args) {
        Area a = new Area();
        a.findArea(5.0);
        a.findArea(4);
        a.findArea(5, 3);
    }
}
```

**Output**

```
Area of Circle: 78.5
Area of Square: 16
Area of Rectangle: 15
```

---

## **22. Scanner Class**

```java
import java.util.Scanner;

class ScannerExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter name: ");
        String name = sc.nextLine();

        System.out.print("Enter age: ");
        int age = sc.nextInt();

        System.out.println("Hello " + name + ", Age: " + age);
    }
}
```

**Output (example input: John, 21)**

```
Enter name: John
Enter age: 21
Hello John, Age: 21
```

---

## **23. Menu Driven Program**

```java
import java.util.Scanner;

class Menu {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int choice;

        do {
            System.out.println("1. Add  2. Subtract  3. Exit");
            choice = sc.nextInt();

            switch (choice) {
                case 1:
                    System.out.println("Enter two numbers:");
                    int a = sc.nextInt(), b = sc.nextInt();
                    System.out.println("Sum = " + (a + b));
                    break;

                case 2:
                    System.out.println("Enter two numbers:");
                    a = sc.nextInt(); b = sc.nextInt();
                    System.out.println("Difference = " + (a - b));
                    break;
            }
        } while (choice != 3);
    }
}
```

**Output (example)**

```
1. Add  2. Subtract  3. Exit
1
Enter two numbers:
5 3
Sum = 8
```

---

## **24. Initialization of Array**

```java
class ArrayInit {
    public static void main(String[] args) {
        int[] arr = {10, 20, 30, 40};

        for (int i : arr) {
            System.out.println(i);
        }
    }
}
```

**Output**

```
10
20
30
40
```

---

## **25. Multidimensional Array**

```java
class MultiArray {
    public static void main(String[] args) {
        int[][] arr = { {1,2}, {3,4}, {5,6} };

        for (int i=0; i<3; i++) {
            for (int j=0; j<2; j++) {
                System.out.print(arr[i][j] + " ");
            }
            System.out.println();
        }
    }
}
```

**Output**

```
1 2
3 4
5 6
```

---

## **26. Addition of Array**

```java
class AddArray {
    public static void main(String[] args) {
        int[] a = {1,2,3}, b = {4,5,6};
        int[] c = new int[a.length];

        for (int i=0; i<a.length; i++) {
            c[i] = a[i] + b[i];
            System.out.println(c[i]);
        }
    }
}
```

**Output**

```
5
7
9
```

---

## **27. Subtraction of Array**

```java
class SubArray {
    public static void main(String[] args) {
        int[] a = {10,20,30}, b = {4,5,6};
        int[] c = new int[a.length];

        for (int i=0; i<a.length; i++) {
            c[i] = a[i] - b[i];
            System.out.println(c[i]);
        }
    }
}
```

**Output**

```
6
15
24
```

---

## **28. Multiplication of Array**

```java
class MulArray {
    public static void main(String[] args) {
        int[] a = {2,3,4}, b = {5,6,7};
        int[] c = new int[a.length];

        for (int i=0; i<a.length; i++) {
            c[i] = a[i] * b[i];
            System.out.println(c[i]);
        }
    }
}
```

**Output**

```
10
18
28
```

---

## **29. Abstract Class**

```java
abstract class Shape {
    abstract void draw();
}

class Circle extends Shape {
    void draw() { System.out.println("Drawing Circle"); }
}

public class TestAbstract {
    public static void main(String[] args) {
        Shape s = new Circle();
        s.draw();
    }
}
```

**Output**

```
Drawing Circle
```

---

## **30. Interface**

```java
interface Animal {
    void sound();
}

class Dog implements Animal {
    public void sound() { System.out.println("Dog barks"); }
}

public class TestInterface {
    public static void main(String[] args) {
        Animal a = new Dog();
        a.sound();
    }
}
```

**Output**

```
Dog barks
```

---

## **31. Super Keyword**

```java
class Animal {
    Animal() { System.out.println("Animal constructor"); }
    void eat() { System.out.println("Animal eats"); }
}

class Dog extends Animal {
    Dog() { super(); }
    void eat() {
        super.eat();
        System.out.println("Dog eats");
    }
}

public class TestSuper {
    public static void main(String[] args) {
        Dog d = new Dog();
        d.eat();
    }
}
```

**Output**

```
Animal constructor
Animal eats
Dog eats
```

---

## **32. Exception Handling**

```java
class ExceptionDemo {
    public static void main(String[] args) {
        try {
            int a = 5 / 0;
        } catch (ArithmeticException e) {
            System.out.println("Error: " + e);
        } finally {
            System.out.println("Finally block executed.");
        }
    }
}
```

**Output**

```
Error: java.lang.ArithmeticException: / by zero
Finally block executed.
```

---

## **33. Thread**

```java
class MyThread extends Thread {
    public void run() {
        for (int i=1; i<=5; i++)
            System.out.println("Thread running: " + i);
    }

    public static void main(String[] args) {
        MyThread t = new MyThread();
        t.start();
    }
}
```

**Output (example)**

```
Thread running: 1
Thread running: 2
Thread running: 3
Thread running: 4
Thread running: 5
```

---

## **34. String Functions**

```java
class StringDemo {
    public static void main(String[] args) {
        String s = "Hello Java";
        System.out.println("Length: " + s.length());
        System.out.println("Upper: " + s.toUpperCase());
        System.out.println("Substring: " + s.substring(0,5));
        System.out.println("Contains 'Java': " + s.contains("Java"));
    }
}
```

**Output**

```
Length: 10
Upper: HELLO JAVA
Substring: Hello
Contains 'Java': true
```

---

## **35. Math Functions**

```java
class MathDemo {
    public static void main(String[] args) {
        System.out.println("Square root: " + Math.sqrt(25));
        System.out.println("Power: " + Math.pow(2, 3));
        System.out.println("Random: " + Math.random());
        System.out.println("Max: " + Math.max(10, 20));
    }
}
```

**Output (example)**

```
Square root: 5.0
Power: 8.0
Random: 0.3748293
Max: 20
```

---

## **36. Utility Package Classes**

```java
import java.util.*;

class UtilityDemo {
    public static void main(String[] args) {
        Date d = new Date();
        System.out.println("Date: " + d);

        Random r = new Random();
        System.out.println("Random: " + r.nextInt(100));

        ArrayList<String> list = new ArrayList<>();
        list.add("Apple");
        list.add("Banana");
        System.out.println("ArrayList: " + list);
    }
}
```

**Output (example)**

```
Date: Mon Sep 17 12:34:56 IST 2025
Random: 42
ArrayList: [Apple, Banana]
```

---

## **37. IO Package**

```java
import java.io.*;

class IODemo {
    public static void main(String[] args) throws Exception {
        FileWriter fw = new FileWriter("test.txt");
        fw.write("Hello, this is a file!");
        fw.close();

        FileReader fr = new FileReader("test.txt");
        int i;
        while((i = fr.read()) != -1)
            System.out.print((char)i);
        fr.close();
    }
}
```

**Output**

```
Hello, this is a file!
```

---

## **38. Applet Message**

```java
import java.applet.Applet;
import java.awt.Graphics;

// <applet code="HelloApplet" width=300 height=200></applet>
public class HelloApplet extends Applet {
    public void paint(Graphics g) {
        g.drawString("Hello, Applet!", 100, 100);
    }
}
```

**Output**

```
(Applet window displaying "Hello, Applet!" text)
```

---

## **39. Configure Applet**

```java
import java.applet.Applet;
import java.awt.Graphics;

// <applet code="ConfigApplet" width=300 height=200>
// <param name="msg" value="Welcome to Java Applet!">
// </applet>
public class ConfigApplet extends Applet {
    String msg;
    public void init() {
        msg = getParameter("msg");
    }
    public void paint(Graphics g) {
        g.drawString(msg, 50, 100);
    }
}
```

**Output**

```
(Applet window displaying "Welcome to Java Applet!" text)
```

---

## **40. Keyboard Events**

```java
import java.awt.*;
import java.awt.event.*;

class KeyEventDemo extends Frame implements KeyListener {
    String msg = "";

    KeyEventDemo() {
        addKeyListener(this);
        setSize(300,300);
        setVisible(true);
    }

    public void keyPressed(KeyEvent e) { msg = "Key Pressed"; repaint(); }
    public void keyReleased(KeyEvent e) { msg = "Key Released"; repaint(); }
    public void keyTyped(KeyEvent e) { msg = "Key Typed"; repaint(); }

    public void paint(Graphics g) { g.drawString(msg, 50, 100); }

    public static void main(String[] args) {
        new KeyEventDemo();
    }
}
```

**Output**

```
(Window displays "Key Pressed" / "Key Released" / "Key Typed" when keys are used)
```

---

## **41. Mouse Events**

```java
import java.awt.*;
import java.awt.event.*;

class MouseEventDemo extends Frame implements MouseListener {
    String msg = "";

    MouseEventDemo() {
        addMouseListener(this);
        setSize(300,300);
        setVisible(true);
    }

    public void mouseClicked(MouseEvent e) { msg = "Mouse Clicked"; repaint(); }
    public void mouseEntered(MouseEvent e) { msg = "Mouse Entered"; repaint(); }
    public void mouseExited(MouseEvent e) { msg = "Mouse Exited"; repaint(); }
    public void mousePressed(MouseEvent e) { msg = "Mouse Pressed"; repaint(); }
    public void mouseReleased(MouseEvent e) { msg = "Mouse Released"; repaint(); }

    public void paint(Graphics g) { g.drawString(msg, 50, 100); }

    public static void main(String[] args) {
        new MouseEventDemo();
    }
}
```

**Output**

```
(Window displays "Mouse Clicked", "Mouse Entered", etc. depending on actions)
```

---

## **42. Graphics Class**

```java
import java.applet.Applet;
import java.awt.*;

// <applet code="GraphicsDemo" width=400 height=400></applet>
public class GraphicsDemo extends Applet {
    public void paint(Graphics g) {
        g.setColor(Color.red);
        g.drawRect(50, 50, 100, 60);
        g.fillOval(200, 50, 100, 60);
        g.drawLine(50, 200, 200, 200);
    }
}
```

**Output**

```
(Applet window showing red rectangle, filled oval, and line)
```
