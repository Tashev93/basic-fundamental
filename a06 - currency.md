# Currncy
            Console.Write("Enter your amount of money: ");
            double inPutNum = double.Parse(Console.ReadLine());
            Console.Write("Enter your currency:(EUR, USD, GBP, BGN): ");
            string inPutValue = Console.ReadLine();
            Console.Write("Enter the exchange currancy(EUR, USD, GBP, BGN): ");
            string outPutValue = Console.ReadLine();
            double inBG = 0;
            if (inPutValue == "EUR")
            {
                inBG = inPutNum * 1.95;
            }
            else if (inPutValue == "USD")
            {
                inBG = inPutNum * 1.81;
            }
            else if (inPutValue == "GBP")
            {
                inBG = inPutNum * 2.24;
            }
            else if (inPutValue == "BGN")
            {
                inBG = inPutNum;
            }
            double result = 0;
            if (outPutValue == "EUR")
            {
                result = inBG * 0.51;
            }
            else if (outPutValue == "USD")
            {
                result = inBG * 0.55;
            }
            else if (outPutValue == "GBP")
            {
                result = inBG * 0.45;
            }
            else if (outPutValue == "BGN")
            {
                result = inBG;
            }
            Console.WriteLine($"{result:F2}");
