# CS-largest_Number-Project
A repository for CS code that finds out the largest number among 3 numbers.  
## Main Code  
```
using System;

namespace largest_Number
{
    internal class Program
    {
        static void Main(string[] args)
        {
            try
            {
                Console.WriteLine("---FINDING THE LARGEST NUMBER---");

                int n1, n2, n3, largest;
                Console.Write("Enter the first number: ");
                n1 = Convert.ToInt32(Console.ReadLine());
                Console.Write("Enter the second number: ");
                n2 = Convert.ToInt32(Console.ReadLine());
                Console.Write("Enter the thrid number: ");
                n3 = Convert.ToInt32(Console.ReadLine());

                if (n1 > n2 && n1 > n3)
                    largest = n1;
                else if (n2 > n1 && n2 > n3)
                    largest = n2;
                else
                    largest = n3;

                Console.WriteLine("Among {0}, {1} and {2} the largest number is {3}", n1, n2, n3, largest);
            }
            catch (FormatException e)
            {
                Console.WriteLine("Enter Only Numbers Please!");
            }
            catch (Exception)
            {
                Console.WriteLine("Something Went Wrong!");
            }
            finally
            {
                Console.WriteLine("Press any key to exit.");
                Console.ReadKey();
            }
        }
    }
}
```
