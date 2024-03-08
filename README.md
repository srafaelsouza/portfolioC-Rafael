using System;

class Program {
  static void Main(string[] args)
  {

      Console.WriteLine("Fibonacci");
      int n = int.Parse(Console.ReadLine());
      int pri = 0, seg = 1;
   
      for (int i = 0; i < n; i++)
      {
          if (i == 0 || i == 1)
          {
            Console.Write(i + " ");
          }
          else
          {
            int prox = pri + seg;
            Console.Write(prox + " ");
            pri = seg;
            seg = prox;
          }
      }
  }
}

