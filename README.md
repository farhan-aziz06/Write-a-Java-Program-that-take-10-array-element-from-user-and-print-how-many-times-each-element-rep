# Write-a-Java-Program-that-take-10-array-element-from-user-and-print-how-many-times-each-element-rep
Write a Java Program that take 10 array element from user and print how many times each element repeated


        import java.util.Scanner;

        public class arrays {
            public static void main (String [] args){
                Scanner console = new Scanner(System.in);
                char [] character = new char[10];
                int size=0;
                int element = character[0];
                char[] unique = new char[size];
                int counter = 0;
                for (int i = 0; i<10; i++){
                    System.out.println("A["+i+"]");
                    character[i]=console.next().charAt(0);
                }
                for (int i =0; i<10; i++){
                    for (int j=0; j<10;j++){
                        if (character[i]==character[j]){
                            counter=counter+1;
                        }
                    }
                    System.out.println(character[i]+ " occurs"+counter+" times");
                    counter =0;
                }
            }
        }
