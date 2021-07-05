
#  1 - Task.run 
Créée le mercredi 05 mai 2021

Executes the function in a t**hreadPool**



```cs

Task t3 = Task.Run( () => {                                  
	for (i = 0; i <= 1000000; i++)  {}
 })

// Wait
t3.Wait();
```
