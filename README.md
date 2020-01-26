# sumandAverage
sum and average using method in java
import java.util.Scanner;

public class Main {
    public static Scanner sn=new Scanner(System.in);
    public static void main(String[] args) {
        int[] myIntegers=getInteger(5);
        for(int i=0;i<myIntegers.length;i++) {
            System.out.println(" element " + i + ",typed values was" + myIntegers[i]);
        }
        System.out.println("the average is "+getAverage(myIntegers));

   }
   public static int[] getInteger(int number){
       System.out.println("enter"+number+"integer values.\r");
       int[] values =new int[number];
       for(int i=0;i<values.length;i++){
           values[i]=sn.nextInt();

       }
       return values;
   }
   public static double getAverage(int[] array){
        int sum=0;
        for(int i=0;i<array.length;i++){
            sum+=array[i];
        }
        int len= array.length;
        return (double) sum/len;

   }
}

