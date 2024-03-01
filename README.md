using System;
					
public class Program
{
	public static void Main()
	{
Console.WriteLine("Напиши височината:");
            
double height = double.Parse(Console.ReadLine());
Console.WriteLine("Напиши килограми");
            
double weight = double.Parse(Console.ReadLine());
 
double smqtane = weight / ((height / 100) * (height / 100));

double smqtaneprint = Math.Round(smqtane, 0);
Console.WriteLine(smqtaneprint);

if (smqtaneprint < 20)
{
Console.WriteLine("Под нормалното тегло.");
}
else if (smqtaneprint <= 25)
{
Console.WriteLine("Теглото ви е стабилно");
}
else
{
Console.WriteLine("Наднормено тегло ");
}
}
}
