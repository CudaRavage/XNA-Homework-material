using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Week1
{
    class Program
    {
        static void Main(string[] args)
        {

            Console.WriteLine(                                                       // welcome message
                "=================================================" +
                "\nWelcome to shell physics computation program v1.0" +
                "\n=================================================");

            Console.Write("\nPlease enter the initial angle of the shell in degrees: ");     // take user input for initial angle
            float degree = float.Parse(Console.ReadLine());


            Console.Write("\nPlease enter the intial speed of the shell: ");    // take user input for initial speed
            float speed = float.Parse(Console.ReadLine());

            float theta = degree * 0.0174532925f;  // convert user input degrees to radians 

            float vox = speed * (float)Math.Cos(theta);      // x component of the velocity at start
            float voy = speed * (float)Math.Sin(theta);      // y component of the velocity at start
            float g = 9.8f;                                  // gravity m/s squared
            float t = voy / g;                               // time until shell reaches apex
            float h = voy * voy / (2 * g);                   // height of shell at apex
            float dx = vox * 2 * t;                          // distance shell travels horizontally (assuming launch and target elevations are equal)

            Console.WriteLine("\nMaximum shell height: " + h.ToString("N3") + " meters");  // print max height
            Console.WriteLine("\nShell distance traveled: " + dx.ToString("N3") + " meters"); // print distance traveled

            Console.ReadKey(); // wait for key-press before closing
        }
    }
}
