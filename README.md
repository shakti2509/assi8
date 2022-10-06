# assi8
package Ass8;

public class Address {
private String perad,currad,pincode;
public Address()
{
	perad=currad=pincode="";
	
}
public Address(String perad, String currad, String pincode) {
	super();
	this.perad = perad;
	this.currad = currad;
	this.pincode = pincode;
}
public String display()
{
	return "permanent address "+perad+"current address"+currad+"pincoed"+pincode;
}

}
package Ass8;

public class Customer {
	String email;
	Address add;
	public Customer()
	{
		email="abc@gmail.com";
		add=new Address("","","");
	}
	public Customer(String email,Address add)
	{
		this.email=email;
		this.add=add;
		
	}
	public Customer(String email,String a,String p,String pin)
	{
		this.email=email;
	add=new Address(a,p,pin);
	}
	public void display()
	{
		System.out.println("-------------------------");
		System.out.println("email"+email+"Address"+add.display());
	}

}
package Ass8;

public class Democustomer {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

	Customer c=new Customer();
	c.display();
	Customer c1=new Customer("shakti@gmail.com","newyork city","near atlanta ","231222");
	c1.display();
	}

}


