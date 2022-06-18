# matrixTranspose
import java.lang.reflect.Array;
import java.util.Arrays;

public class Main {

    public static void main(String[] args) {

        int[][] a = {
                {2, 3, 4, 5},
                {5, 6, 4, 8}
        };
        int[][] t = new int[a[0].length][a.length];
        for (int i = 0; i < t.length; i++) {
            for (int j = 0; j < t[0].length; j++) {
                t[i][j] = a[j][i];
            }
        }
        for (int i = 0; i < t.length; i++) {
            for (int j = 0; j < t[i].length; j++) {
                System.out.print(t[i][j] + " ");
            }
            System.out.println(" ");
        }
    }
}
