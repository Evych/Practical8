# Practical8
 Ось невелика задача на C#, яка демонструє використання класів і методів:
using System;

class Rectangle
{
    // Поля для зберігання довжини і ширини прямокутника
    private double length;
    private double width;

    // Конструктор для ініціалізації довжини і ширини
    public Rectangle(double length, double width)
    {
        this.length = length;
        this.width = width;
    }

    // Метод для обчислення площі прямокутника
    public double CalculateArea()
    {
        return length * width;
    }

    // Метод для обчислення периметру прямокутника
    public double CalculatePerimeter()
    {
        return 2 * (length + width);
    }
}

class Program
{
    static void Main(string[] args)
    {
        // Створення нового прямокутника з довжиною 5 і шириною 3
        Rectangle rectangle = new Rectangle(5, 3);

        // Обчислення та виведення площі прямокутника
        double area = rectangle.CalculateArea();
        Console.WriteLine("Площа прямокутника: " + area);

        // Обчислення та виведення периметру прямокутника
        double perimeter = rectangle.CalculatePerimeter();
        Console.WriteLine("Периметр прямокутника: " + perimeter);
    }
}
