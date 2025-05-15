# Branching-Assignment-Submission
using System;

class Program
{
    static void Main()
    {
        
        Console.WriteLine("Welcome to Package Express. Please follow the instructions below.");

        
        Console.Write("Please enter the package weight: ");
        
        double weight = Convert.ToDouble(Console.ReadLine());

        
        if (weight > 50)
        {
            
            Console.WriteLine("Package too heavy to be shipped via Package Express. Have a good day.");
            return; 
        }

       
        Console.Write("Please enter the package width: ");
        double width = Convert.ToDouble(Console.ReadLine());

        
        Console.Write("Please enter the package height: ");
        double height = Convert.ToDouble(Console.ReadLine());

        
        Console.Write("Please enter the package length: ");
        double length = Convert.ToDouble(Console.ReadLine());

        
        double dimensionTotal = width + height + length;

        
        if (dimensionTotal > 50)
        {
            
            Console.WriteLine("Package too big to be shipped via Package Express.");
            return; // End program
        }

        
        double volume = width * height * length;

        
        double quote = (volume * weight) / 100;

       
        Console.WriteLine("Your estimated total for shipping this package is: ${0:F2}", quote);

       
        Console.WriteLine("Thank you!");
    }
}

