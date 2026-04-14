# Condicionales---Primera-parte
10 ejercicios


// 1. Control de Velocidad:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication2
{
    class Program
    {
        
        static void Main(string[] args)
        {
            Console.WriteLine("A cuantos km/h esta yendo el vehiculo ");
            int velocidad;
            velocidad = Convert.ToInt32(Console.ReadLine());

            if (velocidad > 120)
            {
                Console.WriteLine("Multa en camino: Exceso de velocidad");
            }
            if (velocidad == 120)
            {
                Console.WriteLine("Conque al limite eh? (*saca el rifle FAL 39x20mm*)");
            }

            else if (velocidad < 120)
            {
                Console.WriteLine("Conducción segura");
            }                
        }
    }
}
