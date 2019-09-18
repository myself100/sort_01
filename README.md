# sort_01
package elclipse;
import java.util.*;
public class LinkedList {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int a[]= {1,0,1,0,0,0,1,1,0,0,0,1,0};

		int n=a.length;
		sort(a,n); // calling sort function
		System.out.print(Arrays.toString(a));//convert array to string
	
}
	public static void sort(int a[],int n) {
		int pivot=1;
		int j=0;
		for(int i=0;i<n;i++) {
			if(a[i]<pivot) {
				swap(a,i,j);// calling swap function
				j++;
			}
		}
}
	public static void swap(int a[],int i,int j) {
		int temp;
		temp=a[i];
		a[i]=a[j];
		a[j]=temp;
	}
}
