[[XSS]] or Cross-Site Scripting allows attackers to inject malicious code into web pages.  To prevent it:

## 1. Input Validation:
Always Validate and Sanitize user input on both client and server side.

## 2. Output Encoding:
Data should be encoded before being displayed so that scripts are not interpreted as code.

## 3. Use Security Headers:
Implementing [[HTTPS]] headers like Content-Security-Policy ([[CSP]]) to restrict which scripts can run on the web page.

## 4. Avoiding `innerHTML` or `eval()`:
Avoid inserting raw user data using dangerous methods like eval, [[innerHTML]] and `document.write`, whcih can execute code directly.

## 5. Use Trusted Libraries and Frameworks:
Like React, Angular, 3js.