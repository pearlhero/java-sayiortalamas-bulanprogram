# java-sayiortalamas-bulanprogram
java-sayiortalamasıbulanprogram

import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int k, total = 0, numbers =0;

        System.out.print("Sayı giriniz : ");
        k = input.nextInt();

        for (int i = 0; i <= k; i++){
            if ((i % 12 == 0)){
                numbers += 1;
                total += i;
            }
        }

        if (numbers > 0){
            double ort = total / numbers;
            System.out.println("Sayıların ortalaması: " + ort);
        } else {
            System.out.println("Sayı bulunamadı.");
        }
    }
}
