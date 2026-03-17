using System;

class Calculator
{
    static void Main()
    {
        double num1, num2, result;
        char op;

        Console.WriteLine("Simple Calculator");

        Console.Write("Enter first number: ");
        num1 = Convert.ToDouble(Console.ReadLine());

        Console.Write("Enter operator (+, -, *, /): ");
        op = Convert.ToChar(Console.ReadLine());

        Console.Write("Enter second number: ");
        num2 = Convert.ToDouble(Console.ReadLine());

        if (op == '+')
        {
            result = num1 + num2;
            Console.WriteLine("Result = " + result);
        }
        else if (op == '-')
        {
            result = num1 - num2;
            Console.WriteLine("Result = " + result);
        }
        else if (op == '*')
        {
            result = num1 * num2;
            Console.WriteLine("Result = " + result);
        }
        else if (op == '/')
        {
            if (num2 != 0)
            {
                result = num1 / num2;
                Console.WriteLine("Result = " + result);
            }
            else
            {
                Console.WriteLine("Division by zero is not allowed.");
            }
        }
        else
        {
            Console.WriteLine("Invalid operator");
        }

        Console.ReadLine();
    }
}
