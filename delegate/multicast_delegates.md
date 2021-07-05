
#  multicast delegates 
Créée le mercredi 05 mai 2021


Doivent acvoir la même signature, appelle les methodes à la suite avec mêmes parametres

```cs
public void GetArea(double Width, double Height)
        {
            Console.WriteLine(@"Area is {0}", (Width * Height));
        }
public void GetPerimeter(double Width, double Height)
        {
            Console.WriteLine(@"Perimeter is {0}", (2 * (Width + Height)));
        }
Rectangle rect = new Rectangle();
RectangleDelete rectDelegate = new RectangleDelete(rect.GetArea);
rectDelegate += rect.GetPerimeter;
rectDelegate(23.45, 67.89);
```
