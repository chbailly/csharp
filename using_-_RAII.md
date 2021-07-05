
#  using - RAII 
Créée le jeudi 06 mai 2021


```c#
class ResourceHolder : IDisposable
{
   public ResourceHolder()
   {
       // acquire resource here
   }

   public void Dispose()
   {
       // release resource
   }
}


using(var holder = ResourceHolder())
{
   // use resource and do other stuff as well
}
```
