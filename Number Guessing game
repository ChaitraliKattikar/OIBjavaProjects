import java.util.Scanner;

public class numberGuessing {
    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);

        int number = (int)(Math.random()*100);

        int usernumb = 0;

        do{
            System.out.println("Guess the number(1-100): ");
            usernumb = sc.nextInt();

            if(usernumb == number  ){
                System.out.println("WOHHO.... Correct number!!");
                break;
            }

            else if(usernumb > number ){
                System.out.println("The number is too large .....please try again!");

            }
            else{
                System.out.println("The number is too smalll... please try agian!");
            
            }
        }
        while(usernumb >= 0);
            System.out.println("The Number Was  ");
            System.out.println(number);

    }
    
}
