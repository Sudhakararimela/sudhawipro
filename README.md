# sudhawipro
java -core
jdk1.8.txt

html,css,javascript,Bootstrap,Jquery,Angular10
Oracle,mysql,mongodb,JDBC,Hibernate
spring,springboot,Micro-services
AWS,project
duration -18weeks
------------------------------------------------------------
https://github.com/sandipmohapatra/Batch69
-------------------------------------------------------------
Java 1.8 features
---------------------------
1)Java is a Object Oriented Programming language.
2)Java is simpler than c and c++ as we don't have pointer concept,Multiple Inheritance,operator overloading.
3)Java supports multi-threading or multi-tasking.
4)We can develop web-application,network application,standalone application and also mobile application.
5)In java we have interface which support the concept of multiple inheritance.
6)In java we have constructor but no destructor.There is automatic garbage clearance.
7)Java is a secured language.We have 4 access specifier private,public,protected and default.
------------------------------------------------------------------------------ 
DataTypes
----------------------
primative datatype
---------------------------
1)byte - 1 byte
2)short - 2 bytes
3)int - 4 bytes
4)long - 8 bytes
5)char - 2 bytes
6)boolean - 1 bit
7)float - 4 bytes
8)double - 8 bytes
--------------------------------------------------
derived datatype
----------------------------
1)String
2)array
3)class
----------------------------------------------------
Operators
------------- 
1)unary :- i++,++i,--i,i--
2)binary :- 
i)arithmatic operator:- +,-,/,*,%(modules/remainder)
ii)comparative operator :- <,>,<=,>= ,== 
iii)assignment operator :- = ,!=
iv)bitwise :- >>,<<
3)ternary :- ?,:
-------------------------------------------------------------------------------------------
we have 4 access specifier 
1)private:-If we declare variable and methods as private we can access it within the class only.
2)public:-If we declare variable and methods as public we can access it within the class ,outside the class and outside the package.
3)protected:-If we declare variable and methods as protected we can access it within the class and also within the child class.
4)default:-If we declare variable and methods as default we can access it within the class ,outside the class but not outside the package.
----------------------------------------------------------------------------------------------
example-1
-----------------
package org.sandip;

public class FirstExample
{
public static void main(String[] args) 
{
	System.out.println("welcome to java at wipro");
}
}
-----------------------------------------------------------------------
example-2
----------------------
package org.sandip;

public class SecondExample
{
public static void main(String[] args) 
{
int a=10,b=20,c=a+b;
	System.out.println("The sum of "+a+ " and "+b+" is "+c);
}
}
--------------------------------------------------------------------------------
example-3
----------------
package org.sandip;

public class ThirdExample 
{
public static void main(String[] args) {
	byte a=10;
	short b=20;
	int c=30;
	long d=40;
	float e=34.56f;
	double f=45.34;
	String g="apple";
	char h='a';
	System.out.println(a+" "+b+"  "+c);
	System.out.println(d+" "+e+"  "+f);
	System.out.println(g+" "+h);
	}
}
---------------------------------------------------------------------------------
example-4
-------------------
package org.sandip;
import java.util.*;
public class FourthExample 
{
	public static void main(String[] args)
	{
	Scanner ob=new Scanner(System.in);
	System.out.println("enter your slno,name,address");
	int slno=ob.nextInt();
	String name=ob.next();
	String address=ob.next();
	System.out.println("The slno is "+slno);
	System.out.println("The name is "+name);
	System.out.println("The address is "+address);
		}
}
----------------------------------------------------------------------
example-5
----------------
package org.sandip;
import java.util.*;
public class FourthExample 
{
	public static void main(String[] args)
	{
	Scanner ob=new Scanner(System.in);
System.out.println("enter 2 nos");
int a=ob.nextInt();
int b=ob.nextInt();
int c=a+b;
System.out.println("the sum is "+c);
}
}
---------------------------------------------------
wap to enter 5 nos and find sum and average 
----------------------------------------------------
example-6
------------------------
package org.sandip;
import java.util.*;
public class FourthExample 
{
	public static void main(String[] args)
	{
	Scanner ob=new Scanner(System.in);
System.out.println("enter 5 nos");
int a=ob.nextInt();
int b=ob.nextInt();
int c=ob.nextInt();
int d=ob.nextInt();
int e=ob.nextInt();
int sum=a+b+c+d+e;
int avg=sum/5;
System.out.println("the sum is 5 nos "+sum);
System.out.println("the average of 5 nos "+avg);
}
}
---------------------------------------------------------------------
example-7
---------------------
package org.sandip;
import java.util.*;
public class FourthExample 
{
	public static void main(String[] args)
	{
	Scanner ob=new Scanner(System.in);
System.out.println("enter 5 nos");
float a=ob.nextFloat();
float b=ob.nextFloat();
float c=ob.nextFloat();
float d=ob.nextFloat();
float e=ob.nextFloat();
float sum=a+b+c+d+e;
float avg=(int)sum/5;//type casting
System.out.println("the sum is 5 nos "+sum);
System.out.println("the average of 5 nos "+avg);
}
}
-----------------------------------------------------------------------------------
Single dimentional array
double dimentional array
class and Object
constructor
Inheritance
poly-merphisim
Abstraction
Encapsulation
-------------------------------------------------------
 Example-8
