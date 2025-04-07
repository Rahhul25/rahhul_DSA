## DSA CONCEPTS(I LEARN)

 These are the concepts ,that I keeps
 on updating here as I learn.

#### ARRAY LIST
> To Remove Even Numbers in the Arraylist
```sh
class Removeeven{

	public static void main(String[] args) {
	 ArrayList<Integer>list1=new ArrayList<>();
	 list1.add(5);
	 list1.add(4);
	 list1.add(8);
	 list1.add(13);
	 list1.add(7);
	 list1.add(9);
	 list1.add(101);
	 list1.add(34);
	 list1.add(41);
	 list1.add(15);
	 for(int i=list1.size()-1;i>=0;i--) {
		if(list1.get(i)%2==0) {
			list1.remove(i);
		}
	 }
	 System.out.println(list1);
	 }
}
```
#### STRINGS
> To reverse vowels of a String code
```sh
class reversestr{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        String str="WelcometoCoding";
        char ch[]=str.toCharArray();
        int i=0;
        int j=str.length()-1;
        while(i<j){
            while(ch[i] !='a' && ch[i] !='e' && ch[i] !='i' && ch[i] !='o' && ch[i] !='u'){
                i++;
            }
            while(ch[j] !='a' && ch[j] !='e' && ch[j] !='i' && ch[j] !='o' && ch[j] !='u'){
                j--;
            }
            if(i>=j){
                break;
            }
            char s=ch[i];
            ch[i]=ch[j];
            ch[j]=s;
            i++;
            j--;
        }
        for(char s : ch){
            System.out.print(s);
        }
    }
}
```
> To convert letters to lowercase of a String
```sh
class tolowcase{
    public static void main(String args[]){
        String str="WElcOmeTOScaLEr";
        char ch[]=str.toCharArray();
        for(int i=0;i<str.length();i++){
            char s=ch[i];
            if(s>='A' && s<='Z'){
                char r=(char)(s-'A'+'a');
                ch[i]=r;
            }
        }
        for(char r:ch){
            System.out.print(r);
        }
    }
}
```
#### SORTING
   > Selection Sort
```sh
import java.util.*;

class selecsort {

	public static void main(String[] args) {
	 int arr[]= {2,8,4,-1,7,10,5,6};
	 int minval=0;
	 int minindex=0;
	 for(int i=0;i<arr.length-1;i++) {
		 minval=arr[i];
		 minindex=i;
		 for(int j=i+1;j<arr.length;j++) {
			 if(arr[j]< minval) {
				 minval=arr[j];
				 minindex=j;
			 }
		 }
		 int temp=arr[minindex];
		 arr[minindex]=arr[i];
		 arr[i]=temp;
	 }
	 for(int val: arr) {
		 System.out.print(val +" ");
	 }
    }
}
```
   > Bubble Sort
```sh
 class bubblesort{

	public static void main(String[] args) {
	int arr[]= {4,6,8,3,9,-1,5,2};
	int n=arr.length;
	for(int i=0;i<n-1;i++) {
	for(int j=0;j<n-1-i;j++) {
		if(arr[j]>arr[j+1]) {
			int temp=arr[j+1];
			arr[j+1]=arr[j];
			arr[j]=temp;
		}
	}
	}
	for(int val: arr) {
		System.out.print(val+" ");
	}
	}
}
```
> Insetion Sort
```sh
class insertionsort {

	public static void main(String[] args) {
	int arr[]= {4,6,8,3,9,-1,5,2};
	for(int i=1;i<arr.length;i++) {
		int temp=arr[i];
		int j=i-1;
		while(j>=0 && arr[j]>temp) {
			arr[j+1]=arr[j];
			arr[j]=temp;
			j--;
		}
		
	}
	for(int val: arr) {
		System.out.print(val+" ");
	}
	}
}
```
