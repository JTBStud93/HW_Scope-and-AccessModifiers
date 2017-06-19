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

//Now onto Access Modifiers (as of this class, we're only focusing on "Public" & "Private").

4. 

//The main purpose of the "Public" Access Modifier, is to make the functions within the script to appear in Unity's Inspector window; and for it to interact with other scripts. For now, here's for the Inspector. In this example, we see that the "int Coin = 0;" has been set to public, therefore it can be seen in Unity's Inspector, and (within Unity) the value of "Coin" can easily be changed.

public class AccessModifiers : MonoBehaviour
{
  public int Coin = 0; 
}

5.

//But what if you change Coin's value in the .cs/C# script? Now the value of "Coin" is defaulted to 5. (For me, after I save the script file, I go back into Unity, and nothing seems to have changed. But after you assinged the script to a GameObject, and see it in the Inspector, There should be a little "gear icon", click on it, then click reset. Now "5" should be the default number according to Unity.)

public class AccessModifiers : MonoBehaviour
{
  public int Coin = 5; 
}

6.

//The purpose of the "Private" Access Modifier is to help you, other users & scripts, from accidentally messing with the current script/code that you're working with. It also prevents it from functions being seen in Unity's Inspector.

public class AccessModifiers : MonoBehaviour
{
  private int Coin = 0; 
}

7.

//An alternate (but un-reccommended) way to make a function Private, is by not using any Access Modifier at all. Its preferred to actually type "Private" before a function, so it doesn't look like its just some random code sitting in your script, not doing anything at all.

public class AccessModifiers : MonoBehaviour
{
  int Coin = 0; 
}

8.

public class ScopeAccess : MonoBehaviour
{

  public int Health = 100;
  
  void Attack()
  {
    
    
    void SwordAttack()
    {
      if (SwordAttack > EnemyDefense)
      {
        EnemyHealth.addDamage();
      }
      else
      {
        EndTurn();
      }
    } 
  }
}

9.

public class ScopeAcess : MonoBehaviour
{

  public int Dollars = 44
  private float Cents = 0.95

}

10.

public class ScopeAccess : MonoBehavior
{
    public bool MrPresident = true;

    void Start()
    {
      if(true)
      {
        print("Here are the Top Secret files Mr. President.");
      }
      else
      {
        print("Sorry, but this information is classified");
      }
    }
}
