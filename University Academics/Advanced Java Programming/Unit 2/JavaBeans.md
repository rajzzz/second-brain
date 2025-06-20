Software components that adhere to specific set of conventions defined by Oracle.
- essentially Java Classes that encapsulate data and functionality.
- Java Beans follow the principle of "Write Once, Run Anywhere"

#### Characteristics:
- **Public Default Constructor:** no Arguement.
- **Private Fields with Public Accessors:** Encapsulated fields within a Java bean should be declared as private, with public getter and settor methods.
- **Serializable:** should Implement [[Serializable Interface]] interface, enabling data to be saved and restored.
- **Event Supoort:** Java Beans can support events by implementing appropriate listner interfaces, allowing other components to be notified of state changes.

#### Example of a Java Bean:
```java
public class Person implements Serializable {
	private String name;
	private int age;
	public Person(){
		//Default Constructor	
	}	
	//Getter and Setter Methods
	public String getName(){
		return name;
	}
	public void setname(String name){
		this.name = name;
	}
	public int getAge(int Age){
		return Age;
	}
	public void setAge(int Age) {
		this.age = Age;
	}
}
```