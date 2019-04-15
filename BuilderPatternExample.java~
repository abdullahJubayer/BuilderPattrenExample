public class BuilderPatternExample{
	private int door;
	private int window;
	private int table;
	private int chair; 
	
	public BuilderPatternExample(Builder builder){
		door=builder.door;
		window=builder.window;
		table=builder.table;
		chair=builder.chair;
	}
	public int getDoor(){
		return door;	
	}
	public int getWindow(){
		return window;	
	}
	public int getChair(){
		return chair;	
	}
	public int getTable(){
		return table;	
	}
	
	public static class Builder{
		private int door;
		private int window;
		private int chair;
		private int table; 
		
		public Builder setDoor(int door){
			this.door=door;
			return this;		
		}
		
		public Builder setWindow(int window){
			this.window=window;
			return this;		
		}
		public Builder setChair(int chair){
			this.chair=chair;	
			return this;	
		}
		public Builder setTable(int table){
			this.table=table;
			return this;		
		}
		public BuilderPatternExample build(){
			return new BuilderPatternExample(this);		
		}
	}
	public static void main(String ar[]){
			BuilderPatternExample obj=new BuilderPatternExample.Builder()
							.setDoor(2)
							.setWindow(3)
							.setTable(1)
							.setChair(6)
							.build()
							;
							
			System.out.println(" Door:"+obj.getDoor()+"\n Window:"+obj.getWindow()+"\n Table:"+obj.getTable()+"\n Chair"+obj.getChair());				
	}
	
}