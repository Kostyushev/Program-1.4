Program-1.4
===========
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1_1
{
class Program
{
static void Main(String[] args)
{
Console.Write("Введите два слова: ");
String twowords = Console.ReadLine();
String[] words = twowords.Split(' ');
Char[] first = words[0].ToArray();
Char[] second = words[1].ToArray();
Console.WriteLine(words[0]);
Int32 k = 0;
for (Int32 i = 0; i < first.Length; ++i)
{
for (Int32 j = 0; j < second.Length; j++)
{
if (first[i].Equals(second[j]))
{
Console.Write("да ");
}
else { k += 1; }
}
if (k != 0)
{
if (i != first.Length - 1)
{
Console.Write("нет ");
k = 0;
}
}
}

Console.ReadLine();
}
}
}
