package SRCEM_pack2;

import java.util.ArrayList;

public class lec4 {
public static void main(String[] args) {
//	ArrayList<String> al = new ArrayList<>();
//	paranthesis(3,3,"" , al);
//	System.out.println(al);
//	jumpKaro(5,"") ;
	chaloChalen(0, 0, 2, 2, "" );
}

public static void paranthesis(int op , int cl ,String str , ArrayList<String> al) {
	
	
	if(cl<op) {
		return;
	}
	
	if(cl==op && op==0) {
//		System.out.println(str);
		al.add(str);
		return;
	}
	if(op<0) {
		return;
	}
	
	paranthesis(op-1 , cl , str+"(" , al);
	paranthesis(op , cl-1 , str + ")" , al);
	
	
}

public static void jumpKaro(int n , String str) {
	
	if(n==0) {
		System.out.println(str);
		return;
	}
	if(n<0) {
		return;
	}
	
	
	jumpKaro(n-1 , str + 1);
	jumpKaro(n-2 , str + 2);
	jumpKaro(n-3 , str+3);
}

public static void chaloChalen(int crow , int ccol , int drow , int dcol , String path ) {
	
		if(crow == drow && ccol == dcol) {
			System.out.println(path);
			return;
		}
		
		if(ccol > dcol || crow >drow) {
			return;
		}
	 chaloChalen(crow , ccol+1 , drow , dcol , path + "R");
	 chaloChalen(crow+1 , ccol , drow , dcol , path+"D");
}

// palindrom partitioning leetcode
public List<List<String>> partition(String s) {
        List<List<String>> ALL = new ArrayList<>();
        List<String> al = new ArrayList<>();

        solve(s , ALL , al);
        return ALL;
    
    }
        public static void solve(String str ,List<List<String>> ALL , List<String> al){

            if(str.length()==0){
                // System.out.println(al);
                ArrayList<String> temp = new ArrayList<>(al);
                ALL.add(temp);
                return;
            }





            for(int i =0 ;i <str.length() ; i++){
                String piece = str.substring(0 , i+1);
                if(isPalin(piece)){
                    al.add(piece);
                    String remain = str.substring(i+1);
                    solve(remain , ALL , al);
                    al.remove(al.size()-1);
                }
            }

        }

        public static boolean isPalin(String str){
            int i = 0;
            int j = str.length()-1;
            while(i<j){
                if(str.charAt(i)!=str.charAt(j)){
                    return false;
                }
                i++;
                j--;
            }
            return true;
        }
}
