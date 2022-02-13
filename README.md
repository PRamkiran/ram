root
import java.util.Scanner;
import java.lang.Math;
class Roots
{
public static void main(String args[])
{
double root1,root2;
Scanner obj=new Scanner(System.in);
System.out.println("enter values of a,b,c");
int a=obj.next Int();
int b=obj.next Int();
int c=obj.next Int();
double determinent=b*b-4*a*c;
if(determinent>0)
{
root1=(-b+Math.sqrt(determinent))/2*a;
root2=(-b-Math.sqrt(determinent))/2*a;
System.out.println("quadratic eq has real roots"+"\n"+"its roots are:"+"\n"+"root1="+root1+"\n"+"root2="+root2);
}
else if(determinent==0)
{
root1=root2=-b/2*a;
System.out.println("quadratic equation has equal roots"+"\n"+"root1="+root1+"\n"+"root2="+root2);
}
else
{
double real=-b/2*a;
double imaginary=Math.sqrt(-determinant)2*a;
System.out.println("real="+real+"imaginary="+imaginary);
}
}
}
race
import java.io.*;
class Race
{
public static void main(String [] args)
{
int R[]=new int[20];
float avg;
int sum=0;
System.out.println("enter speed of 5 members");
Scanner sc=new Scanner(System.in);
for(int j=1;j<=5;j++)
{
R[j]=sc.next Int();
sum+=R[j];
}
avg=sum/5;
for(int i=1;i<=5;i++)
{
if(avg<R[i])
{
System.out.println("Qualified racer is:"+i+"with value="+R[i]);
}
}
}
}
implement class mechanism
class Student
{
   String name="Raju";
   String _class="B.Tech 1st year";
   int rollno=178;
   public void display()
   {
     System.out.println("Name of the student is:"+name);
     System.out.println("Present qualification of the student is:"+_class);
     System.out.println("Roll number of the student is:"+rollno);
   }

}
class Details
{
  public static void main(String args[])
  {
     Student s1=new Student();
     s1.display();
  }
}
implementing constructor
class Main {
  private String name;

  // constructor
  Main() {
    System.out.println("Constructor Called:");
    name = "Programiz";
  }

  public static void main(String[] args) {

    // constructor is invoked while
    // creating an object of the Main class
    Main obj = new Main();
    System.out.println("The name is " + obj.name);
  }
}
constructor overloading
class Student5{
    int id;
    String name;
    int age;
    Student5(int i,String n){
    id = i;
    name = n;
    }
    Student5(int i,String n,int a){
    id = i;
    name = n;
    age=a;
    }
    void display(){System.out.println(id+" "+name+" "+age);}
 
