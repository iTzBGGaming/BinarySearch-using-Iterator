		import java.util.Iterator;
		import java.util.Scanner;
		import java.util.LinkedList;
		
		public class LinkyListy {
		public static void main(String []args) {
		LinkedList linky = new LinkedList();
		Scanner in = new Scanner(System.in);

		//Add something in LinkedList
		linky.add("Pisang");
		linky.add("Rambutan");
		linky.add("Durian");
		linky.add("Cempaka");
		linky.add(0,"Nasi"); //add an element to linked list at index that you desired
		
		//if you dont know which element in index in linked list you're looking for. aka BINARY SEARCH
		Iterator it = linky.iterator();
			System.out.println("********** INDEX SEARCHER **********");
			System.out.println("Search for a food? (Pisang,Rambutan,Durian,Cempaka,Nasi)");
			String choice = in.nextLine();

			while(it.hasNext()) {
				if(((String)it.next()).equalsIgnoreCase(choice)) {
					System.out.println("it's in index "+linky.indexOf(it.next()));
				}
			}	
}
}
