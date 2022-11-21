		Iterator it = linky.iterator();
			System.out.println("********** INDEX SEARCHER **********");
			System.out.println("Search for a food? (Pisang,Rambutan,Durian,Cempaka,Nasi)");
			String choice = in.nextLine();

			while(it.hasNext()) {
				if(((String)it.next()).equalsIgnoreCase(choice)) {
					System.out.println("it's in index "+linky.indexOf(it.next()));
				}
			}	
