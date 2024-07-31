# Max-ones-in-which-row-of-Array
import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int [][]a=new int[n][n];
        System.out.println("Enter array values :");
        for(int i=0;i<n;i++){
            for(int j=0;j<n;j++){
                int p=sc.nextInt();
                a[i][j]=p;
            }
        }
        int c=0;
        int m=0;
        int k=0;
        for(int i=0;i<n;i++){
            for(int j=0;j<n;j++){
                if(a[i][j]==1){
                    c++;
                }
            }
            if(c>m){
                m=c;
                k=i;
            }
        }
        
        System.out.println("Max ones are in "+(k+1)+" Row");
    }
}
