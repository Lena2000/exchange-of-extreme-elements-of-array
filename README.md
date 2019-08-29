package javaapplication21;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class JavaApplication21 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
         
        int i;
        System.out.println("Input size of array: ");
        int kol=sc.nextInt();
        int[]array=new int[kol];
       
        System.out.println("Input elements of array: ");
        for( i=0; i<kol; i++)
           array[i]=sc.nextInt();
        
        int a=array[0];
        int b=array[kol-1];
        for(i=0; i<kol; i++){
            array[0]=b;
            array[kol-1]=a;
        
        }
        System.out.println("Result");
        for( i=0; i<kol; i++)
            System.out.print(array[i]+" ");
        
    }
    
}
