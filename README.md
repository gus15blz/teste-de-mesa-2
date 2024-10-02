using System;
namespace CalculadoraRendimento
{
    class Program
    {
        static void Main(string[] args)
        {
            // Valores iniciais
            double dinheiroInicial = 3800;
            double jurosPorMes = 1.25 / 100; int totalMeses = 6;
            // Mostrar o título da tabela
            Console.WriteLine("Mês\tDinheiro");
            //Calcular e mostrar o dinheiro a cada mês
            for (int mes = 1; mes <= totalMeses; mes++)
            {
                dinheiroInicial = dinheiroInicial * (1 + jurosPorMes);
                Console.WriteLine($"{mes}\tR${dinheiroInicial:F2}"); 
                Console.ReadLine();
            }

            for (int mes = 1; mes <= totalMeses; mes++)
            {
                dinheiroInicial = dinheiroInicial * (1 + jurosPorMes);
                Console.WriteLine($"{mes}\tR${dinheiroInicial:F2}");
                Console.ReadLine();
            }
        }
    }
}
