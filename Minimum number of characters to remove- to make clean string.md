#Minimum number of characters needed to remove to make the string clean



``` java
import java.util.*;
public class main{
    public static void main(String args[])
    {
        Scanner sc=new Scanner(System.in);
        String x=sc.nextLine();
        TreeSet<Character> ts=new TreeSet<>();
        int count=0;
        for(char c:x.toCharArray())
        {
            if(!ts.add(c))
            {
                count++;
            }
        }
        System.out.println(count);
    }
}