    public static void main(String args[]){
    Student5 s1 = new Student5(111,"Karan");
    Student5 s2 = new Student5(222,"Aryan",25);
    s1.display();
    s2.display();
   }
}
method overloading
class DisplayOverloading
{
    public void disp(char c)
    {
         System.out.println(c);
    }
    public void disp(char c, int num)  
    {
         System.out.println(c + " "+num);
    }
}
class Sample
{
   public static void main(String args[])
   {
       DisplayOverloading obj = new DisplayOverloading();
       obj.disp('a');
       obj.disp('a',10);
   }
}
single inheritance
class A
{
public void method A()
{
system.out.println("base class");
}
}
class B extends A
{
public void method B()
{
System.out.println("child class");
}
public static void main(String args[])
{
b obj=new B();
obj.method A();
obj.method B();
}
}
calculator
class Calculator
{
public static void main(String args[])
{
System.out.println("enter values:");
Scanner s = new Scanner(System.in);
int a=s.next Int();
int b=s.next Int();
Product pr =new Product();
pr.Addition(a,b):
pr.subtaction();
pr.mul();
}
}
class Add
{
Protected int p,q;
Public void addition(int x,int y)
{
p=x;
q=y;
int r=p+q;
System.out.println("inside of theclass Add");
System.out.println("sum is:"+r);
}
}
class sub extends add
{
int diff;
public void subtraction()
[
int diff =p-q;
System.out.println("inside of the class sub");
System.out.println("diff is:"+diff);
}
}
class product extends sub
{
int prod;
public void mul()
{
int prod=p*q;
System.out.println("inside of theclass product");
System.out.println("product is:"+prod);
}
}
abstract class area
import java.util.Scanner;
abstract class Area
{
public void display()
{
system.out.println("inside abstract");
}
Abstract void area();
}
class Rectangle extends Areas
{
int base=10;
int height=20;
public void area()
{
int area=base*height;
System.out.println("area is"+area);
}
}
class Square extends Areas
{
int base=15;
public void area()
{
int area1=base*base;
System.out.println("area is"+area);
}
}
class Triangle extends Areas
{
int base=5;
int height=15;
public void area()
{
int area2=(base*height)/2;
System.out.println("area is"+area);
}
}
class Geometry
{
public static void main(String args[])
{
Rectange r = new Rectangle();
Square s =new Square();
Triangle t=new Triangle();
r.display();
r.area();
s.area();
t.area();
}
}
super key
class One
{
protected int a;
One(int I)
{
this.a=i;
}
void display()
{
System.out.println("super class method:a="+a);
}
}
class Two extends One
{
protected int a;
Two(int i,int j)
{
super(I);
a=j;
}
void diplay()
{
super.diplay()
System.out.println("sub class method:a="+a);
}
}
class Super
{
public static void main(String args[])
{
Two t=new Two(9,6);
t.diplay();
}
}
interface
import java.util.Scanner;
interface Base1
{
final double pie=3.41;
void area();
}
interface Base2
{
final double pie=3.41;
void area();
}
class Derived implements Base1,Base2
{
double area;
public void area()
{
area=pie*r*r;
System.out.println("area of circle if:"+arae);
}
}
class Inheritance
{
public static void main(String args[])
{
Derived d=new Derived();
d.arae();
}
}
multiple catch block
public class multiple catch block
{
public static void main (String [] args)
{
try{
int a[]=new int[5]
a[3]=30/0;
system.out.println(a[10]);
}
catch(Arithemetic exception e)
{
system.out.println("Arithemetic exception occured");
}
catch(Array index out of bounds exception e)
{
system.out.println("Array index out of bounds exception occurs");
}
catch(exception e){
system.out.println("parent exception occurs");
}
system.out.println("rest of the code");
}
}

exception handling
import java.util.scanner;
class exception_handle
{
public static void main(string args[])
{
exception ex=new exception();
}
}
class exception 
{
exception()
{
Scanner S=new Scanner(System.in);
System.out.print("enter a&b);
int a=s.nxtInt();
int b=s.nxtInt();
try
{
int c=a/b;
System.out.print(c);
}
catch(arithemetic exception ae)
{
system.out.println("arthemetic exception occured");
}
}
}
multiple catch block
class Dilip
{
public static void main(String args[])
{
try
{
int array[]=new int[10];
array[10]=30/0;
}
catch(arithmatic Exception e)
{
System.out.println(e.getMessage());
}
catch(Array Index out of Bounds Exception e)
{
System.out.println(e.getMessage());
}
}
}
rut time polymorphism
class Bank
{
float get RateOfIntrest()
{
return 0;
}
}
class ICICI extends Bank
{
float get RateOfIntrest()
{
return 7.3f;
}
}
class SBI extends Bank
{
float get RateOfIntrest()
{
return 8.4f;
}
}
class AXIS extends Bank
{
float get RateOfIntrest()
{
return 9.7f;
}
}
class TestPolymorphism
{
public static void main(String args[])
{
Bank b;
b =new SBI();
System.out.println("SBI rate of intrest:"+b.getrateofintrest());
b=new  ICICI();
System.out.println("ICICI rate of intrest:"+b getrateofintrest());
 b=new  AXIS();
System.out.println("AXIS rate of intrest:"+b getrateofintrest());
 }
}
throw
import java.io.*;
public class Oops
{
static void check Age(int age)
{
if(age<18)
{
throw new Arithmetic Exception("access denied you must be atleast 18 years");
}
else
{
System.out.println("access granted you are old enough");
}
}
public static void main(string []args)
{
check Age(17);
}
}
null pointer exception
class Nullpointerexception
{
public static void main(String[] args)
{
try
{
string a=null;
System.out.println(a.char At(0));
}
catch(Null pointer Exception e)
{
System.out.println("null poinetr exception occured");
}
}
}
arithmetic exception
class ArithmeticEexception
{
public static void main(String args[])
{
try
{
int a=30,b=0;
int c=a/b;
System.out.println("result is"+c);
}
catch(Arithmetic Exception e)
{
System.out.println("error");
}
}
}




