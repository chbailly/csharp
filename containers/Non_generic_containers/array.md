
#  array 
Créée le mercredi 05 mai 2021


C'est non dynamique (comme array basic en C..), non resizable)

```cs
		 int []  n = new int[10]; /* n is an array of 10 integers */
	
		
		 foreach (int j in n ) {
			int i = j-100;
			Console.WriteLine("Element[{0}] = {1}", i, j);
		 }
```
