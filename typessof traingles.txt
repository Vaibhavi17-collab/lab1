import java.util.Scanner;
public class TypeOfTriangle {
    public static void main(String[] args) {
       Scanner scanner= new Scanner(System.in);
        System.out.println("Enter the lengths of the three sides of the triangle:");
        double a = scanner.nextDouble();
        double b = scanner.nextDouble();
        double c = scanner.nextDouble();
        
        // Sort the sides so that a <= b <= c
        if (a > b) {
            double temp = a;
            a = b;
            b = temp;
        }
        if (b > c) {
            double temp = b;
            b = c;
            c = temp;
        }
        if (a > b) {
            double temp = a;
            a = b;
            b = temp;
        }
        
        // Check the type of triangle
        if (a + b <= c) {
            System.out.println("The given sides do not form a triangle.");
        } else {
            double a2 = a * a;
            double b2 = b * b;
            double c2 = c * c;
            
            if (a2 + b2 == c2) {
                System.out.println("The triangle is a right-angle triangle.");
            } else if (a2 + b2 > c2) {
                System.out.println("The triangle is an acute-angle triangle.");
            } else {
                System.out.println("The triangle is an obtuse-angle triangle.");
            }
        }
        
        scanner.close();
    }
}
