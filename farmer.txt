import java.util.*;
public class FarmerField {
    public static void main(String[] args) {
        System.out.println("Enter length and width of field in feet.");
        Scanner sc= new Scanner(System.in);
        int length= sc.nextInt();
        int width= sc.nextInt();
        System.out.println("Area of field in acres is "+ (length*width)/43560);
        sc.close();
    }
}
