import java.util.Scanner;

public class ATMinterface {
    static String name;
    static int id ;
    static int pin;
    static int  withdraw = 0;
    static int deposit = 0;
    static String transactionHistory = " ";
    static boolean flag = false;
    static int transaction=0;
    static float balance = 100000;
    public static void register(){
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter Your Name :");
        name = sc.nextLine();
        System.out.println("Enter ID :");
        id = sc.nextInt();
        System.out.println("Enter pin :");
        pin = sc.nextInt();
        System.out.println("Registration completed succesfully!!....Kindly login to your Account");
       }
       public static void login(){
        Scanner sc = new Scanner(System.in);
            System.out.println("Enter your id :");
            int id1 = sc.nextInt();
            System.out.println("Enter Your pin :");
            int pin1 = sc.nextInt();
            if(id1 == id && pin1 == pin){
                        System.out.println("Logined successfull!!");
                        flag=true;
                    }else{
                        System.out.println("Incorrect id or pin");
                    }
                }
       public static void withdraw(){
        System.out.println("Enter Ammount to be withdrawn :");
        Scanner sc = new Scanner(System.in);
        float amount = sc.nextFloat();

        if(balance >= amount){
            balance -= amount;
            System.out.println("Withdrawal Successfully!");
            System.out.println("After withdrawing " + amount +"Rupees Your Current balance is "+balance+" Rupees");
            transaction++;
            transactionHistory.concat(amount+" Rupees withdraw from your account");
        }
        else{
            System.out.println("Insufficient balance");
        }
        }

       public static void deposit(){
        System.out.println("Enter amount to deposite :");
        Scanner sc = new Scanner(System.in);
        float amount = sc.nextFloat();
      
            balance+=amount;
            System.out.println("After depositing " + amount +" Rupees Your Current balance is "+balance+" Rupees");
            transaction++;
            transactionHistory.concat(amount+" Rupees deposited into your account");
            }
       
       public static void transfer(){
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter Recipent's Name :");
        String recipents = sc.nextLine();
        System.out.println("Enter amount to transfer :");
        float amount = sc.nextFloat();
       
            if(balance >= amount){
                transaction++;
                balance -= amount;
                System.out.println("Successfully transferd to " +recipents);
                transaction++;
                transactionHistory.concat(amount+" Rupees transferred from your account");
            }
            else{
                System.out.println("Sorry ...Insufficient balance!");
            }
        }
       
       public static void  checkbalnce(){
        System.out.println("Your current balance is " +balance+"Rs");
       }
       public static void transactionHistory(){
        if(transaction>0){
            System.out.println("You have performed "+transaction+" transactions");
            System.out.println("Transaction Details :");
            System.out.println(transaction);
        }else{
            System.out.println("No transactions are performed");
        }
       }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
       System.out.println("WELCOME TO ATM SERVICES!!");
       System.out.println("1. Register");
       System.out.println("2. Exit");
       System.out.println("Enter Your Option!!");
       int option = sc.nextInt();
       if(option==1){
        register();
        System.out.println("Choose an option");
        System.out.println("1. Login");
        System.out.println("2. Exit");
        int ch = sc.nextInt();
        if(ch == 1){
            login();
            while(flag == true){
                System.out.println("Choose an option");   
                System.out.println("1. Transaction history");
                System.out.println("2. Withdraw");
                System.out.println("3. Deposite");
                System.out.println("4. Transfer");
                System.out.println("5. Exit"); 
                int choice = sc.nextInt();
                switch(choice){
                    case 1:
                    transactionHistory();
                    break;
                    case 2:
                    withdraw();
                    break;
                    case 3:
                    deposit();
                    break;
                    case 4:
                    transfer();
                    break;
                    case 5:
                    checkbalnce();
                    break;
                    case 6 :
                    flag = false;
                    System.out.println("Collect Your Card!!");
                    break;
                    default:
                    System.out.println("please select valid option");
                }
            }
        }
        else{
            System.out.println("Please collect your card"); 
            System.exit(0);
        }
    }
       
       else{
        System.out.println("Please collect your card"); 
            System.exit(0);
        }
    }
}
    
    

