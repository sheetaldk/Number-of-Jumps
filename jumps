import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;
public class CandidateCode {
public static int GetJumpCount(int INPUT1,int INPUT2,int[] input3)
    {
	    int tn=0,n;
        for(int i=0; i<input3.length; i++) {
            if(input3[i]<=INPUT1) {
                tn+=1;
                continue;
            }

            n=((input3[i]-INPUT1)/(INPUT1-INPUT2));
            n+=input3[i]-((INPUT1-INPUT2)*n)==INPUT1?1:2;
            tn+=n;
        }
      return tn;
    }

public static void main(String[] args) throws IOException{
        Scanner in = new Scanner(System.in);
        int output = 0;
        int ip1 = Integer.parseInt(in.nextLine().trim());
        int ip2 = Integer.parseInt(in.nextLine().trim());
        int ip3_size = 0;
        ip3_size = Integer.parseInt(in.nextLine().trim());
        int[] ip3 = new int[ip3_size];
        int ip3_item;
        for(int ip3_i = 0; ip3_i < ip3_size; ip3_i++) {
            ip3_item = Integer.parseInt(in.nextLine().trim());
            ip3[ip3_i] = ip3_item;
        }
        output = GetJumpCount(ip1,ip2,ip3);
        System.out.println(String.valueOf(output));
    }
}
