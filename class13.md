# class13 - Bearer Authentication

Authorization: Bearer <token>
when the request have this formela we are talking about barearer
this is usualy used when you want to take it from other site you can re use this token to update data to that user

arer Tokens are encoded JSON objects that “bear” or “contain” enough information for the server to assert that any client request that presents a valid token must have originated from a client that has previously authenticated themselves using either Basic or OAuth. Upon receiving a Bearer Token from a client, the server can decode it, inspect the JSON object inside, look up the appropriate account, and re-authenticate the user in a single lookup.
1- Bearer Tokens are sent to the user/client after the initial signin process has completed.
2- Clients must make every subsequent request to the server with that token, in the header

- Authorization: Bearer encoded.jsonwebtoken.here

3- The server opens the token, does the re-authentication, and then grants or denies access
4- In express servers, this can be done in middleware, in conjunction with a user model

## JSON Web Tokens

{
  "alg": "HS256",
  "typ": "JWT"
}
payload
{
  "sub": "1234567890",
  "name": "John Doe",
  "admin": true
}
HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)

this is the form of token and it has alot of info coded with secreat code and you can encoded it by that secreat key also 

this usuly used by your app it self 

JSON Web Token (JWT) is an open standard that defines a compact and self-contained way for securely transmitting information between parties (servers, clients, etc) as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

### When should you use JSON Web Tokens?

#### Authorization:

This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

#### Information Exchange:

JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content