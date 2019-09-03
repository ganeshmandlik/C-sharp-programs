# C-sharp-programs


Sort an array in ascending order without using inbuilt C# function

We will create a simple one integer array having values 2,9,4,3,5,1,7 in the array as described in the following example. We will take two for loops; first, a for loop for checking the first position of an array and iterating the length of the array.  The second loop starts with the i+1 position and iterates the length of the array.



    using System;  

    namespace SortArrayExample  
    {  
        class Program  
        {  
            static void Main(string[] args)  
            {  
                int[] intArray = new int[] {2,9,4,3,5,1,7 };  
                int temp = 0;  

                for (int i = 0; i <= intArray.Length-1; i++)  
                {  
                    for (int j = i+1; j < intArray.Length; j++)  
                    {  
                        if (intArray[i] > intArray[j])  
                        {  
                            temp = intArray[i];  
                            intArray[i] = intArray[j];  
                            intArray[j] = temp;  
                        }  
                    }  
                }  
                Console.WriteLine("Array sort in asscending order");  
                foreach (var item in intArray)  
                {  
                    Console.WriteLine(item);  
                }  
                Console.ReadLine();  
            }  
        }  
    }  


-------------------------------------OUTPUT----------------------------------------

Array sort in asscending order

1
2
3
4
5
7
9





=======================================================================================================================

Example 2
 
Sort an array in descending order without using inbuilt C# function. 

using System;  
  
        namespace SortArrayExample  
        {  
            class Program  
            {  
                static void Main(string[] args)  
                {  
                    int[] intArray = new int[] {2,9,4,3,5,1,7 };  
                    int temp = 0;  

                    for (int i = 0; i <= intArray.Length-1; i++)  
                    {  
                        for (int j = i+1; j < intArray.Length; j++)  
                        {  
                            if (intArray[i] < intArray[j])  
                            {  
                                temp = intArray[i];  
                                intArray[i] = intArray[j];  
                                intArray[j] = temp;  
                            }  
                        }  
                    }  
                    Console.WriteLine("Array sort in descending order");  
                    foreach (var item in intArray)  
                    {  
                        Console.WriteLine(item);  
                    }  
                    Console.ReadLine();  
                }  
            }  
        }  
