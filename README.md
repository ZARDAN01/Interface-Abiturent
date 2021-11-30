# Interface-Abiturent
import java.util.Scanner;

 abstract class Student implements Abiturent {
     Scanner in = new Scanner(System.in);

        void name() {
            System.out.printf("Имя: \n");
            String nam = in.nextLine();
            System.out.println("Имя " + nam);
        }

        void famile() {
            System.out.printf("Фамилия: \n");
            String famil = in.nextLine();
            System.out.println("Фамилия " + famil);
        }
        static String VishiUchebZaved = ("ENU") ;
       static  String UchebProgpamm = ("InfoBez");








     }




import java.util.Scanner;

public interface Abiturent {
    Scanner in = new Scanner(System.in);

    default void SborDoki() {
        Scanner in = new Scanner(System.in);
        System.out.print("Собираем документы ");
        System.out.printf("Введите какие документы нужны : \n");
        String nam = in.nextLine();
        System.out.println("Список документов" + nam);

    }


    default void Oplatit() {
        Scanner in = new Scanner(System.in);
        System.out.print("Оплачиваем учебу ");
        System.out.printf("ВВедите какую сумму надо оплатить чтобы учится : \n");
        String nam = in.nextLine();
        System.out.println("Необходимая сумма " + nam);


    }


    default void SdatDoki() {
        Scanner in = new Scanner(System.in);
        System.out.print("Сдаем документы ");
        System.out.printf("Укажите дату и место где нужно доставить документы : \n");
        String nam = in.nextLine();
        System.out.println("Документы нужно сдать" + nam);
    }


    default void Zaiava() {
        Scanner in = new Scanner(System.in);
        System.out.print("Пишем заявление ");
        System.out.printf("Распишитесь свойм именем: \n");
        String nam = in.nextLine();
        System.out.println("Роспись" + nam);

    }


    default void SdatENT() {
        Scanner in = new Scanner(System.in);
        System.out.print("Сдаем ЕНТ ");
        System.out.printf("укажите ваш выбранный предмет на ЕНТ: \n");
        String nam = in.nextLine();
        System.out.println("Предмет " + nam);

    }
}

 
 
import java.util.Scanner;

public class StudentZaochnik extends Student  {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        new StudentZaochnik().name();
        new StudentZaochnik().famile();
        new StudentZaochnik().SborDoki();
       new StudentZaochnik().Zaiava();
       new StudentZaochnik().SdatENT();
       new StudentZaochnik().SdatDoki();
       new StudentZaochnik().Oplatit();
        System.out.println("Нужна стипендия если есть выход я готов на все просто дайте знать $$$"+ VishiUchebZaved+ UchebProgpamm);
        System.out.println("87767042002");

    }

}

