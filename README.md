# projeto2
Exercício de fixação 
using System;
using System.Globalization;
namespace Program
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine(" Entre com o seu nome completo ");
            string fullname = Console.ReadLine();
            Console.WriteLine(" Quantos quartos tem a sua casa ?");
            int quarto = int.Parse(Console.ReadLine());
            Console.WriteLine("Entre com o preço do produto");
            double produto = double.Parse(Console.ReadLine(), CultureInfo.InvariantCulture);
            Console.WriteLine("Entre com seu ultimo nome, idade e altuta ( mesma linha )");

            string[] vet = Console.ReadLine().Split(' ');
            string nome = vet[0];
            int idade = int.Parse(vet[1]);
            double altura = double.Parse(vet[2], CultureInfo.InvariantCulture);
            Console.WriteLine(  "        ");
            Console.WriteLine(fullname);
            Console.WriteLine(quarto);
            Console.WriteLine(produto.ToString("F2", CultureInfo.InvariantCulture));
            Console.WriteLine(nome);
            Console.WriteLine(idade);
            Console.WriteLine(altura.ToString("F2", CultureInfo.InvariantCulture));
        }
      }