-----------------
package org.sandip;
import java.util.*;
public class SingleDimention 
{
public static void main(String[] args) 
{
int a[]=new int[5];
System.out.println("Enter 5 nos");
Scanner ob=new Scanner(System.in);
for(int i=0;i<5;i++)                                    //array index start from 0
	a[i]=ob.nextInt();

System.out.println("5 nos are");
for(int i=0;i<5;i++)
System.out.println(a[i]);
}
}
-----------------------------------------------------
Example-9
------------------
package org.sandip;
import java.util.*;
public class SingleDimention 
{
public static void main(String[] args) 
{
int a[]=new int[5];
int sum=0;
System.out.println("Enter 5 nos");
Scanner ob=new Scanner(System.in);
for(int i=0;i<5;i++)
a[i]=ob.nextInt();

System.out.println("5 nos are");
for(int i=0;i<5;i++)
sum=sum+a[i];
System.out.println("The sum of 5 nos is "+sum);
}
}
---------------------------------------------------------------------------
Example-10
----------------------
double dimentional array
----------------------------------
package org.sandip;
import java.util.*;
public class DoubleDimention 
{
public static void main(String[] args) 
{
int a[][]=new int[3][3];
Scanner ob=new Scanner(System.in);
System.out.println("enter 3*3 matrix");
for(int i=0;i<3;i++)  //outer loop exceute for 1 time
{
	for(int j=0;j<3;j++)     //inner loop execute for 3 times
	{
		a[i][j]=ob.nextInt();   //00,01,02,--10,11,12,--20,21,22
	}
}

System.out.println(" 3*3 matrix is");
for(int i=0;i<3;i++)
{
	for(int j=0;j<3;j++)
	{
		System.out.print(a[i][j]+"  ");
}
System.out.println();
}
}
}

