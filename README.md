# ReadingMaterial93
public class ReadingMaterial {
	private int pages;
   	private String names;
    	public ReadingMaterial(int p, String n){
               pages = p;
               names = n;
	}
	public int getPages(){
		return pages;
	    }
	    public String getName(){
		return names;
	    }

	    public String toString(){
		return names + ", "+ pages+" pages";
	    }
}

# Main
public class Main {

	public static void main(String[] args) {
	Novel nov1 = new Novel(328, "1984", "Sci-fi", 1949);
        Comic com1 = new Comic(40,"Captain Underpants", "Color", 2020);
        Magazine mag1=new Magazine(20,"Sports Illustrated", "Sports", 1993);
        
        System.out.println(mag1);
        mag1.getCategory();
        mag1.getYear();
        
        System.out.println(nov1);
        nov1.getGenre();
        nov1.getYear();
        
        System.out.println(com1);
        com1.getColor();
        com1.getYear();
    }
    
}

# Comic
public class Comic extends ReadingMaterial{
	public String col;
	public int year;
	public Comic (int page, String name, String color, int releaseYear) {
		 super(page, name);
		 col=color;
		 year = releaseYear;
		 
	 }
	 public String getColor() {
		 return col;
	 }
	 public int getYear() {
		 return year;
	 }
}

# Magazine
public class Magazine extends ReadingMaterial{
	public String cat;
	public int year;
	public Magazine (int page, String name, String category, int releaseYear) {
		 super(page, name);
		 cat=category;
		 year = releaseYear;
		 
	 }
	 public String getCategory() {
		 return cat;
	 }
	 public int getYear() {
		 return year;
	 }
}

# Novel
public class Novel extends ReadingMaterial{
	public String gen;
	public int year;
	public Novel (int page, String name, String genre, int releaseYear) {
		 super(page, name);
		 Gen=genre;
		 year = releaseYear;
		 
	 }
	 public String getGenre() {
		 return gen;
	 }
	 public int getYear() {
		 return year;
	 }
}
