**Java Servlet** is a Java program that runs on a Java-enabled web server or application server.

handles client requests, processes them and generates responses dynamically.

## Types of Servlet:
1. [[Generic Servlets]]
2. [[HTTP Servlets]]
## Creating a basic Servlet:
``` java
import java.io.*;
import jakarta.servlet.*;
import jakarta.servlet.http.*;

public class HelloWorld extends HTTPServlet {
	protected void doGet(HttpServletRequest req, HttpServletResponse rsp)
	
	throws ServletExcetion, IOException {
		response.setContentType("text/html");
		
		PrintWriter out = response.getWriter();
		
		out.println("<html><body>");
		out.println("<h2>Hello, World</h2>")
		out.println("</body></html>);
	}
}
```
## [[Servlet Architecture]]

#java 