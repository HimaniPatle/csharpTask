# csharpTask

namespace HelloWorld
{
public class Program
{
public static void Main(string[] args)
{
string str = Console.ReadLine();
while (str.Length > 0)
{
 Console.Write(str[0] + " - ");
 int cal =0;
 for(int j = 0; j < str.Length; j++)
 {
   if (str [0] == str[j])
   {
     cal++;
   }
 }
 Console.WriteLine(cal);
 str = str.Replace(str[0].ToString(), string.Empty);
}
Console.ReadLine();
}
}
}

using System;
using System.Linq;

namespace LogicalPrograms
{
    class Program
    {
        static void Main(string[] args)
        {
            string str = Console.ReadLine();
            
            string revWordString = string.Join(" ", str
            .Split(' ')
            .Select(x => new String(x.Reverse().ToArray())));

            Console.WriteLine($" {revWordString}");
            Console.ReadKey();
        }      
    }
}
