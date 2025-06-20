1. **Translation:** 
	1. The JSP page is translated into a Java Servlet file by the container.
	2. Happens only once, the first time the page is requested.
2. **Compilation:** 
	1. The generated Servlet file is compiled into a `.class` file(bytecode).
3. **Loading & Instantiation:** 
	1. The servlet class is loaded into memory and an instance of it is created.
4. **Initialization:** 
	1. Called **once** when the JSP is initialized. 
	2. We us this for one-time setup tasks like DB connections.
	3. `jspInit`
5. **Request Handling:**
	1. Called **everytime** the page is requested.
	2. This is where our main [[JSP]] logic is executed.
	3. `jspService(HttpServletRequest, HttpServletResponse)`
6. **Destruction:**
	1. Called **once** when JSP is removed from the memory
	2. `jspDestroy()`

