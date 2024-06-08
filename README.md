import java.util.Scanner;

public class Main4 {

    public static void main(String[] args) {
    
    /* Koşullar :

        Sıcaklık 5'dan küçük ise "Kayak" yapmayı öner.
        Sıcaklık 5 ve 15 arasında ise "Sinema" etkinliğini öner.
        Sıcaklık 15 ve 25 arasında ise "Piknik" etkinliğini öner.
        Sıcaklık 25'ten büyük ise "Yüzme" etkinliğini öner.*/
        
        int sicaklik;
        Scanner input= new Scanner(System.in);
        
        
        System.out.print("Lutfen bir sıcaklık giriniz: ");
        sicaklik= input.nextInt();
        
        if(sicaklik<5){
            System.out.print("Kayak yapmaya gidebilirsiniz");
            
        } else if (sicaklik<=25) {
            if(sicaklik>=5 && sicaklik<15){
                System.out.print("Sinemaya gidebilirsiniz");
            }
            if(sicaklik>=15 && sicaklik<25){
                System.out.print("pikniğe gidebilirsiniz");
            }
        } else if (sicaklik>=25) {
            System.out.print("Yüzmeye gidebilirsiniz");

        }
        else {
            System.out.print("Yanlış tercih");
        }


    }

}
