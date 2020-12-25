# java-program
largest among 3
import java.util.*;
class Placement{
public static void main(String[] args) 
{
    int x,y ,z ;
    Scanner sc= new Scanner(System.in) ;
    System.out.println( "Enter the no of students placed in CSE: " );
    x=sc.nextInt( );
    System.out.println("Enter the no of students placed in ECE:" );
    y=sc.nextInt( ) ;
    System.out.println("Enter the no of students placed in MECH:" );
    z=sc.nextInt( ) ;
    if(x==z && x==y && y==z)
    {   
    System.out.println("None of the department has got the highest placement" ) ;
    }
    else if(x<0 || y<0 || z<0)
    {
    System.out.println("Input is Invalid" ) ;
    }
    else
    {
        System.out.println( "Highest placement" );
        
        if(x>=z && x>=z)
        {
        System.out.println("CSE");
            if(x==y)
            {
            System.out.println("ECE");
            }
            else if(x==z)
            {
                System.out.println("MECH");
            }
            
        }
        else if(y>=x && y>=z)
        {
            System.out.println("ECE");
            if(y==x)
            {
                System.out.println("CSE");
            }
            else if(y==z)
            {
              System.out.println("MECH");  
            }
        }
        else if(z>=x && z>=y)
        {
            System.out.println("MECH");
            if(z==x)
            {
                System.out.println("CSE");
            }
            else if(z==y)
            {
                System.out.println("MECH");
            }
            
        }
    }
}
}
