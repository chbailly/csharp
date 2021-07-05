
#  event 
Créée le mercredi 05 mai 2021


```cs
   public delegate string MyDel(string str); ''**//the delegate to be used**
	
   class EventProgram {
      event MyDel MyEvent;  //An event is declared a delegate
		
      public EventProgram() {
         this.MyEvent += new MyDel(this.WelcomeUser);
      }''
      public string WelcomeUser(string username) {
         return "Welcome " + username;
      }''
      static void Main(string[] args) {
         EventProgram obj1 = new EventProgram();
         string result = obj1.MyEvent("Tutorials Point");
         Console.WriteLine(result);
      }
   }

```