# coins

 double coins = double.Parse(Console.ReadLine());
            double allCoins = coins * 100;
            int coinsCount = 0;
            while (allCoins >= 1)
            {
                if (allCoins >= 200)
                {
                    allCoins -= 200;
                    coinsCount++;
                }
                else if (allCoins >= 100)
                {
                    allCoins -= 100;
                    coinsCount++;
                }
                else if (allCoins >= 50)
                {
                    allCoins -= 50;
                    coinsCount++;
                }
                else if (allCoins >= 20)
                {
                    allCoins -= 20;
                    coinsCount++;
                }
                else if (allCoins >= 10)
                {
                    allCoins -= 10;
                    coinsCount++;
                }
                else if (allCoins >= 5)
                {
                    allCoins -= 5;
                    coinsCount++;
                }
                else if (allCoins >= 2)
                {
                    allCoins -= 2;
                    coinsCount++;
                }
                else if (allCoins >= 1)
                {
                    allCoins -= 1;
                    coinsCount++;
                }
            }
            Console.WriteLine(coinsCount);
