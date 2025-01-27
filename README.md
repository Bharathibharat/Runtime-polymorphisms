# Runtime-polymorphisms
package runtime.polymorphism;
class Animal{  
  void eat(){
System.out.println("Animals Eat");
}  
}  
class herbivores extends Animal{  
  void eat(){
System.out.println("Herbivores Eat Plants");
} 
  }
class omnivores extends Animal{  
  void eat(){
System.out.println("Omnivores Eat Plants and meat");
} 
  }
class carnivores extends Animal{  
  void eat(){
System.out.println("Carnivores Eat meat");
} 
  }
/**
 *
 * @author 1BSCCSA11
 */
public class RuntimePolymorphism {
 public static void main(String args[]){ 
    Animal A = new Animal();
    Animal h = new herbivores(); //upcasting  
	Animal o = new omnivores(); //upcasting  
    Animal c = new carnivores(); //upcasting  
    A.eat();
    h.eat();
    o.eat();  
    c.eat();  
  
  }  
}  
   

output:
Animals Eat
Herbivores Eat Plants
Omnivores Eat Plants and meat
Carnivores Eat meat
