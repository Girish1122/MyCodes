# VirtusaTraining1122
GitHub account for Girish's Virtusa Training
1) Abstract class assignment:-

abstract class Shape
{
  public abstract void CalculateArea ();
  public void SetColor (String col)
  {
    System.out.println ("Color is:"+col);
  }
}
class circle extends Shape
{
  double r = 5.0;
  public void CalculateArea ()
  {
    System.out.println ((double) 3.14 * r * r);
  }
 
}
class square extends Shape
{
  int l = 4, b = 4;
  public void CalculateArea ()
  {
    System.out.println (l * b);
  }

}
public class Main
{
  public static void main (String args[])
  {
    circle o1 = new circle ();
    square o2 = new square ();
      o1.CalculateArea ();
      o1.SetColor ("Blue");
      o2.CalculateArea ();
      o2.SetColor ("Green");
  }
}



