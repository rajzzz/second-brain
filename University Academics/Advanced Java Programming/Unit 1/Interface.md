Blueprint for a class, Defines a set of abstract methods that a class must implement.

#### Example:
``` java
interface Animal {
  void makeSound();  // abstract method
}

class Dog implements Animal {
  public void makeSound() {
    System.out.println("Bark!");
  }
}

```

**Marker Interface:** A special interface with no methods or fields.