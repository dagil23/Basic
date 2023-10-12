# Basic
Algunos programas básicos en C#
using System;
namespace ejemplo
{
    class Program
    {
        static void Main()
        {
           Random numero = new Random();
           int numeroAleatorio = numero.Next(0,100);
           Console.WriteLine("Escribe un Nº entre el 0, 100");
           int numeroUsuario;
           int intentos = 0;
           

           do
           {

            intentos++;

            numeroUsuario = int.Parse(Console.ReadLine()??"1");
            if (numeroAleatorio > numeroUsuario) Console.WriteLine($"El Nº aleatorio es mas mayor");
            if (numeroAleatorio < numeroUsuario) Console.WriteLine($"El Nº aleatorio es menor");


           } while (numeroAleatorio != numeroUsuario) ;

           
Console.WriteLine($"Haz tardado {intentos} en conseguir el mismo numero que la consola ");

           

        }
    }
}

