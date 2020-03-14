# binarySearch-
Binary Search in Java
package Serching;

import java.util.Scanner;

public class BinarySearch {

	public static void main(String[] args) {
		/*System.out.println("hello");*/
		
		/*int[]a = {2,4,9,14,17,19,23,27,32};
		
		int srch =40;*/ 
		int counter, num, item, array[], li,hi,mi;
		Scanner sc= new Scanner(System.in);
		System.out.println("Enter The Array size");
		num = sc.nextInt();
		array =new int[num];
		System.out.println("Enter " + num + " integers");
	      for (counter = 0; counter < num; counter++)
	          array[counter] = sc.nextInt();

	      System.out.println("Enter the search value:");
	      item = sc.nextInt();
		 li=0;
		 hi= num-1;  
		 mi=(li+hi)/2;
		while(li<=hi){
		if(array[mi]==item){
			System.out.println("element is at "+mi+ "index position");
			break;
		}

		else if(array[mi]<item){
			li= mi+1;
		}
		else
		{
			hi =mi-1;
		}
		mi=(li+hi)/2;
	}
	if(li>hi){
		System.out.println("element not found");
		
	}
	}
	}
