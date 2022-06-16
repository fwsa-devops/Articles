# REST API

A REST API (also know as RESTful API) is an **Application Programming Interface** (API or web API) that conforms to the constraints of REST architectural style and allows for interaction with RESTful web services. REST stands for R**epresentational State Transfer** and was created by computer scientist **Roy Fielding**

![rest-api-model](https://user-images.githubusercontent.com/98386787/173993897-af430f27-d5a5-42e6-8a62-19cb7dcd5550.png)

REST is a set of architectural constraints, not a protocol or a standard. API developers can implement REST in a variety of ways. 

When a client request is made via a RESTful API, it transfers a representation of the state of the resource to the requester or endpoint. This information, or representation, is delivered in one of several formats via HTTP: JSON (Javascript Object Notation), HTML, XLT, Python, PHP, or plain text. **JSON is the most generally popular file format** to use because, despite its name, it’s language-agnostic, as well as readable by both humans and machines.

**Something else to keep in mind**: Headers and parameters are also important in the HTTP methods of a RESTful API HTTP request, as they contain important identifier information as to the request's metadata, authorization, uniform resource identifier (URI), caching, cookies, and more. There are request headers and response headers, each with their own HTTP connection information and status codes.


## HTTP Methods

REST APIs enable you to develop all kinds of web applications having all possible CRUD (create, retrieve, update, delete) operations. REST guidelines suggest using a specific HTTP method on a particular type of call made to the server (though technically it is possible to violate this guideline, yet it is highly discouraged).

- HTTP GET
- HTTP POST
- HTTP PUT
- HTTP DELETE
- HTTP PATCH

![CRUD-Operations-What-is-REST-API](https://user-images.githubusercontent.com/98386787/173994324-0c08a983-0c21-4df0-abfb-e10b6b6a94c3.png)

### HTTP GET

Use GET requests to **retrieve resource representation/information only** – and not modify it in any way. As GET requests do not change the resource’s state, these are said to be safe methods.

Making multiple identical requests must produce the same result every time until another API (POST or PUT) has changed the state of the resource on the server.


### HTTP POST

Use POST APIs to **create new subordinate resources**, e.g., a file is subordinate to a directory containing it or a row is subordinate to a database table.

When talking strictly about REST, POST methods are used to create a new resource into the collection of resources.

Responses to this method are not cacheable unless the response includes appropriate Cache-Control or Expires header fields.


### HTTP PUT

Use PUT APIs primarily **to update an existing resource** (if the resource does not exist, then API may decide to create a new resource or not).


### HTTP DELETE

As the name applies, DELETE APIs **delete the resources** (identified by the Request-URI).

### HTTP PATCH

HTTP PATCH requests are to **make a partial update on a resource**.

If you see PUT requests modify a resource entity too. So to make it more precise – the PATCH method is the correct choice for partially updating an existing resource, and you should only use PUT if you’re replacing a resource in its entirety.





### Reference: 
- [Red Hat](https://www.redhat.com/en/topics/api/what-is-a-rest-api)
- [REST API Tutorial](https://restfulapi.net/http-methods/)

