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