-----------------------------------------------------------------------------------------------
class and Object:-
---------------------------
class :- It is a collection of data members and member functions.
It is a blue print of an Object.
It is also called as an Object factory.
-----------------
Object is an ref pointer to the class.
We can access variables and methods of a class by using an Object.
--------------------------------------------------------
example-11
------------------
package org.sandip;
import java.util.*;
public class Student 
{
int rollno;//instance variable and can be accessed all over the program
String name,address;
void input()
{
	Scanner ob=new Scanner(System.in);
	System.out.println("enter rollno,name,address");
	rollno=ob.nextInt();
	name=ob.next();
	address=ob.next();
}
void display()
{
	System.out.println("the rollno is "+rollno);
	System.out.println("the name is "+name);
	System.out.println("the address is "+address);
	}
public static void main(String[] args)
{
Student ob=new Student();//Student is the class,ob is the object,new to create memory block,student() is a constructor
ob.input();
ob.display();
}
}
--------------------------------------------------------------------------
when we close the program the data are send to grabage clearance.
There is no destructor in java .There is automatic garbage clearance.
-------------------------------------------------------------------------------------------
step 1:- class declaration
step 2:- main
step 3:- creating object
step 4:- accessing variables and methods.
---------------------------------------------------------------------------
wap to enter an employee data
and display it.
empno,name,address,salary.
----------------------------------------------------
Example-12
------------------
package org.sandip;
import java.util.*;
public class Employee 
{
int empno;
String name,address;
float salary;
void input()
{
	Scanner ob=new Scanner(System.in);
	System.out.println("enter empno,name,address,salary");
	empno=ob.nextInt();
	name=ob.next();
	address=ob.next();
	salary=ob.nextFloat();
}
void display()
{
	System.out.println("the empno is "+empno+"The name is "+name);
	System.out.println("the address is "+address+"The salary is "+salary);
	}
public static void main(String[] args) {
	Employee ob=new Employee();
	ob.input();
	ob.display();
}
}
--------------------------------------------------------------
example-13
---------------------
wap to enter student's data
rollno,name,address,phy,chem,bio marks
find the total,avg,and grade of the student.
-----------------------------------------------------------------
package org.sandip;
import java.util.*;
public class StudentData 
{
	int rollno,phy,chem,bio,tot,avg;
	String name,address,grade;
	void input()
	{
		Scanner ob=new Scanner(System.in);
		System.out.println("enter rollno,name and address");
		rollno=ob.nextInt();
		name=ob.next();
		address=ob.next();
		System.out.println("enter phy,chem,bio marks");
		phy=ob.nextInt();
		chem=ob.nextInt();
		bio=ob.nextInt();
		tot=phy+chem+bio;
		avg=tot/3;
			}
	void display()
	{
		System.out.println("The rollno is "+rollno);
		System.out.println("The name is "+name);
		System.out.println("The address is "+address);
		System.out.println("The total is "+tot);
		System.out.println("The average is "+avg);
		if(avg>=70)
			System.out.println("First Division");
		else if(avg>=60)
			System.out.println("Second Division");
		else if(avg>=50)
			System.out.println("Third Division");
		else 
			System.out.println("fail");
				}
public static void main(String[] args) {
	StudentData ob=new StudentData();
	ob.input();
	ob.display();
}
}
------------------------------------------------------------------------------------------
wap to enter your name,age,nationality and find if you are eligible to vote.
use class and object.
----------------------------------------------------------------------------------------------
wap to create a bank class.
enter accno,name,balance.
do some transaction (withdraw or deposite)
and display the final balance.
===================================================================
Example-14
-------------------------------------
package org.sandip;
import java.util.*;
public class BankDemo 
{
int accno;
String name;
float bal;
void input()
{
	Scanner ob=new Scanner(System.in);
	System.out.println("Enter accno,name,balance");
	accno=ob.nextInt();
	name=ob.next();
	bal=ob.nextFloat();
}
void display()
{
	System.out.println("the accno is "+accno);
	System.out.println("the name is "+name);
	System.out.println("the balance is "+bal);
	}
float deposite()
{
	Scanner ob=new Scanner(System.in);
	System.out.println("enter the amount you want to deposite");
	int tot=ob.nextInt();
	bal=bal+tot;
	return bal;
	}
float withdraw()
{
	Scanner ob=new Scanner(System.in);
	System.out.println("enter the amount you want to withdraw");
	int draw=ob.nextInt();
	if(bal>=draw+1000)  
	{
		bal=bal-draw;
		return bal;
	}
	else
	{
		System.out.println("Your Balance is low");
	}
	return bal;
}
public static void main(String[] args) 
{
BankDemo ob=new BankDemo();
Scanner ob1=new Scanner(System.in);
System.out.println("Do you want to do transaction 1.deposite 2.withdraw");
int choice=ob1.nextInt();
switch(choice)
{
case 1:
	ob.input();
	ob.display();
	System.out.println("The total balance is "+ob.deposite());
	break;
case 2:
	ob.input();
	ob.display();
	System.out.println("The total balance is "+ob.withdraw());
	break;
default:System.out.println("wrong input");
	}
}
}
--------------------------------------------------------------------
Constructor
------------------
A constructor is a method which has the same name as that of the class name.
It doenot have any return type nor it return any value.
A constructor execute automatically when an object is created for a class.
There are 2 types of constructor
1)default constructor :- It is without any parameter.
2)parameterized constructor:- It is with parameter.
----------------------------------------------------------------------------------------
Example-15
-------------------
package org.sandip;

public class Constructor
{
Constructor()
{
	System.out.println("This is default constructor");
}
Constructor(int a,int b)
{
	System.out.println("the sum is "+(a+b));
}
public static void main(String[] args) {
	Constructor ob1=new Constructor();
	Constructor ob2=new Constructor(4,5);
	Constructor ob3=new Constructor(6,7);
	Constructor ob4=new Constructor();
		}
}
------------------------------------------------------------------------
example-16
---------------------
package org.sandip;

