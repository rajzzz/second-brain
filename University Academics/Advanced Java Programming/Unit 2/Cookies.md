In [[HTTP Servlets]], cookies are used to store small pieces of information, (key-value pairs) on client side.
These values maintain state across multiple requests (since [[HTTP]] is stateless).

A cookie is represented by the `javax.servlet.http.Cookie` class, sent to the client by the server.

#### Types of Cookies:
There are two main types:
1. [[Session-Cookie]]
2. [[Persistent-Cookie]]


``` java
//creation
Cookie cookie = new Cookie("username", "raj");

//Session Cookie (default), will be delted when browser is closed

//Persistent Cookie
cookie.setMaxAge(60*60*24); //valid for 1 day

//Add cookie to response
response.addCookie(cookie);
```

