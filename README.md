# Lab-6
Sentence
package lab_2;  

import java.util.Scanner;  

public class lab4 {  

    public static void main(String[] args) {  

        String cumle;  
        System.out.println("Cumle giriniz:");  
        Scanner input = new Scanner(System.in);  
        cumle = input.nextLine();  
        System.out.println("Cumleniz: " + cumle);  
        
        String kelimeler[] = cumle.split(" "); 
        int toplamKarakter = 0; 
        
        for (String kelime : kelimeler) {  
            toplamKarakter += kelime.length();  
            
            String degisenKelime = kelime.substring(0, 1).toUpperCase() + kelime.substring(1).toLowerCase();  
            System.out.println("Degisen kelime: " + degisenKelime);  
            
            if (kelime.length() < 4) {  
                System.out.println("Kısa kelime: " + kelime);  
            }  
            
            String tersKelime = new StringBuilder(degisenKelime).reverse().toString(); 
            System.out.println("Ters kelime: " + tersKelime);  
        }  

        System.out.println("Toplam karakter: " + toplamKarakter); 
    }  
}
