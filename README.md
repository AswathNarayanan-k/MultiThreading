package aaaaaa;
 class Add extends Thread
 {
	 public void run()
	 {
		 for(int i = 0; i<=5;i++)
		 {
			 System.out.println("Sum");
			 try
			 {
				 Thread.sleep(1000);
			 }
			 catch(Exception e)
			 {
			 }
		 }
		 
		
		 
	 }
 }
 class Kick extends Thread 
 {
	 public void run()
	 {
		 for (int i = 0; i<= 5;i++)
		 {
			 System.out.println("Kicker");
			 try
			 {
				 Thread.sleep(1000);
			 }
			 catch(Exception e)
			 {
			 }
		 }
		 
		
	 }
	 
 }

public class MultiThread {

	public static void main(String[] args) {
		Add o = new Add();
		Kick p = new Kick();
		
		o.start();
		p.start();
		   

	}

}
