public class base_operations {
    public static void main(String[] args) {
        int n = 10;
        int a = 6, b = a + 3;

        System.out.println(a+b); // базовые операторы + - * /
        System.out.println(a-b);
        System.out.println(a*b);
        System.out.println(a/b);

        System.out.println("");

        for(int i = 0; i < n; i++) { // каждый раз, когда счетчик будет четным или наоборот числа а и b обновляются 
            if(i%2==0){
                a+=1;
            }
            else{
                b+=1;
            }
        }
        System.out.println(a);
        System.out.println(b);
    }

}

import java.util.Scanner;
public class switch_case {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        System.out.print("Input a number: "); // определение дня недели
        int day = in.nextInt();
        if (day > 7) { // так как всего 7 дней в неделе используем проверку на число. если больше - условие не выполнется и выведет ошибку
            System.out.println("Wrong number!");
        } else {
            switch (day) {
                case 1:
                    System.out.println("Monday");
                    break;
                case 2:
                    System.out.println("Tuesday");
                    break;
                case 3:
                    System.out.println("Wednesday");
                    break;
                case 4:
                    System.out.println("Thursday");
                    break;
                case 5:
                    System.out.println("Friday");
                    break;
                case 6:
                    System.out.println("Saturday");
                    break;
                case 7:
                    System.out.println("Sunday");
            }

        }
    }
}

