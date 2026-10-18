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

### Homework7
```Java

public class Homework7 {
    public static void main(String[] args) {
        int[] num = new int[20];

        // 난수 20개 생성
        for (int i = 0; i < num.length; i++) {
            num[i] = (int)(Math.random() * 100);
        }
        // 정렬 전 출력
        System.out.println("정렬 전:");
        for (int i = 0; i < num.length; i++) {
            System.out.print(num[i] + " ");
        }
        // 선택 정렬
        for (int i = 0; i < num.length - 1; i++) {
            int min = i;
            for (int j = i + 1; j < num.length; j++) {
                if (num[j] < num[min]) {
                    min = j;
                }
            }
            int temp = num[i];
            num[i] = num[min];
            num[min] = temp;
        }
        // 정렬 후 출력
        System.out.println("\n정렬 후:");
        for (int i = 0; i < num.length; i++) {
            System.out.print(num[i] + " ");
        }
    }
}
```
<img width="340" height="111" alt="image" src="https://github.com/user-attachments/assets/017c4bb5-f74a-4703-9d04-1b1485233e2c" />

### Homework8

```Java
public class Homework8 {
    public static void main(String[] args) {
        int[][] score = new int[30][4];

        // 학생 10명의 과목별 성적 생성
        for (int i = 0; i < score.length; i++) {
            for (int j = 0; j < score[i].length; j++) {
                score[i][j] = (int)(Math.random() * 101);
            }
        }
        // 성적 출력 및 학생별 합계 계산
        for (int i = 0; i < score.length; i++) {
            int sum = 0;

            System.out.print((i + 1) + "번 학생: ");

            for (int j = 0; j < score[i].length; j++) {
                System.out.print(score[i][j] + " ");
                sum += score[i][j];
            }

            System.out.println("| 합계: " + sum);
        }
    }
}
```
<img width="192" height="387" alt="image" src="https://github.com/user-attachments/assets/03ded50a-e23e-42dc-bb3c-09e1bece107f" />

### Homework10
```Java
public class Homework10 {
    public static void main(String[] args) {
        int array_count, max_value, bin_size, display_scale, hist_size;

        if (args.length != 4) {
            System.out.println("실행 인자 4개를 입력하세요.");
            return;
        }

        array_count = Integer.parseInt(args[0]);
        max_value = Integer.parseInt(args[1]);
        bin_size = Integer.parseInt(args[2]);
        display_scale = Integer.parseInt(args[3]);

        hist_size = max_value / bin_size;

        int[] arr = new int[array_count];
        int[] hist = new int[hist_size];

        // 난수 데이터 생성
        for (int i = 0; i < array_count; i++) {
            arr[i] = (int)(Math.random() * max_value);
        }

        // 생성한 데이터 출력
        System.out.println("데이터:");
        for (int i = 0; i < array_count; i++) {
            System.out.print(arr[i] + " ");
        }
        System.out.println();

        // 구간별 데이터 개수 계산
        for (int i = 0; i < array_count; i++) {
            hist[arr[i] / bin_size]++;
        }

        // 도수분포표 출력
        System.out.println("도수분포표:");
        for (int i = 0; i < hist_size; i++) {
        	System.out.printf("%02d~%02d: ", i * bin_size,
                    (i + 1) * bin_size - 1);
        	
            for (int j = 0; j < hist[i] / display_scale; j++) {
                System.out.print("#");
            }

            System.out.println(" (" + hist[i] + ")");
        }
    }
}
```





