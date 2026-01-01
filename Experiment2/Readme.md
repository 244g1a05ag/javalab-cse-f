# Experiment2
## TITLE : 2a) Class mechanism in Java
```
class Square
{
    int length;

    int AreaofSquare()
    {
        return length * length;
    }

    int PerimeterofSquare()
    {
        return 4 * length;
    }
}
class Main {
    public static void main(String args[])
    {
        Square sq = new Square();
        sq.length = 5;

        int area = sq.AreaofSquare();
        int perimeter = sq.PerimeterofSquare();

        System.out.println("Area of the square: " + area);
        System.out.println("Perimeter of the square: " + perimeter);
    }
}
```

# OUTPUT
![output_of_classmechanism](exp2a.PNG)

## TITLE 2b) Overloading(Addition of numbers)
```
class Add
{
    int Add(int a, int b)
    {
        return a + b;
    }

    double Add(double a, double b)
    {
        return a + b;
    }

    int Add(int a, int b, int c)
    {
        return a + b + c;
    }
}
class Main
{
    public static void main(String args[])
    {
        Add obj = new Add();

        System.out.println("Addition of two integers: " + obj.Add(10, 20));
        System.out.println("Addition of two doubles: " + obj.Add(10.5, 20.5));
        System.out.println("Addition of three integers: " + obj.Add(10, 20, 30));
    }
}
```

# OUTPUT
![output_of_addition](exp2b.PNG)

## TITLE : 2c) Student information
```
class Student
{
    String sname;
    int sage;
    double smarks;

    Student(String name, int age, double marks)
    {
        sname = name;
        sage = age;
        smarks = marks;
    }

    void display()
    {
        System.out.println("Student name : " + sname);
        System.out.println("Student age  : " + sage);
        System.out.println("Student marks: " + smarks);
    }
}
class Main
{
    public static void main(String args[])
    {
        Student std = new Student("Salini", 20, 98.9);
        std.display();
    }
}
```

# OUTPUT
![output_of_studentinfo](exp2c.PNG)

