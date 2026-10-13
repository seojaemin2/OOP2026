# OOP2026
### Homework1
```Java
public class Homework1{
  public static void main(String []args){
    int i, j;
    for(i=0; i<10; i++) {
      for(j=0; j<=i; j++) {
        System.out.print("#");
      }
      System.out.println("");
    }
  }
}
```
<img width="340" height="205" alt="image" src="https://github.com/user-attachments/assets/90e677b9-fa63-4298-82ff-85d41d27c901" />

```Java
public class Homework1{
  public static void main(String []args){
    int i, j;
    for(i=0; i<10; i++) {
      for(j=i; j<10; j++) {
        System.out.print("#");
      }
      System.out.println("");
    }
  }
}
```
<img width="339" height="205" alt="image" src="https://github.com/user-attachments/assets/384bd742-5d4c-4110-bbd5-dde4731e148b" />

```Java
public class Homework1 {
    public static void main(String[] args) {
        int i, j;
        for (i = 1; i <= 10; i++) {
            // 공백 출력
            for (j = 1; j <= 10 - i; j++) {
                System.out.print(" ");
            }
            // # 출력
            for (j = 1; j <= i; j++) {
                System.out.print("#");
            }
            System.out.println();
        }
    }
}
```
<img width="266" height="168" alt="image" src="https://github.com/user-attachments/assets/24585fec-3c7f-4381-9968-4d6b87685ae3" />

```Java
public class Homework1 {
    public static void main(String[] args) {
        int i, j;
        for (i = 1; i <= 10; i++) {
            // 공백 출력
            for (j = 1; j < i; j++) {
                System.out.print(" ");
            }
            // # 출력
            for (j = 10; j >= i; j--) {
                System.out.print("#");
            }
            System.out.println();
        }
    }
}
```
<img width="205" height="166" alt="image" src="https://github.com/user-attachments/assets/126883f3-0578-42fa-b8a8-397718e6f5b4" />

### Homework2
```Java
public class Homework2 {
    public static void main(String[] args) {
        int a = 1;
        int b = 1;
        int c;

        System.out.print(a + " " + b + " ");

        for (int i = 3; i <= 20; i++) {
            c = a + b;
            System.out.print(c + " ");

            a = b;
            b = c;
        }
    }
}
```
<img width="448" height="155" alt="image" src="https://github.com/user-attachments/assets/b88eea37-125d-48f3-8518-a962d758bf3d" />

### Homework3
```Java
public class Homework3 {
    public static void main(String[] args) {
        int a = 1;
        int b = 1;
        int c;

        for (int i = 1; i <= 20; i++) {
            c = a + b;

            double ratio = (double) c / b;
            System.out.println(c + "/" + b + "=" + ratio);

            a = b;
            b = c;
        }
    }
}
```
<img width="227" height="272" alt="image" src="https://github.com/user-attachments/assets/5fe869bf-c2c8-44c3-a210-92c41a2a7207" />

### Homework4
```Java

public class Homework4 {
    public static void main(String[] args) {
        int i, j;

        for (i = 1; i <= 9; i++) {
            for (j = 1; j <= 9; j++) {
                System.out.print(j + "*" + i + "=" + (j * i) + "\t");
            }
            System.out.println();
        }
    }
}
```
<img width="410" height="166" alt="image" src="https://github.com/user-attachments/assets/ca78f34b-b8b2-49e6-83bb-497258c0f1ec" />

### Homework5
```Java

public class Homework5 {
    public static void main(String[] args) {
        double pi = 0.0;

        for (int i = 0; i < 100000; i++) {
            if (i % 2 == 0) {
                pi += 4.0 / (2 * i + 1);
            } else {
                pi -= 4.0 / (2 * i + 1);
            }
        }

        System.out.println("원주율: " + pi);
    }
}
```
<img width="192" height="98" alt="image" src="https://github.com/user-attachments/assets/af838eb6-3430-43a5-8b75-583e1ebee0b5" />

```Java
public class Homework5Madhava {
    public static void main(String[] args) {
        double sum = 1.0;

        for (int i = 1; i < 100; i++) {
            sum += Math.pow(-1, i) /
                   ((2 * i + 1) * Math.pow(3, i));
        }

        double pi = Math.sqrt(12) * sum;

        System.out.println("원주율: " + pi);
    }
}
```
<img width="206" height="98" alt="image" src="https://github.com/user-attachments/assets/b398afd2-166b-4b41-83f3-e6a87165738f" />

### Homework6
```Java

public class Homework6 {
    public static void main(String[] args) {
        int binomial[][] = new int[11][11];

        for (int i = 0; i <= 10; i++) {
            binomial[i][0] = 1;
            binomial[i][i] = 1;

            for (int j = 1; j < i; j++) {
                binomial[i][j] = binomial[i - 1][j - 1]
                               + binomial[i - 1][j];
            }
        }

        for (int i = 0; i <= 10; i++) {
            for (int j = 0; j <= i; j++) {
                System.out.print(binomial[i][j] + " ");
            }
            System.out.println();
        }
    }
}
```
<img width="229" height="188" alt="image" src="https://github.com/user-attachments/assets/fe7fd2d4-7500-4acb-b07a-999c48f75e0b" />






