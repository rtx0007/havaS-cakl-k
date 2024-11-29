package Exercise;

import java.util.Scanner;

public class havaSıcaklıgı {
    public static void main(String[] args) {
        int sıcaklık;

        Scanner input = new Scanner(System.in);
        System.out.print("Hava sıcaklığını giriniz: ");
        sıcaklık = input.nextInt();
        System.out.println("Hava sıcaklığı: " + sıcaklık + "°C");
        input.close();

        if (sıcaklık < 5) {
            System.out.println("Kayak yapabilirsiniz");
        } else if (sıcaklık < 25) {
            if (sıcaklık <= 15 && sıcaklık >= 5) {
                System.out.println("Sinema yapabilirsiniz");
            }
            if (sıcaklık <= 25 && sıcaklık >= 10) {
                System.out.println("Piknik yapabilirsiniz");
            }
        } else if (sıcaklık >= 25) {
            System.out.println("Yüzme yapabilirsiniz");
        }


    }
}
