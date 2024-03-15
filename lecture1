package SRCEM_pack2;

import java.util.ArrayList;

public class lec2 {
public static void main(String[] args) {
//	int arr1[] = {1,2,2,2,3,4,4,5,6};
//	int arr2[] = {1,1,2,2,2,3,3,4,5};
//	
//	funcInter(arr1,arr2);
	
//	int arr1[] = {2 ,3 ,7 ,10, 12, 15, 30, 34};
//	int arr2[] = {1 ,5 ,7 ,8 ,10, 15, 16 ,19};
//	maxSumPath(arr1,arr2);
	
//	boolean ans = isPalin("abbbbbba");
//	System.out.println(ans);
	countPalin("aaa");
	}
public static void funcInter(int arr1[] , int arr2[]) {
	int i = 0;
	int j =0;
	ArrayList<Integer> al = new ArrayList<>();
	while(true) {
		
		if(i>=arr1.length || j>=arr2.length) {
			break;
		}
		
		if(arr1[i] == arr2[j]) {
			i++;
			j++;
			System.out.println(arr1[i]);
//			i++;
//			j++;
		}
		else if(arr1[i]>arr2[j]) {
			j++;
		}
		else {
			i++;
		}
	}
	
}

public static void maxSumPath(int arr1[] , int arr2[]) {
	int i = 0;
	int j =0;
	int sum1 = 0;
	int sum2 = 0;
	int TS = 0;
	
	while(i<arr1.length && j<arr2.length) {
		
		
		
		if(arr1[i] == arr2[j]) {
			TS+= (int)Math.max(sum1, sum2) + arr1[i];
			sum1=0;
			sum2 =0;
			i++;
			j++;
		}
		else if(arr1[i]>arr2[j]) {
			sum2 = sum2 + arr2[j];
			j++;
		}
		else {
			sum1 = sum1 + arr1[i];
			i++;
		}
	}
	System.out.println(TS);
	System.out.println("sum1 =>" + sum1);
	System.out.println("sum2 =>" + sum2);
	
	while(i<arr1.length) {
		sum1 = sum1 + arr1[i];
		i++;
	}
	
	while(j<arr2.length) {
		sum2 = sum2 + arr2[j];
		j++;
	}
	TS+= (int)Math.max(sum1, sum2);
//	System.out.println(TS);
//	System.out.println("sum1 =>" + sum1);
//	System.out.println("sum2 =>" + sum2);
}

public static boolean isPalin(String str) {
	int i = 0;
	int j = str.length()-1;
	while(i<j) {
		if(str.charAt(i)!=str.charAt(j)) {
			return false;
		}
		i++;
		j--;
	}
	return true;
	
}

public static void countPalin(String str) {
	int ans = 0;
	for(int i = 0; i<str.length() ; i++) {
		ans = ans + grow(str , i , i , 0);
		ans = ans + grow(str , i , i+1 , 0);
	}
	System.out.println(ans);
	
}

public static int grow(String str , int left , int right , int count) {
	while(left>=0 && right<str.length()) {
		
		if(str.charAt(left)==str.charAt(right)) {
			count++;
			left--;
			right++;
		}
		else {
			break;
		}
		
	}
	return count;
}
}
