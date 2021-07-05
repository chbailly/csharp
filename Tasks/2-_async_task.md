
#  2- async task 
Créée le mercredi 05 mai 2021

```cs
public static async void callMethod()  
    {  
        Task<int> task = Method1();  
        Method2();  
		int count = await task; 
        Method3(count);  
    }  

public static async Task<int> Method1()  
    {  ''
        int count = 0;  
        await Task.Run(() =>  
        {  
            for (int i = 0; i < 100; i++)  
            {  
                Console.WriteLine(" Method 1");  
                count += 1;  
            }  
        });  
        return count;  
    }  
```