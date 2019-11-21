# HTTP Request

Each HTTP request must contain the header Accept: application/json as all our responses are in JSON format.

**HTTP Success**

Successful HTTP responses have the status code 200 and the body in a format according to documentation of the requested resource.

> You should always check that your HTTP response status code is equal to 200, otherwise the requested was not successful.


**HTTP Errors**

All HTTP requests with response status codes different to 200 must be considered as failed and you should expect additional JSON inside the body of the response with the error message encapsulated inside it as shown in the example. We use the following error codes:

Error Code | Meaning 
---------|----------
 400 | Bad Request – There is something wrong with your request 
 401 | Unauthorized – Your API key is wrong
 403 | Forbidden – Your API key doesnt’t have enough privileges to access this resource
