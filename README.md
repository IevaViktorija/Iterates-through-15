# Iterates-through-15
# Pirmais variants
```java
public class Main {
    public static void main(String[] args) {
        for (int i = 0; i <= 15; i++) {
            if (i % 3 == 0 && i % 5 == 0) {
                System.out.println("WoTech");
            } else if (i % 3 == 0) {
                System.out.println("Wo");
            } else if (i % 5 == 0) {
                System.out.println("Tech");
            }
        }
    }
}
```
# Otrais variants
```java
import java.util.Scanner;

public class Main {
  public static void main(String[] args) {

    Scanner scanner = new Scanner(System.in);
    System.out.println("Please enter a number: ");

    int number = scanner.nextInt(); //15

    for(int i = 1; i <= number; i++){
      // 1 2 3 4 5 ... 15

      // 7
      String result = "";
      if (i % 3 == 0){ //15
        result += "Wo"; //Add Wo to the result
      } 
      if (i % 5 == 0){ // 5 10 15
        result += "Tech";
      } 
      
      if (result == ""){ 
        //result = String.valueOf(i); //Then result = i (number)
        System.out.println(i);
      }else{
        System.out.println(result);
      }
      
      

      scanner.close();
    }
  }
}
```
