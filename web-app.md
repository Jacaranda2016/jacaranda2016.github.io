## Why "session" is used?
Web applications use HTTP protocol for communication. Because HTTP is stateless, 
> in order to associate a request to any other request, a way is needed to store user data between HTTP requests.
> Cookies or URL parameters are both suitable ways to transport data between 2 or more request. But it is not safe because cookies and url
> parameters are readable/editable on client side. So a way how we could store that data on server side is needed. 

Session will be created on server side and a corresponding session id will be created and stored there. For your following HTTP requests in the same
session, the server will point you to the correct session data (stored by the server). 

## HTTP requests
stateless. How the server tell your request apart from everyone else's?

### HTTP Method
>The request **method** indicates the method to be performed on the resource identified by the givn Request-URI. 
>The method is case-sensitive and should always be mentioned in uppercase.

- **GET**
- **HEAD**
- **POST**
- **PUT**
- **DELETE**
- **CONNECT**
- **OPTIONS**
- **TRACE**

### URI(Uniform Resource Identifier) identifying the resource upon which to apply the request
``` Request-URI = "*" | absoluteURI | abs_path | authority ```
