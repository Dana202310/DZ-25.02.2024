//Задача 1. Задайте значения M и N. 
//Напишите программу, которая выведет все натуральные числа в промежутке от M до N. 
//Использовать рекурсию, не использовать циклы. 

// Console.Write("Введите значение M:");
// int m = Convert.ToInt32(Console.ReadLine());
// Console.Write("Введите значение N:");
// int n = Convert.ToInt32(Console.ReadLine());
// void che(int m, int n)
// {
// if (m > n)
// return;
// if (m % 2 == 0)
// {
// Console.Write($"(m),");
// }
// che(m+1,n);

// }
// che(m,n);



//Задача 2. Напишите программу вычисления функции Аккермана с помощью рекурсии.
//Даны два неотрицательных числа m и n.

// Console.Write("Введите число M: ");
// int m = Convert.ToInt32(Console.ReadLine());

// Console.Write("Введите число N: ");
// int n = Convert.ToInt32(Console.ReadLine());

// AkkermanFunction(m,n);

// // вызов функции Аккермана
// void AkkermanFunction(int m, int n)
// {
//     Console.Write(Akkerman(m, n)); 
// }

// // функция Аккермана
// int Akkerman(int m, int n)
// {
//     if (m == 0)
//     {
//         return n + 1;
//     }
//     else if (n == 0 && m > 0)
//     {
//         return Akkerman(m - 1, 1);
//     }
//     else
//     {
//         return (Akkerman(m - 1, Akkerman(m, n - 1)));
//     }
// }



//Задача 3. Задайте произвольный массив. 
//Выведите его элементы, начиная с конца. Использовать рекурсию, не использовать циклы.
using System;
namespace New_Project 
{  
  public static class Program  
  { 
    public static void print(int [] A, int n) 
    { 
      if (n > 0) 
      { 
      	Console.Write(A[n] + " "); 
      	print(A, n - 1); 
      } 
      else Console.WriteLine(A[0]); 
    } 
    public static void Main()   
    { 
      int [] num = {1, 3, 7, 0, 20, 29}; 
      print(num, num.Length - 1); 
    }  
  }   
}
