# my-firs-prosect1
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);

        int n = in.nextInt(), m = in.nextInt(), i, j;
        int[][] arr = new int[n][m];

        // Считываем элементы массива размером n x m
        for (i = 0; i < arr.length; i++)
            for (j = 0; j < arr[i].length; j++)
                arr[i][j] = in.nextInt();

        // Проходим по всему массиву и ищем отрицательные элементы
        for (i = 0; i < arr.length; i++) {
            for (j = 0; j < arr[i].length; j++) {
                if (arr[i][j] < 0) {
                    // Если элемент отрицательный, выводим его координаты (индексы)
                    System.out.println(i + " " + j);
                }
            }
        }
    }
}

