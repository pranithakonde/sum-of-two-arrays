# sum-of-two-arrays
import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        /* Enter your code here. Read input from STDIN. Print output to STDOUT. Your class should be named Solution. */
        Scanner s = new Scanner(System.in);
        int N = s.nextInt();
        int M = s.nextInt();
        int[][] a = new int[N][M];
        int[][] b = new int[N][M];
        int[][] c = new int[N][M];
        
        for(int i=0;i<N;i++)
        {
            for(int j=0;j<M;j++)
            {
                a[i][j]=s.nextInt();
            }
        }
        for(int i=0;i<N;i++)
        {
            for(int j=0;j<M;j++)
            {
                b[i][j]=s.nextInt();
            }
        }
        for(int i=0;i<N;i++)
        {
            for(int j=0;j<M;j++)
            {
                c[i][j]=a[i][j]+b[i][j];
               
            }
        }
        for(int i=0;i<N;i++)
        {
            for(int j=0;j<M;j++)
            {
              System.out.print(c[i][j]+" ");
               
            }
            System.out.println();
        }
    }
}
