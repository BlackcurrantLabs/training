# JWT

After authentication is complete, the backend sends a unique token to the frontend. 
This is usually a JWT or JSON Web Token.

JWTs are pure JSON objects which are base64 encoded to make them concise. 
JWTs also support signing with RSA Keys so that if any modifications are made to the token stored in a browser, its signature will not match and the JWT will fail validation.

Apart from this, JWT defines some standards to check expiration, validity, authenticated user, custom fields etc.

!!! tldr "Resource"
    Check out the npm package<br>
    <a href="https://www.npmjs.com/package/json-web-token">https://www.npmjs.com/package/json-web-token</a>

!!! tldr "Resource"
    Check out the online jwt decoder<br>
    <a href="https://jwt.io/">https://jwt.io/</a>

