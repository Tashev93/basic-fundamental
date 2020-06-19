# coins

      double coinsInput = double.Parse(Console.ReadLine());
            double coinCount = 0;
            double coins = coinsInput * 100;
            while (coins >= 1)
            {
                coinCount++;
                if(coins >= 200)
                {
                    double num = Math.Floor(coins / 100);
                    double twoCoinsCount = Math.Floor(num / 2);
                    double rem = num % 2;

                    coinCount += twoCoinsCount;
                    coinCount--;

                    coins %= 100;
                    coins = coins + (rem * 100);

                }
                else if (coins >= 100)
                {
                    coins -= 100;
                }
                else if (coins >= 50)
                {
                    coins -= 50;
                }
                else if (coins >= 20)
                {
                    coins -= 20;
                }
                else if (coins >= 10)
                {
                    coins -= 10;
                }
                else if (coins >= 5)
                {
                    coins -= 5;
                }
                else if (coins >= 2)
                {
                    coins -= 2;
                }
                else if (coins >= 1)
                {
                    coins -= 1;
                }

            }
            Console.WriteLine(coinCount);
