import java.util.*;
public class MarksSecured {
 public static void main(String[] args) {
    Scanner sc= new Scanner(System.in);
    System.out.println("Enter the marks in Physics, Chemistry, Maths, English and Computer Science");
    double Physics= sc.nextDouble();
    double Chemistry= sc.nextDouble();
    double Maths= sc.nextDouble();
    double English= sc.nextDouble();
    double Computer= sc.nextDouble();

    double percentage= ((Physics+ Chemistry+Maths+English+Computer)/500)*100;
    if(percentage>90){
        System.out.println("A");
    }else if(percentage<90 && percentage>80){
        System.out.println("B");
    }else if(percentage<80 && percentage>70){
        System.out.println("C");
    }else{
        System.out.println("E");
    }
    sc.close();
   
 }

}
