import java.util.Scanner;

public class LOGIN {
    public static void main(String[] args) {
        Scanner bbit = new Scanner(System.in);
        int maxTries =3;
        for(int attempt =1;attempt<=maxTries;attempt++){
            System.out.print("Enter username:");
            String usernameInput= bbit.nextLine();
            System.out.print("Enter password:");
            String passwordInput= bbit.nextLine();
                    if
            (isValidLogin(usernameInput, passwordInput)){
                System.out.println("Login successful!");
            }else{
                System.out.println("Invalid username or password. Try again.Attempts left: "+( maxTries-attempt));
            }
        }
       bbit.close();
    }
    private static String
            getPasswordInput(Scanner bbit){
                char[] passwordchars= System.console(). readPassword("Enter password:");
                return new
         String(passwordchars);
            }
            private static boolean
                    isValidLogin(String username, String password){
                        return
                                username.equals("your_username")&& password.equals("your_password");
                                
                    }
    }
   
