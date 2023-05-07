# Day5-project
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int []arr={2,33,4,33,1,2,6,7};
         int []longest={4,7,8};
           hello();
           compineSt("Rawan","Ali");
           System.out.printf("the greatest num"+Th_max(10,5,6));
           avr_s(20,34,67);
           calc(60,70);
           countVowels("Rawan will be a strong programmer");
           Th_max(7,9,9);
           System.out.println("the uniq num is"+uniq(arr));
           sp_lite("just keep going");
    }
    public static int[] hello(){
        System.out.println("Hello world!");

        return new int[0];
    }
    public static  String compineSt(String s1,String s2){
        String s3=s1+s2;
        System.out.println("the combiend Name:"+s3);
        return s3;
    }
    public static  int Th_max(int n1,int n2,int n3){
        int greatest1;
        greatest1 =Math.max(n1,n2);
        int greatest2=Math.max(greatest1,n3);

        return greatest1;
    }

    public static int avr_s(int num1, int num2, int num3){
        int sum=num1+num2+num3;
        int avr=sum/3;
        System.out.printf("The Result"+avr);
        return avr;
    }
  //
    public static int calc(int nn,int mm){
      Scanner s=new Scanner(System.in);
      System.out.println("Enter on of these operatain :+ * % /");
     char opr=s.next().charAt(0);
        System.out.println("enter number 1:");
        int n1=s.nextInt();
        System.out.println("enter number 2:");
        int n2=s.nextInt();
      switch (opr){
          case '+':
              System.out.println("The result addition"+nn+mm);
              break;
          case '*':
              System.out.println("The result multiplication"+nn*mm);
              break;
          case '/':System.out.println("The result divided"+nn/mm);
            break;
          case '%':System.out.println("The result mode"+nn%mm);
          break;
          default:
              System.out.println("Wrong operatin");
      }return opr;

  }

//  /س
    public static int[] uniq(int[]arr) {
        int[] arra = {1, 3, 33, 3, 3, 4, 4, 4, 3, 6, 7, 88, 88, 7, 0, 9};
        int n;
        for (int u = 0; u <= arra.length; u++) {
            int c = 0;
            for (int j = 0; j <= u; j++) {
                if (j == arra[u]) {

                    System.out.println("it is  not a uniqe numnber");
                    c++;
                } else {
                    System.out.printf("Not uniqe", c);
//              return c;
                }
            }
            //the vowel letter challange
            public static int countVowels (String str)
            {
                int vowelCount = 0;

                for (int i = 0; i < str.length(); i++) {
                    if (str.toLowerCase().toCharArray()[i] == 'a' | str.toLowerCase().toCharArray()[i] == 'e' | str.toLowerCase().toCharArray()[i] == 'i' | str.toLowerCase().toCharArray()[i] == 'o' | str.toLowerCase().toCharArray()[i] == 'u') {
                        vowelCount++;
                    }
                }
                return vowelCount;
            }
            // the lastl challange
            public static void sp_lite (String last){
                for (int sp = 0; sp <= last.charAt('j'); sp++) {
                    System.out.println("" + last.split(""));
                }
            }
        }
    }}
