# Authentication

In a de-coupled environment where the frontend and backend are developed independently, we need a way of storing credentials securely on the server and the frontend client as well.
Since most apps we build have multiple clients (Android/IOS/Web), we don't use outdated methods like using serverside $SESSION variables.

For storing passwords securely on the server, we use hashing. The most popular algorithm is Bcrypt mentioned in the next section.

The frontend also needs to store some tokens to access the backend which is cryptographically secure such that any modifications to them will leave them invalid. 
We use RSA PKI signing within JWTs for the same. This is also discussed in the next sections.

Apart from these, there are also social sign-on (Login with Google / Facebook) which are also frequently used but are not covered in this guide. Google / Facebook) which are also frequently used but are not covered in this guide.