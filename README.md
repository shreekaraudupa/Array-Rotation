# Array-Rotation
Array rotation using deque
package rotation;

import java.util.*;

public class rotation {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Deque q=new LinkedList();
		Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int k = sc.nextInt();
        int a[] = new int[n];
        int e;
        for(int i=0; i < n; i++)
        {
        	e=sc.nextInt();
        	q.add(e);
        }
        int first;
        for(int i=0; i < k; i++)
        {    
        	first=(Integer) q.remove();
        	q.addLast(first);
        }
      
        for(int i=0;i<n;i++)
        {
        	System.out.print(q.remove()+" ");
            
        }
	}

}
/*
n is number of elements
k in number of rotation 

final print the result after  left rotation 
*/
