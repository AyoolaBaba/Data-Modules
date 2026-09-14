# HTTP

HTTP stands for Hypertext Transfer Protocol. It is the protocol often used to transfer data between two applications, most commonly: a client and a server on the web, it also works for documents or html files and also between apps and servers to name a few.

- A client sends a request, a server sends back a response.
- Requests include a method, a URL, headers, and sometimes a body.
- Common methods: GET(requests a representation of a specoified recourcse), POST(submits an entity to the specified recourcse), PUT(asks for a response identicalto a GET request, but without the hard text body), PATCH(partital modidications to a recourse), DELETE(self explanatroy).
- Responses include a status code, headers, and sometimes a body.
- Status codes indicate the result: 2xx for success, 3xx for redirects, 4xx for client errors, 5xx for server errors.
- HTTP is stateless. Each request is handled independently, with no memory of previous requests.
- Cookies are small data stored by the client, sent back on future requests used for sessions, preferences, and tracking and Work around HTTP's stateless nature.

# JSON

JSON stands for JavaScript Object Notation. It is a text format used to store and exchange data.

- Data is stored as key-value pairs, similar to a Python dictionary.
- Keys are strings, written in double quotes.
- Values can be strings, numbers, booleans, null, arrays, or nested objects.
- JSON is language-independent and widely used for API requests and responses.
- Python includes a `json` module to convert between JSON and Python objects (`json.load`, `json.dumps`, etc).

# API

Application programming interface, a set of rules to communicate between software using standard HTTP requests.


# REST Concepts

REST stands for Representational State Transfer. It is an architectural style for designing APIs. Constraints: client-server communication(so sommunication between the user interface and the server sending back json stuff), statelessness(no state is stored on teh server, it gets everything from user then returns back json and you need to layer with things like cookies to store data), cachebillity(, layered system, uniform interface.

- Resources (e.g. users, orders) are represented by URLs.
- Actions on resources are performed using HTTP methods (GET, POST, PUT, DELETE).
- REST APIs are stateless, matching the stateless nature of HTTP.
- Responses are usually returned in JSON format.
- REST is not a strict protocol, it is a set of conventions and constraints for building consistent APIs.

# REST Implementation

This covers how REST concepts are put into practice when building an API.


- Each resource gets its own endpoint (e.g. `/customers`, `/orders`).
- HTTP methods map to actions: GET reads data, POST creates data, PUT/PATCH updates data, DELETE removes data.
- Status codes confirm the result of each request (e.g. 200 OK, 201 Created, 404 Not Found).
- Endpoints often accept parameters, either in the URL path, query string, or request body.
- Frameworks (e.g. Flask, FastAPI) are commonly used to build REST APIs in Python.
