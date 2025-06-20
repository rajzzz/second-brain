Remote Method Invocation alllows a Java program on one machine to call methods on an object located on another machine (server).

#### Step 1: Define a Remote Interface
```java 
//MyRemote.java
import java.rmi.*;

public interface MyRemote extends Remote{
	String sayHello() throws RemoteException;
}
```

#### Step 2: Create the Implementation Class:
- Handles Actual logic
- Extends `UnicastRemoteObject`
``` java 
//MyRemoteImpl.java
import java.rmi.*;
import java.rmi.server.*;

public class MyRemoteImpl extends UnicastRemoteObject implements MyRemote {
	protected MyRemoteImpl() throws RemoteException {
		super();
	}

	public String sayHello() throws RemoteException {
		return "Hello from the server!";
	}
}
```

#### Step 3: Create the Server Program
- Instantiates the implementation
- Binds the remote object to the RMI registery
``` java
//RMIServer.java
import java.rmi.*

public class RMIServer{
	public static void main(String[] args) {
		try{
			MyRemoteImpl obj = new MyRemoteImpl();
			Naming.rebind("rmi://localhost:5000/hello, obj");
			System.out.println("Server is ready.");
		} catch (Exception e){
			e.printStackTrace();
		}
	}
}
```

#### Step 4: Create the Client Program
- Looks up the object in the RMI registry
- Calls its methods as if it were local
```java
//RMIClient.java
import java.rmi.*;

public class RMIClient{
	public static void main(String[] args) {
		try{
			MyRemote stub = (MyRemote) Naming.lookup("rmi://localhost/5000/hello"); //Being Typecasted
		} catch (Excetion e) {
			e.printStackTrace();	
		}
	}
}
```

A **Stub** is a client side proxy, local object that looks like the real remote object.