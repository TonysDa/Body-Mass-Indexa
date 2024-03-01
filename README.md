using System;
					
public class Program
{
	public static void Main()
	{
            Console.WriteLine("Напиши височината:");
            double height = double.Parse(Console.ReadLine());
            Console.WriteLine("Напиши килограми");
            double weight = double.Parse(Console.ReadLine());
            double bmi = weight / ((height / 100) * (height / 100));
            double bmiprint = Math.Round(bmi, 0);
            Console.WriteLine(bmiprint);
            if (bmiprint < 20)
            {
                Console.WriteLine("Под нормалното тегло.");
            }
            if (bmiprint >= 20 && bmiprint <= 25)
            {
                Console.WriteLine("Теглото ви е стабилно");
            }
            else if (bmiprint > 25)
            {
                Console.WriteLine("Наднормено тегло ");
            }
}
}
