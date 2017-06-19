# HW_Scope-and-AccessModifiers
Watch read and practice from the module: Logical Operators, Scope and Access Modifiers  Write your understanding of the topic using comments and examples (at least 10 examples) to the instructor and describe them in your own words to the best of your knowledge. Put your work to GIT. Submit the GIT url to canvas. 

(Reccommened to view this in its .cs file.)

1.

//Those "curly braces" that we have used and talked about in class, those are actually called "scopes". Using scopes can help to organize scripts/codes so the whole thing doesn't look like (and doesn't have to operate) in ONE. LONG. LINE. If it were, it could still function without scopes, but it would more confusing. So as the first example, we only see "public int Coin = 0;" in the scope (the "curly braces" / "{}") of the script's class.

public class Scopes : MonoBehaviour
{
  public int Coin = 0; 
}


2.

//In the next example, a void has been included, with 'print("2nd Scope Set");'. As obvious this may sound, if I were to ask you what is the scope of the print function, the answer would be the void "void Start()", because it has its own scope. Another way to easily tell what the scopes are holding, press tab to create an indent WHILE WITHIN the "curly braces", and do this every time a new scope is created.

public class Scopes : MonoBehaviour
{
  public int Coin = 0;
  
  void Start()
  {
    print("2nd Scope Set");
  }
}

3.

//Once again for example, if I were to ask what is the scope of "print(true);", it would be the "if(2 + 2 == 4)".

public class Scopes : MonoBehaviour
{ 
  public int Coin = 0;
  
  void Start()
  { 
    if(2 + 2 == 4)
    {
      print(true);
    }
    else
    {
      print(false);
    }
  }
}

4. 

//
