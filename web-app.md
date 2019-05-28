## Why "session" is used?
Web applications use HTTP protocol for communication. Because HTTP is stateless, 
> in order to associate a request to any other request, a way is needed to store user data between HTTP requests.
> Cookies or URL parameters are both suitable ways to transport data between 2 or more request. But it is not safe because cookies and url
> parameters are readable/editable on client side. So a way how we could store that data on server side is needed. 

Session will be created on server side and a corresponding session id will be created and stored there. For your following HTTP requests in the same
session, the server will point you to the correct session data (stored by the server). 

## HTTP requests
stateless. How the server tell your request apart from everyone else's?
### What is HTTP protocol?
The HTTP protocol is a request/response protocol based on client/server based architecture. Hypertext Transfer Protocol is an application-level protocol for distributed, collaborative hypermedia information systems. HTTP is the foundation for data communication for the WWW since 1990.
**Basic Features**:
- HTTP is connectionless: The HTTP client ie.browser initiates an HTTP request and after request is made, the client disconnects from the server and waits for a response. The server process the request and re-establish the connection with the client to send response back.
- HTTP is media independent: 
- HTTP is stateless: The server and client are aware of each other only during current request. Afterwards, both of them forget about each other. 

### HTTP Method
>The request **method** indicates the method to be performed on the resource identified by the givn Request-URI. 
>The method is case-sensitive and should always be mentioned in uppercase.

- **GET** : retrieve information from the given server using a given URI. Request using GET should only retrieve data and should have no other effect on the data.
- **HEAD**: Same as GET, but it transfers the status line and the header section only.
- **POST**: send data to the given server using HTML forms.
- **PUT**: replace all the current representations of the target resource with the uploaded content.
- **DELETE**: remove all the current representations of the target resource given by URI.
- **CONNECT**: establish a tunnel to the server identified by a given URI.
- **OPTIONS**: describe the communication options for the target resource.
- **TRACE**: perform a message loop back test along with the path to the target resource.

### URI(Uniform Resource Identifier) identifying the resource upon which to apply the request
``` Request-URI = "*" | absoluteURI | abs_path | authority ```

