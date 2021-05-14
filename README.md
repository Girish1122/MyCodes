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

********************************************************************************************************************************************************************************

2) Interface assignment:-

public interface IVehicle
{
  public void drive();
  public void turnLeft();
  public void brake();
}
public interface IPublicTransport
{
    public void getNumberOfPeople();
}
class MotorisedVehicle
{
  public void checkMotor()
  {
    System.out.println ("the motor of vehicle is in good condition");
  }
}
class car extends MotorisedVehicle implements IVehicle
{
  public void drive()
  {
      System.out.println ("this car is in driving condition");
  }
  public void turnLeft()
  {
       System.out.println ("this car can turn left");
  }
  public void brake()
  {
       System.out.println ("the car is in brake mode");
  }
  
}
class train implements IVehicle,IPublicTransport
{
    public void drive()
  {
      System.out.println ("this train is in driving condition");
  }
  public void turnLeft()
  {
       System.out.println ("this train can't turn left");
  }
  public void brake()
  {
       System.out.println ("the train is in brake mode");
  }
   public void getNumberOfPeople()
  {
    System.out.println ("This train contains 100 people");   
  } 
    
}
public class Main
{
  public static void main (String args[])
  {
    MotorisedVehicle o1=new MotorisedVehicle();
    o1.drive();
    o1.turnLeft();
    o1.brake();
    train o2=new train();
    o2.drive();
    o2.turnLeft();
    o2.brake();
    o2.getNumberOfPeople();
  }
}

*********************************************************************************************************************************************************************************

3) Date and time API assignment:-

import java.time.LocalDate;
public class Main
{
	public static void main(String[] args)
	{
	    LocalDate today=LocalDate.now();
	    int day=today.getDayOfMonth();
	    int m=today.getMonthValue();
	    LocalDate dob=LocalDate.of(2021,05,14);
	    int dobday=dob.getDayOfMonth();
	    int dobmonth=dob.getMonthValue();
	    
	    if(dobday==day && dobmonth==m)
	   {
	       System.out.println("Today is your birthday.....Happy Birthday!!");
	   }
	    if(dobday==day && dobmonth==m)
	   {
	       System.out.println("Today is day of paying a bill");
	   }
	   
		//System.out.println("Hello World");
	}
}

