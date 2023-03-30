# jwt 
## chatgpt 
"jwt" stands for JSON Web Token. It is a standard method for transmitting data securely between parties in the form of a digitally signed and encrypted token. The token contains a JSON payload that is base64 encoded and can be decoded by the recipient using a secret key. It is commonly used for authentication and authorization purposes in web applications and APIs. 

There are several commands related to JWT, but they are usually implemented using libraries or frameworks in programming languages such as JavaScript, Python, and Ruby. Some of the common JWT-related commands include generating a new JWT, verifying the validity and integrity of a received JWT, and decoding the JWT payload to extract the information it contains. For instance, a JavaScript library such as "jsonwebtoken" provides functions such as "sign", "verify", and "decode" to handle JWT-related operations. 

## tldr 
 
> A command-line tool to work with JSON Web Tokens (JWTs).
> Encryption algorithms available are HS256, HS384, HS512, RS256, RS384, RS512, ES256, ES384.
> More information: <https://github.com/mike-engel/jwt-cli>.

- Decode a JWT:

`jwt decode {{jwt_string}}`

- Decode a JWT as a JSON string:

`jwt decode -j {{jwt_string}}`

- Encode a JSON string to a JWT:

`jwt encode --alg {{HS256}} --secret {{1234567890}} '{{json_string}}'`

- Encode key pair payload to JWT:

`jwt encode --alg {{HS256}} --secret {{1234567890}} -P key=value`
