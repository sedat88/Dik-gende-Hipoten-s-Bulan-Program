# Dik ücgende-Hipotenüs-Bulan-Program
Ödev
import java.util.Scanner;
public class Main {
    public static void main (String[]orgs) {
        // Değişenlerimizi oluşturuyoruz.
        int a, b;
        double c,u,UcgenAlan,UcgenCevre;

        // Kullanıcıdan verileri alıyoruz.
        Scanner sonuc = new Scanner(System.in);
        System.out.print("1.Kenarı giriniz : ");
        a = sonuc.nextInt();
        System.out.print("2. Kenarı giriniz : ");
        b = sonuc.nextInt();
        //Hipotenüsün hesaplanması.
        c = Math.sqrt((a*a) + (b*b));
        System.out.println("Hipetenüs : " + c);

        //Üçgenin alan hesabı.
        u=(a+b+c)/2;
        System.out.println("Üçgenin alanı: "+u);
        UcgenAlan=Math.sqrt(u*(u-a)*(u-b)*(u-c));
        System.out.println("Üçgen alan hesabı: " +UcgenAlan);

        //Üçgenin çevresinin hesaplanması.
        UcgenCevre = 2*u;
        System.out.println("Üçgenin çevresi: " +UcgenCevre);

    }



}
