class A
{
int x,y;
void Addinfo(int a,int b)
{
x=a;
y=b;
}
void display()
{
System.out.println("Addition in  super class :");
System.out.println("addition of "+x+" and"+y+"="+(x+y));

}
}
class B extends A
{
void Set(int b,int c)
{
x=b;
y=c;
System.out.println("from intermediate superclass:");

System.out.println("Substraction of "+x+"and" +y+"="+(x-y));
}
}
class C extends B
{
void Display(int a,int b)
{
x=a;y=b;
System.out.println("from subclass:");
System.out.println("multiplication of "+x+"and"+y+"="+(x*y));
}
public  static void main(String arg[])
{
C c=new C();
c.Addinfo(10,8);
c.display();
c.Set(7,8);
c.Display(2,4);
}
}
