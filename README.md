# Csharp
Trick to C# programing

<p>Csharp just like many other OOP(object oriented programming) language, has a similar declaration, variable, function, and etc. And the use of this repository just to keep note to myself about the basic fundamental of C#.</P>

Function
<p>Inorder to call function from the Main function, we need to ever create a STATIC FUNCTION or OBJECT REFERENCE.This might be confusing, but let get it an example.</p>
<br></br>
1. Static Function<br>
  using System;<br>
    class T<br>
    {<br>
      static void Main()<br>
      {<br>
        ....;<br>
        ....;<br>
        int result = add(5,3);<br>
      }<br>
      public static int add(int a, int b)<br>
      {<br>
        ....;<br>
      }<br>
    }<br>
  
  <p>In this class, the function add would be static because of keyword static. But why we need to do add the keyword static in      the function? This is because in C# the function do not exist independently, instead, they exist in the context of an           object. So only the instance of class T know how to add. And that the object reference come in.</p>

2.Object Reference
  To create an object reference, we need the class T. So it would be 

  T pro = new T();<br>
  int result = pro.add(5,3);<br>
  
  This way, we don't need the keyword static.
