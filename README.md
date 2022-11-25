import java.util.Scanner;

public class Main {
    public static void main(String[] args){


        Scanner scanner = new Scanner(System.in);
        System.out.println("День рождения:");
        int day = scanner.nextInt();
        if (day>31 ) {
            System.out.println("ощибка");
        }
        System.out.println("Месяц рорждения:");
        int month = scanner.nextInt();
        if (month>12) {
            System.out.println("ощибка");
        }
        System.out.println("Год рорждения:");
        int year = scanner.nextInt();
       if (year>2022) {
           System.out.println("ощибка");
       }
        int naw_years = 2022;
        int years = (naw_years - year) *365;
        int naw_months = 11;
        int months = naw_months - month;
        float mont = (float) ((float) months*30.5);
        int naw_days =26;
        int days = naw_days-day;
        int overall = (int) (years + mont + days);
        int age_year = overall/365;
        int a = overall%365;
        int age_month = a/30;
        int age_day = a%30;
        System.out.println(age_year+"лет ," + age_month +"месяцев и " +age_day +"Дней");
    }

}
