# Lab-2-1
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Введiть поштовий iндекс:");
        string input = Console.ReadLine();
        int postalCode;

        // Перевіряємо, чи вхідні дані є дійсним числом
        if (int.TryParse(input, out postalCode))
        {
            string city;

            switch (postalCode)
            {
                case 58000:
                    city = "Чернiвцi";
                    break;
                case 79000:
                    city = "Львiв";
                    break;
                case 01000:
                    city = "Київ";
                    break;
                case 61000:
                    city = "Харкiв";
                    break;
                case 54000:
                    city = "Миколаїв";
                    break;
                case 33000:
                    city = "Рiвне";
                    break;
                case 46000:
                    city = "Тернопiль";
                    break;
                case 89000:
                    city = "Ужгород";
                    break;
                case 99000:
                    city = "Сiмферополь";
                    break;
                case 74000:
                    city = "Херсон";
                    break;
                default:
                    city = "Невiдомий поштовий iндекс";
                    break;
            }

            Console.WriteLine($"Мiсто для поштового iндексу {postalCode}: {city}");
        }
        else
        {
            Console.WriteLine("Будь ласка, введiть дiйсний поштовий iндекс.");
        }
    }
}
