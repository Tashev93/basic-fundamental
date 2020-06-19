specialnumbers

int n = int.Parse(Console.ReadLine());
          for(int i = 1111; i <= 9999; i++)
            {
                bool isSpecial = true;
                int num2 = i;
                while (num2 != 0)
                {
                    double num = num2 % 10;
                     num2 = num2 / 10;
                    
                    if(num == 0 || n % num != 0)
                    {
                        isSpecial = false;
                        break;
                    }
                    
                }
                if (isSpecial)
                {
                    Console.Write($"{i} ");
                }
            }
