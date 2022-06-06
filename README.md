# Working-with-tables

﻿using System;

public class Program
{
    public static void Main()
    {
        char[] tablica;
        char zamiana;
        string nazwa;
        int n;

        Console.WriteLine("Podaj hasło");
        nazwa = Console.ReadLine();
        n = nazwa.Length;
        tablica = new char[n];
        tablica = nazwa.ToCharArray();
        zamiana = tablica[0];
        tablica[0] = tablica[n - 1];
        tablica[n - 1] = zamiana;
        Console.WriteLine(tablica);
    }
}
