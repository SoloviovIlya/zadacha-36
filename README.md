// Задайте одномерный массив, заполненный случайными числами. Найдите сумму элементов, стоящих на нечётных позициях.
//[3, 7, 23, 12] -> 19
//[-4, -6, 89, 6] -> 0

void Nechet(int[] a, int n)

{

    int m = 0;
    
    for (int i=0;i<n;i++)
    
    {
    
       if (i%2 != 0)
       
       {
        m = m+a[i];
       }
       
    }
    
    Console.WriteLine($"Сумма элементов, стоящих на нечётных позициях равна {m}");
    
}

int n = new Random().Next(5,11);

int[] a = new int[n];

for (int i = 0; i<n; i++)

{

    a[i] = new Random().Next(-100,101);
    
    Console.WriteLine(a[i]);
    
}

Nechet(a, n);

