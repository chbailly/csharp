
#  LINQ 
Créée le mercredi 05 mai 2021


##  Sur IEnumerable<T> 

```cs
static void Main()

    {

        // Specify the data source.
        int[] scores = new int[] { 97, 92, 81, 60 };

        // Define the query expression.
        IEnumerable<int> scoreQuery =
            from score in scores
           where score > 80
            select score;

        // Execute the query.
        foreach (int i in scoreQuery)
        {''
            Console.Write(i + " ");
        }''
    }''
```