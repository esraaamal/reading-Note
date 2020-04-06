## SuperAgent
SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js

A request can be initiated by invoking the appropriate method on the request object, then calling .then() (or .end() or await) to send the request. 

HTTP method may also be passed as a string
Absolute URLs can be used. In web browsers absolute URLs work only if the server implements CORS.
The Node client supports making requests to Unix Domain Sockets
DELETE, HEAD, PATCH, POST, and PUT requests can also be used, simply change the method name:

DELETE can be also called as .del() for compatibility with old IE where delete is a reserved word.The HTTP method defaults to GET
### Setting header fields
Setting header fields is simple, invoke .set() with a field name and value:

 request
   .get('/search')
   .set('API-Key', 'foobar')
   .set('Accept', 'application/json')
   .then(callback);

You may also pass an object to set several fields in a single call

### GET requests
The .query() method accepts objects, which when used with the GET method will form a query-string. The following will produce the path **/search?query=Manny&range=1..5&order=desc**
 request
   .get('/search')
   .query({ query: 'Manny' })
   .query({ range: '1..5' })
   .query({ order: 'desc' })
   .then(res => {

   });
   The .query() method accepts strings as well Or joined

   ### POST / PUT requests
A typical JSON POST request might look a little like the following, where we set the Content-Type header field appropriately, and "write" some data, in this case just a JSON string.

  request.post('/user')
    .send({ name: 'tj', pet: 'tobi' })
    .then(callback, errorCallback)
Or using multiple .send() calls:

  request.post('/user')
    .send({ name: 'tj' })
    .send({ pet: 'tobi' })
    .then(callback, errorCallback).

***By default sending strings will set the Content-Type to application/x-www-form-urlencoded, multiple calls will be concatenated with &,***    



    
