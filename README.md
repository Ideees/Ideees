import java.util.*;
public class profPra{
public static void main(String[] args) {
Scanner sc= new Scanner(System.in);
double h=0.7,f=9, 
x,e=2.71828183d,exp=0.75,po=2.3d,c=2d,sol1,sol2,sol3,fr1,fr2,approximateValue,trueValue,trueErro
r ; 
System.out.println("Question no 1 ");
System.out.println("Enter value of x in between 1 to 900 : ");
x= sc.nextInt();
while( x<0 || x>900 )
{
System.out.println(" invalid!!! try again");
System.out.println("Enter value of x in between 1 to 900 : ");
x= sc.nextInt();
}
sol1=f*Math.pow(e,exp*po);
sol2=f*Math.pow(e,exp*x);
fr1=sol1-sol2;
approximateValue=fr1/h;
trueValue =3.5*Math.pow(e,exp*x);
trueError=trueValue-approximateValue;
System.out.println("True Error is "+trueError);
fr2=trueError/trueValue;
System.out.println("Relative error is "+fr2);
sol3=fr2*100;
System.out.println("as a percentage is "+sol3+"%");
}
}
