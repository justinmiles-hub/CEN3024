# CEN3024
Creating new repository 
import java.util.Scanner;

//Author Name: Justin Miles
//Date: 9/1/2019
//Program Name: Miles_Drone
//Purpose: Simulation using button, drone movement in x,y,z location



public class Miles_Drone
{
		
	public static void main(String args[])
	{
		int x = 0;
		int y = 0;
		int z = 0;
		String s = null;
				
		for (int i =1; i<=1000; i++)
		 {
			Scanner input = new Scanner(System.in);
			
		System.out.println("Which direction would you like to move the drone?");
		System.out.println("1 - Move Up");
		System.out.println("2 - Move Down");
		System.out.println("3 - Move Foward");
		System.out.println("4 - Move Backward");
		System.out.println("5 - Move Left");
		System.out.println("6 - Move Right");
		System.out.println("7 - Display Position");
		System.out.println("8 - Exit Navigation");
		
		int b = input.nextInt();
		
		 if ( b == 1) 
		{
			y++;
			System.out.println("You have moved forward");
		}
		  if ( b == 2) 
		{
			y--;
			System.out.println("You have moved backward");
		}
		  if ( b == 3) 
		{
			z++;
			System.out.println("You have moved up");
		}
		 else if ( b == 4) 
		{
			z--;
			System.out.println("You have moved down");
		}
		  if ( b == 5) 
		{
			x--;
			System.out.println("You have moved left");
		}
		  if ( b == 6) 
		{
			x++;
			System.out.println("You have moved right");
		}
		  if (x > y)
		  {
			  s = "East";
		  }
		  if (x < y)
		  {
			  s = "West";
		  }
		  if (y > x)
		  {
			  s = "North";
		  }
		  if (y < x)
		  {
			  s = "East";
		  }
		  
		 if ( b ==7)  
		{
			System.out.println("Miles_Drone[x_pos=" + x + ", y_pos=" + y + ", z_pos=" + z + ", orientation=" + s +"]");
		}
		 
		 if (b == 8)
		 {
			 System.exit(0);
		 }
		 
		 }
	}

}
