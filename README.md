package inherited;

class calculation{
  int x=10,y=5,z;
  void add(){
    z=x+y;
    System.out.println("Sum of numbers is "+z);
  }
    //new
    void multiple()
    {
      z=x*y;
      System.out.println("Multiplication of number"+z);  
    }
}
     class my_calculation extends calculation
     {
     void sub()
     {
       z=x-y;
       System.out.println("Substraction of number is "+z);
     }  
       void div()
       {
         z=x/y;
         System.out.println("division of number is "+z);
       }
  }
//public class inherited {
   public class inherited{
  public static void main(String[] args) {

   my_calculation obj=new my_calculation();
  obj.add();
  obj.multiple();
  obj.sub();
  obj.div();
  }
}
