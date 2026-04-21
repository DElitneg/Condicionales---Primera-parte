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

// 4. Aprobación de Examen:


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Introduzca la nota del examen . . . ");

            Double nota;
            nota = Convert.ToDouble(Console.ReadLine());

            if (nota >= 7)
            {
                Console.WriteLine("Promocionado");
            }    

            else 
            {
                    if (nota < 7)
                    {
                        if (nota > 4)
                        {
                            Console.WriteLine("A finales");
                        }

                        else
                        {
                            if (nota < 5)
                            {
                                Console.WriteLine("Recuperatorio");
                            }
                        }
                    }
                }
            }
    }
}


// 5. Calculadora de Descuentos:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Monto total de la compra: ");

            Double monto;
            monto = Convert.ToDouble(Console.ReadLine());

            Double descuento;
            descuento = (monto / 100) * 15;

            double total;
            total = monto - descuento; 

            if (monto <= 5000)
            {
                Console.WriteLine("El monto total es " + monto +"$");
            }   

            else 
            {
                    if (monto > 5000)
                    {
                    Console.WriteLine("El monto total es de " + total + "$ con un descuento del 15% ");
                     
                    }
                }
            }
    }
}

// 6. Login Simple:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Nombre de Usuario: ");

            String nombre;
            nombre = Console.ReadLine();


            Console.WriteLine("Contraseña: ");

            int contraseña;
            contraseña = Convert.ToInt32(Console.ReadLine());

            if(contraseña == 1234)
            {
                Console.WriteLine("Acceso Concedido, " + nombre);
            }
            else
            {
                Console.WriteLine("Error de credenciales ");
            }

        }
      }
}

// 7. Clima de Montaña:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {

            Console.WriteLine("Temperatura Actual:");
            int temperatura;
            temperatura = Convert.ToInt32(Console.ReadLine());

            if(temperatura <= 0)
            {
                Console.WriteLine("Peligro de congelamiento ");
            }
            else if (temperatura <= 15)
            {
                if(temperatura > 0)
                {
                    Console.WriteLine("Mucho frío");
                }
            }
            else if(temperatura > 15)
            {
                Console.WriteLine("Clima agradable");
            }

        }
    }
}


// 8. Múltiplos de 5:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {

            Console.WriteLine("Numero Entero:");
            int numero;
            numero = Convert.ToInt32(Console.ReadLine());

            if(numero%5 == 0)
            { 
                Console.WriteLine("Es divisible por 5 ");
            }
            else
            {
                Console.WriteLine("No es divisible por 5 ");
            }
           

        }
    }
}


// 9. Diferencia de edad:


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {

            Console.WriteLine("Edad del primer hermano:");
            int edadprimero;
            edadprimero = Convert.ToInt32(Console.ReadLine());

            Console.WriteLine("Edad del segundo hermano:");
            int edadsegundo;
            edadsegundo = Convert.ToInt32(Console.ReadLine());

            int diferencia1;
            diferencia1 = edadprimero - edadsegundo;
           
            if(edadprimero > edadsegundo)
            {
                diferencia1 = (diferencia1 * diferencia1) / diferencia1;
                Console.WriteLine("El primer hermano es el mayor por " + diferencia1 + " años");
            }
            else if (edadsegundo > edadprimero)
            {
                diferencia1 = diferencia1 * -1;
                Console.WriteLine("El segundo hermano es el mayor por " + diferencia1 + " años");
            }
            else if (edadprimero == edadsegundo)
            {
                Console.WriteLine("Ambos tienen la misma edad");
            }


        }
    }
}


// 10. Presupuesto de Obra:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {

            Console.WriteLine("Presupuesto disponible:");
            int presupuesto;

            presupuesto = Convert.ToInt32(Console.ReadLine());

            Console.WriteLine("Costo de los materiales:");
            int materiales;
            materiales = Convert.ToInt32(Console.ReadLine());
            int dineroFaltante;
            dineroFaltante = materiales - presupuesto;

            if (materiales > presupuesto)
            {
                Console.WriteLine("Faltan " + dineroFaltante + "$ para pagar el costo de los materiales");
            }
            else
            {
                Console.WriteLine("It's all fine then");
            }      

        }
    }
}
