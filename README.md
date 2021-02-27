double a, b, c, D, x1, x2;
        bool h = true;
        while (h == true) ;
        try
        {
            Console.WriteLine("Введите a");
            a = Convert.ToDouble(Console.ReadLine());
            Console.WriteLine("Введите b");
            b = Convert.ToDouble(Console.ReadLine());
            Console.WriteLine("Введите c");
            c = Convert.ToDouble(Console.ReadLine());

            if (b == 0)
            {
                Console.WriteLine("Ошибка");
            }
            else
            {
                D = Math.Pow(b , 2 ) - 4 * a * c;

                if (D >= 0)
                {
                    x1 = (-b + Math.Sqrt(D)) / (2 * a);
                    x2 = (-b - Math.Sqrt(D)) / (2 * a);
                    Console.WriteLine("x1 = " + x1);
                    Console.WriteLine("x2 = " + x2);
                }
                else
                {
                    Console.WriteLine("Уравнение не имеет корней");
                }

                h = false;

                Console.ReadKey();
            }
        }
        catch { Console.WriteLine("Некореетный ввод"); }
        finally { Console.WriteLine("Конец программы"); }
