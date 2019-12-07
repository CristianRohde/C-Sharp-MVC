# C-Sharp-MVC
Modelo MVC 
using System;

namespace Aula01
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");// Console é o mesmo que SystemAut do Java serve para imprimir na tela
            Console.WriteLine("Tudo bem!!!"); // para escrever Console.WriteLine(); só digitar Cw e presionar tab tab
            float nota1 = 7.5f;
            float nota2 = 5.0f; // tem que declarar o tipo da nota ao final
            float nota3 = 5.0f;
            float nota4 = 4.0f;
            float nota5 = 9.0f;
            int divisor = 5;
            string entrada;

            //rescrevendo os valores
            Console.WriteLine("Digite a nota 1: ");
            entrada = Console.ReadLine(); // serve para pedir ao usuario algum dado
            nota1 = float.Parse(entrada); // ele salva na variavel e converte de string para float
            

            Console.WriteLine("Digite a nota 2: ");
            entrada = Console.ReadLine();
            nota2 = float.Parse(entrada);

            Console.WriteLine("Digite a nota 3: ");
            entrada = Console.ReadLine();
            nota3 = float.Parse(entrada);

            Console.WriteLine("Digite a nota 4: ");
            entrada = Console.ReadLine();
            nota4 = float.Parse(entrada);

            Console.WriteLine("Digite a nota 5: ");
            entrada = Console.ReadLine();
            nota5 = float.Parse(entrada);

            

            Console.WriteLine("A média é " + CalculaMedia(nota1,nota2,nota3,nota4,nota5, divisor));// chamando o metodo para calcular e imprimindo na tela
        }

        static float CalculaMedia(float n1, float n2, float n3, float n4, float n5, int m)
        {
            float media = (n1+n2+n3+n4+n5) / m;
            return media;

           // int media2 = int.Parse(media.ToString());
            

        }
    }
}
