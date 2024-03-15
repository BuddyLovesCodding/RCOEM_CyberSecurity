
public class lec2 {
public static void main(String[] args) {
	
//	print(1,5);
//	int ans = fibo(10);
//	System.out.println(ans);
//	coinPrint(3,"");
	partyKarteHai(0,"ab","");
}
public static void print(int s , int e) {
	
	if(s>e) {
		return;
	}
	
	
	System.out.println(s);
	print(s+1 , e);
	System.out.println(s);
	
	
	
}
public static int fibo(int n) {
	if(n<=1) {
		return n;
	}
	
int	sp1 = fibo(n-1);
	int sp2 = fibo(n-2);
	
	return sp1 + sp2;
}

public static void coinPrint(int coin , String str) {
	
	if(coin == 0) {
		System.out.println(str);
		return;
	}
	
	coinPrint(coin-1 , str + "H");
	coinPrint(coin-1 , str+ "T");
}

public static void partyKarteHai(int idx ,String given, String str) {
	
	if(idx==given.length()) {
		System.out.println("=>" + str);
		return;
	}
	
	partyKarteHai(idx+1 , given , str + given.charAt(idx));
	partyKarteHai(idx+1 , given , str);
	partyKarteHai(idx+1 , given , str + (int)given.charAt(idx));
}
}
