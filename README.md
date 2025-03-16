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
