# compile-time polymorphism
package main;


/**
 *

 */
public class Main {
    public int addition(int x,int y){
        return x+y;
    }
public int addition(int x,int y,int z){
    return x+y+z;
    
}
public double addition(double x,double y){
    return x+y;
    
}
    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        Main number=new Main();
        int res1=number.addition(444,555);
        System.out.println("Addition of two integers:" +res1);
        
        int res2=number.addition(333,555,777);
        System.out.println("Addition of three integers:" +res2);
        
        double res3=number.addition(20.5,72.3);
        System.out.println("Addition of two doubles:" +res3);
        // TODO code application logic here
    }
    
}
OUTPUT:




Addition of two integers:999
Addition of three integers:1665
Addition of two doubles:92.8
BUILD SUCCESSFUL (total time: 0 seconds)






