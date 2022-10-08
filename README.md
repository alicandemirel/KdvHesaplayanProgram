//KdvHesaplayanProgram

import  java.util.Scanner;

public class KdvHesaplayanProgram {

    public static void main(String[] args) {

        double tutar;

        Scanner inp = new Scanner(System.in);

        System.out.print("Ürünün fiyatını giriniz: ");
        tutar = inp.nextInt();

        boolean sonuc = tutar<1000;


        String str = sonuc ? "Ürünün KDV' siz fiyatı: " + tutar + "\nÜrünün KDV tutarı: " + tutar*0.18 + "\nÜrünün KDV' li fiyatı: " + tutar*1.18
                :"Ürünün KDV' siz fiyatı: " + tutar +", "+ "\nÜrünün KDV tutarı: " + tutar*0.08 + "\nÜrünün KDV' li fiyatı: " + tutar*1.08;

        System.out.print(str);
    }
}
