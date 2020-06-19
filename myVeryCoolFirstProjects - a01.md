# powerNum


            int a = int.Parse(Console.ReadLine());
            int b = int.Parse(Console.ReadLine());
     
                Console.WriteLine(GetPow(a, b));

                Console.ReadLine();
            }
            static int GetPow(int baseNum, int powNum)
            {
                int result = 1;
                for (int i = 0; i < powNum; i++)
                {
                    result = result * baseNum;

                }
                return result;
