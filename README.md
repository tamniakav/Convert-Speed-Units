# Convert-Speed-Units
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Convert_Speed_Units
{
    class Program
    {
        static void Main(string[] args)
        {
            float meters = float.Parse(Console.ReadLine());
            float hours = float.Parse(Console.ReadLine());
            float minutes = float.Parse(Console.ReadLine());
            float seconds = float.Parse(Console.ReadLine());

            
                hours *= 60f;
                minutes += hours;
                minutes *= 60f;
                seconds += minutes;

                meters /= seconds;
            
            Console.WriteLine(meters);

            float kmPerHour = (meters * 3600) / 1000f;

            Console.WriteLine(kmPerHour);

            float milePerHour = (meters * 3600) / 1609f;

            Console.WriteLine(milePerHour);
           
        }
    }
}
