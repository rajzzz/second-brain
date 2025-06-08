```
public class MyServlet implements Servlet {
	public void init(ServletConfig config)
		throws ServletException
	{
		//initialization code
	}
	//rest of the code
}
```

 **Q**. Why can't we write connected architecture code inside the constructor, since constructor also runs only once in it's entire life.
	We cannot use throw inside the contructor.

**Q** Why it is recommended to use the non parameterized version of init()
	https://www.geeksforgeeks.org/life-cycle-of-a-servlet/#:~:text=Approach%201%3A%20Using%20the%20Parameterized%20init(ServletConfig.con)

