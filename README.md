# amicabl
using System;<br>

namespace amicable_number<br>
{
    class amicable_number<br>
    {
        static void Main(string[] args)<br>
        {<br>
            int num1, num2, sum1 = 0, sum2 = 0;<br>
            Console.WriteLine("\n---- Amicable numbers-----\n");<br>
            Console.Write("\n enter the first number:");<br>
            num1 = Convert.ToInt32(Console.ReadLine());<br>
            Console.Write("\n enter the SECOND number:");<br>
            num2 = Convert.ToInt32(Console.ReadLine());<br>
            for (int i = 1; i < num1; i++)<br>
            {<br>
                if (num1 % i == 0)<br>
                {<br>
                    sum1 += i;<br>
                }<br>
            }<br>
            for (int i = 1; i < num2; i++)<br>
            {<br>
                if (num2 % i == 0)<br>
                {<br>
                    sum2 += i;<br>
                }<br>
            }<br>
            if (sum1 == num2 && sum2 == num1)<br>
            {<br>
                Console.WriteLine("\n the numbers {0} and {1} are amiciable.", num1, num2);<br>
            }<br>
            else<br>
            {<br>
                Console.WriteLine("\n the numbers {0} and {1} are not amiciable.", num1, num2);<br>
            }<br>
        }<br>
    }<br>
}<br>
