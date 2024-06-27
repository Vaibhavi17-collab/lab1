import java.util.*;
public class SumOfn {
public static void main(String[] args) {
    System.out.println("Enter the number upto which you want to find the sum.");
   Scanner sc= new Scanner(System.in);
    int n= sc.nextInt();
     System.out.println("The sum upto n is "+ (n*(n+1)/2));
     sc.close();
}    
}
