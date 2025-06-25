package lecture;

import java.util.Scanner;

public class Two {

	public static int linear_search(int[] a, int x) {
		int i = 0, last = a.length -1;
		while (i <= last && a[i] != x) {
			i++;
		}
		if (i > last) {
			return -1;
		} else {
			return i;
		}
	}
	

	public static void main(String[] args) {
		// TODO Auto-generated method stub
        int[] a = new int[] {67, 33, 21, 84, 49, 50, 75};
        System.out.println("" + linear_search(a, 84));
        System.out.println("" + linear_search(a, 70));
        
        int[] b = new int[] {21, 33, 49, 58, 67, 75, 84};
        System.out.println("" + linear_search(a, 84));
        System.out.println("" + linear_search(a, 70));
	}
}
