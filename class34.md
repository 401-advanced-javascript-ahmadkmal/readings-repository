# Authentication + Role Based Authorization

Authentication is used to protect our applications and websites from unauthorized access and also, it restricts the user from accessing the information from tools like postman and fiddler. In this article, we will discuss basic authentication, how to call the API method using postman, and consume the API using jQuery Ajax.
To access the web API method, we have to pass the user credentials in the request header. If we do not pass the user credentials in the request header, then the server returns 401 (unauthorized) status code indicating the server supports Basic Authentication.

## token

an access token contains the security credentials for a login session and identifies the user, the user's groups, the user's privileges, and, in some cases, a particular application. Typically one may be asked to enter the access token (e.g. 40 random characters) rather than the usual password (it therefore should be kept secret just like a password).

## <Auth />  <Auth capability="read">

react provide tags that will allow to make different views for every user depend on the state of auth 

### <Auth />

after this tag you can put whatever you want to appear in logged in state 

### <Auth capability="read">

after this tag you can put whatever you want to appear in logged in state  and have read capability 