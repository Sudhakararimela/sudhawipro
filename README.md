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
