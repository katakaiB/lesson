using System;
using System.Linq;

class Program
{
    static void Main()
    {
        // Пример массива целых чисел
        int[] numbers = { 10, 5, 20, 7, 3, 15, 8, 4, 9, 6 };
        
        // Задание а) Заменить элементы, кратные 10, на 0
        numbers = numbers.Select(x => x % 10 == 0 ? 0 : x).ToArray();
        
        // Задание б) Удвоить нечетные элементы, четные уменьшить вдвое
        numbers = numbers.Select(x => x % 2 == 0 ? x / 2 : x * 2).ToArray();
        
        // Задание в) Уменьшить нечетные элементы на m, увеличить элементы с нечетными номерами на n
        int m = 3; // Пример значения m
        int n = 2; // Пример значения n
        numbers = numbers
            .Select((x, i) => (i % 2 == 0 ? x + n : x - m))
            .ToArray();
        
        // Вывод результата
        Console.WriteLine("Результат: " + string.Join(", ", numbers));
    }
}
