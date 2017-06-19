# HW_Scope-and-AccessModifiers
Watch read and practice from the module: Logical Operators, Scope and Access Modifiers  Write your understanding of the topic using comments and examples (at least 10 examples) to the instructor and describe them in your own words to the best of your knowledge. Put your work to GIT. Submit the GIT url to canvas. 

(Reccommened to view this in its .cs file.)

1.

//Those "curly braces" that we have used and talked about in class, those are actually called "scopes". Using scopes can help to organize scripts/codes so the whole thing doesn't look like (and doesn't have to operate) in ONE. LONG. LINE. If it were, it could still function without scopes, but it would more confusing.

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
