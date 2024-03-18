package SRCEM_pack2;

import java.util.Stack;

public class lec5 {
public static void main(String[] args) {
	Stack<Integer>st = new Stack<>();
	
	st.add(1);
	st.add(2);
	st.add(3);
	st.add(4);
	st.add(5);
//	Stack<Integer> temp = new Stack<>();
//	while(!st.isEmpty()) {
//		System.out.println(st.peek());
//		temp.add(st.pop());
//	}
//	while(!temp.isEmpty()) {
//		st.add(temp.pop());
//	}
	
	printSt(st);
	System.out.println(st);
}
public static void printSt(Stack<Integer> st) {
	
	if(st.isEmpty()) {
		return;
	}
	
	int top = st.pop();
	System.out.println(top);

	printSt(st);
	System.out.println(top);
	st.add(top);
}
}
