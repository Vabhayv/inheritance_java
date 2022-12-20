# inheritance_java
import java.util.Scanner;

public class inhertitance {
                    int age; 
                    String name;
                    Scanner sc =new Scanner(System.in);
                    void getBase()
                    {

                     System.out.println("enter the name =");
                      name =sc.next();
                      System.out.println("enter the age =");
                      age =sc.nextInt();

                    }
                    void show_base()
                    {
                      System.out.println("NAME :"+name);
                      System.out.println("AGE :"+age);                  
                    }
}
                
                   class child extends inhertitance
                    {
                         String branch;
                         int semester;
                         void getchild(){
                                        System.out.println("enter the BRANCH =");
                                        branch =sc.next();
                                        System.out.println("enter the sem =");
                                        semester =sc.nextInt();
                         }
                         void showchild()
                         {
                                        System.out.println("BRANCH :"+branch);
                                        System.out.println("SEMESTER :"+semester); 
                         }
                         public static void main (String args[]){
                                        child object = new child();
                                        object.getBase();

                                        object.getchild();
                                        object.show_base();
                                        object.showchild();

                    }
}
