class Add
{
	int a=5,b=7;
	Add()
	{
		System.out.println(a+b);
	}
	public Add(int c)
	{
		System.out.println(a+b+c);
	}
	protected Add(int c,int d)
	{
		System.out.println(a+b+c+d);
	}
	private Add(int c,int d,int e)
	{
		System.out.println(a+b+c+d+e);
	}
}
class Jala {
	
	public static void main(String[] args) {
		Add a = new Add();
		Add b = new Add(5);
		Add c = new Add(4,5);
		Add d = new Add(4,5,6); // Error for private defined constructor
		
	}
}