public class Constructor
{
int rollno;//instance variables can be accessed any where within the program
String name,address,email;
//right click --->source ->Generate constructor using fields 
public Constructor(int rollno, String name, String address, String email) //local variables scope is within the () 
{
	this.rollno = rollno;//this is a self ref pointer ,points to itself.we are using bcos to differ between local and instance var
	this.name = name;
	this.address = address;
	this.email = email;
}
void display()
{
	System.out.println("the rollno is "+rollno+"the name is "+name);
	System.out.println("the address is "+address+"the email is "+email);
	}
public static void main(String[] args)
{
	Constructor ob=new Constructor(101,"sandip","Bangalore","sandip@gmail.com");
	ob.display();
		}
}
---------------------------------------------------------------------------------
wap to enter an employee data and display it using constructor
empno,name,salary,designation
-------------------------------------------------------------------------------
example-17
------------------
package org.sandip;
import java.util.*;
public class ConstructorDemo 
{
int empno;
String name,address,design;
float salary;
public ConstructorDemo(int empno, String name, String address, String design, float salary) {
	this.empno = empno;
	this.name = name;
	this.address = address;
	this.design = design;
	this.salary = salary;
}
void display()
{
	System.out.println("the empno is "+empno);
	System.out.println("the name is "+name);
	System.out.println("the address is "+address+"The design is "+design);
	System.out.println("the salary is "+salary);
	}
public static void main(String[] args) 
{
	Scanner ob=new Scanner(System.in);
	System.out.println("enter empno,name,address,design,salary");
	int empno=ob.nextInt();
	String name=ob.next(), address=ob.next(), design=ob.next();
	float salary=ob.nextFloat();
	
	ConstructorDemo ob1=new ConstructorDemo(empno, name, address, design, salary);
	ob1.display();
}
}
--------------------------------------------
getter and setter
getter is used to get the value
setter is used to set the value.
Example-18
-------------------------
package org.sandip;

public class SetterGetter
{
int empno;
String name,address,design;
float salary;
public int getEmpno() {
	return empno;
}
public void setEmpno(int empno) {
	this.empno = empno;
}
public String getName() {
	return name;
}
public void setName(String name) {
	this.name = name;
}
public String getAddress() {
	return address;
}
public void setAddress(String address) {
	this.address = address;
}
public String getDesign() {
	return design;
}
public void setDesign(String design) {
	this.design = design;
}
public float getSalary() {
	return salary;
}
public void setSalary(float salary) {
	this.salary = salary;
}


}
---------------------------------------------------
package org.sandip;

public class SetGetMain 
{
public static void main(String[] args) {
	SetterGetter ob=new SetterGetter();
	ob.setEmpno(101);
	ob.setName("sandip");
	ob.setDesign("Worker");
	ob.setAddress("Bangalore");
	ob.setSalary(76000);
	System.out.println("the empno is "+ob.getEmpno());
	System.out.println("the name is "+ob.getName());
	System.out.println("the Designation is "+ob.getDesign());
	System.out.println("the address is "+ob.getAddress());
	System.out.println("the salary is "+ob.getSalary());
	}
}
----------------------------------------------------------------------------------
wap to enter productid,productname,productprice
and display it.using getter() and setter().
----------------------------------------------------------------------------
Inheritance --(IS-A) relationship.
java supports single inheritance,multi-level inheritance,hyrarchal inheritance.
It is one of the oops concept.
In this we  reuse the code of the parent class into the child class.
we use the keyword super to access the parent class variables and methods into the child class.
we use the keyword extends to inherite the parent class into the child class.
-----------------------------------------------------------------
java doesnot support multiple and hybrid inheritance.
we use interface in java to perform multiple inheritance.
------------------------------------------------------------------------------------
Aggregation --(Has-a) relationship
Employee has-a address
Bank has-a customer
-----------------------------------------------
Type casting
------------------
They are 2 types
1)implicit casting
2)explicit casting
----------------------------------------------
example-1
-----------------
public class Snippet {
	public static void main(String[] args)
	{
		byte x=10;
		short y=x;
		System.out.println(y);
		
	}
--------------------------------------------------------------------
public class Snippet {
	public static void main(String[] args)
	{
		byte x=10,z=20;
		short y=(short) (x+z);
		System.out.println(y);
		
	}
}
--------------------------------------------------------------
example-2
---------------------
explicit casting
-----------------------
public static void main(String[] args)
	{
		short x=10;
		byte y=(byte) x;
		System.out.println(y);
		
	}
}
--------------------------------------------------------------------
example-1
-----------------
package org.inheritance;

public class Student 
{
int rollno;
String name,address;
public Student(int rollno, String name, String address) {
	this.rollno = rollno;
	this.name = name;
	this.address = address;
}


void display()
{
	System.out.println("The rollno is "+rollno);
	System.out.println("The name is "+name);
	System.out.println("The address is "+address);
	}
}
-----------------------------------------------
package org.inheritance;

public class Marks extends Student
{
int phy,chem,maths;

public Marks(int rollno, String name, String address, int phy, int chem, int maths) 
{
	super(rollno, name, address);
	this.phy = phy;
	this.chem = chem;
	this.maths = maths;
}
void display()
{
	super.display();
	System.out.println("the phy marks is "+phy+"the chem marks is "+chem+"the maths marks is "+maths);
	System.out.println("The total is "+(phy+chem+maths));
	System.out.println("The avg is "+(phy+chem+maths)/3);
	}
public static void main(String[] args) {
	Marks ob=new Marks(101,"sandip","hyd",77,55,56);
	ob.display();
}
}
----------------------------------------------------------------------------------------------------------


