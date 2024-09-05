<pre lang=c#><code>
using System;
using System.Collections.Generic;
using System.Data;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _3._2._2_ProgrammingConcepts
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //  variable declaration
            // dataType Idendtifier (value) ;
            int num;
            string myString = "This is a string";
            //• constant declaration
            // const dataType Identifier = value ;
            const double planck = 6.62607015e-34;
            //• assignment
            // variable = value ;
            num = 123;
            myString = "This is an assignment";
            // assignemnt from user input
            // Console.ReadLine();
            // Always reads as a string
            // need to convert to any other data type
            // dataType.Parse(Console.Readline());
            Console.Write("Enter some text: "); //output same line ending
            myString = Console.ReadLine();
            Console.Write("Enter a value for a new string: ");
            string newString = Console.ReadLine();
            // Non string inputs
            Console.Write("Enter a number: ");
            num = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter a single character: ");
            char c =Convert.ToChar (Console.ReadLine());
            Console.Write("Enter a floating point number: ");
            double d = Convert.ToDouble (Console.ReadLine());
            //• iteration
            // for loops
            //
            for (int i = 0; i < 10; i++) // 0 to 9 counting up
            {
                Console.WriteLine(i);
            }
           
            //User input to guide number of times to loop
            Console.Write("Enter how many times to loop: ");
            num = Convert.ToInt32(Console.ReadLine());
            for (int i = 1; i <= num; i++)
            {
                Console.WriteLine(i);
            }
            //Loop with diferent increment
            for (int i = 0; i <= 100; i += 10)
            {
                Console.WriteLine(i); // adding 10 each time it loops
            }
            //Loop down
            for (int i = 10; i > 0; i--)
            {
                Console.WriteLine(i); // counting down from 10 to 1
            }
            // Condition controlled looping
            num = 10;
            while (num > 0)
            {
                num--;
            }
            num = 10;
            do
            {
                num -= 2;
            }while (num > 0);
            
            // Nested iteration
            bool found = false;
            int counter = 0;
            while (!found)
            {
                for (int i = 0;i<10;i++)
                {
                    Console.WriteLine(i);
                }
                counter++;
                if (counter == 10)
                {
                    found = true;
                }
            }

            for (int i = 0; i<10; i++) {
                found = false;
                while (!found)
                {
                    Console.WriteLine("Enter a number: ");
                    num = Convert.ToInt32(Console.ReadLine());
                    if (num == i)
                    {
                        found = true;
                    }
                }
            }
            //• selection
            // if(criteria){ thing to do }
            // Compari
            
            //• subroutine(procedure / function)
        }
    }
}
</code></pre>
