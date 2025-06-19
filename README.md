using System;

class Program
{
    static void Main()
    {
        int dogruSayisi = 0;

        Console.WriteLine("Kim Milyoner Olmak İster? 🚀");
        Console.WriteLine("2 cevap şıklı 3 sorumuz var. En az 2'sini doğru bilirseniz 1 Milyon TL kazanırsınız!\n");

        // Soru 1
        Console.WriteLine("1) Kızınca tüküren hayvan hangisidir?");
        Console.WriteLine("a) Lama  b) Deve");
        Console.Write("Cevabınız: ");
        string cevap1 = Console.ReadLine();

        if (cevap1.ToLower() == "a")
        {
            dogruSayisi++;
            Console.WriteLine("Doğru!\n");
        }
        else
        {
            Console.WriteLine("Yanlış!\n");
        }

        // Soru 2
        Console.WriteLine("2) Dünya'ya en yakın gezegen hangisidir?");
        Console.WriteLine("a) Venüs  b) Mars");
        Console.Write("Cevabınız: ");
        string cevap2 = Console.ReadLine();

        if (cevap2.ToLower() == "a")
        {
            dogruSayisi++;
            Console.WriteLine("Doğru!\n");
        }
        else
        {
            Console.WriteLine("Yanlış!\n");
        }

        // Soru 3 (her durumda sorulmalı)
        Console.WriteLine("3) 5 * 2 + 8 / 2 - 2 işleminin sonucu kaçtır?");
        Console.WriteLine("a) 7  b) 12");
        Console.Write("Cevabınız: ");
        string cevap3 = Console.ReadLine();

        if (cevap3.ToLower() == "b")
        {
            dogruSayisi++;
            Console.WriteLine("Doğru!\n");
        }
        else
        {
            Console.WriteLine("Yanlış!\n");
        }

        // Final sonucu
        if (dogruSayisi >= 2)
        {
            Console.WriteLine("🎉 Tebrikler! 1 Milyon TL'lik büyük ödülü kazandınız! 🏆");
        }
        else
        {
            Console.WriteLine("😔 Üzgünüz, büyük ödülü kazanamadınız.");
        }
    }
}
