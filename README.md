# rotation-of-array-elements
import java.util.*;

public class Rotation{

  public static void main (String args[])

  {

    Scanner sc=new Scanner(System.in);

    int i,r1,l1,n;

    System.out.println("Enter l1 value:");

    l1=sc.nextInt();

    System.out.println("Enter r1 value:");

   r1=sc.nextInt();

    System.out.println("Enter n value:");

    n=sc.nextInt();

   int br[]=new int[n];

   int cr[]=new int[n];

    int ar[]=new int[n];

    System.out.println("Enter array elements:");

    for(i=0;i<n;i++)

    {

      ar[i]=sc.nextInt();

    }

    

    System.out.println(" ");

      for( i=0;i<n;i++)

      {

         if((i-r1)<0)

         {

            br[i]=ar[n+i-r1];

         }

         else 

         br[i]=ar[i-r1];

      }

      for(i=0;i<n;i++)

      System.out.print(br[i]);

      System.out.println(" ");

      for( i=0;i<n;i++)

      {

         if((i-l1)<0)

         {

            cr[n+i-l1]=br[i];

         }

         else 

         cr[i-l1]=br[i];

      }

      for(i=0;i<n;i++)

      System.out.print(cr[i]);

  }

}
