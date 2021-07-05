
#  delegate 
Créée le mercredi 05 mai 2021


public delegate int MyDelegate (string s);

```c#
public delegate void printString(string s);

printString ps1 = new printString(WriteToScreen);
printString ps2 = new printString(WriteToFile);
```
