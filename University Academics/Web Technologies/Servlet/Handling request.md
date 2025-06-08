1. The container creates ``ServletRequest`` and ``ServletResponse`` objects.
   For HTTP requests, it creates `HttpServletRequest` and `HttpServletResponse` objects. 

2. Invoke the [[service()]] Method
   
   `service(ServletReqest req, ServletResponse res)`
   determines the type of HTTP request: (GET, POST, PUT, DELETE, etc.)	 
   and delegates the request to the appropriate method(doGet(), doPost(), etc).
