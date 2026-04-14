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


// 2. El Club de la Pelea (Ingreso):

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
            Console.WriteLine("Cual es su Nombre? ");
            String nombre;
            nombre = Console.ReadLine();
            Console.WriteLine("Cuantos años tenes vos? ");
            int edad;
            edad = Convert.ToInt32(Console.ReadLine());

            if (edad >= 18)
            {
                Console.WriteLine("Bienvenido al club, " + nombre);
            }
            else if (edad < 18)
            {
                Console.WriteLine("Lo siento, eres muy polluelo para esto");
            }
        }
    }
}

// 3. Par o Impar:


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
            Console.WriteLine("Introduzca un Numero entero ");

            int numero;
            numero = Convert.ToInt32(Console.ReadLine());

            if (numero%2 == 0) { Console.WriteLine("Es Par"); }
            else { Console.WriteLine("Es impar"); } 
        }
    }
}
