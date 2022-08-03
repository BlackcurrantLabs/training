# Hashing & Bcrypt

Hashing is not new and various methods of hashing like SHA-1 SHA-256 MD5 are all very popular. 
But the problem with storing a hashed password is that someone can maintain a table of frequently used passwords along with their hashes and simply query this table for a quick attack.

Since hashes are always deterministic, to get away from this problem, we use salting.

## Salting
Salting is the process of adding a unique bit of secret specific to your application to the password and then hashing it. 
If what you add is unique, then the hash cannot be present in any pre-computed hash tables.

## Bcrypt
Bcrypt hashes combine these best practices and provide not only a unique salt per application but a unique salt per password.
These are conveniently wrapped together in a string that can be safely stored in the database.

!!! tldr "Resource"
    Check out the npm package<br>
    <a target="_blank" href="https://www.npmjs.com/package/bcrypt">https://www.npmjs.com/package/bcrypt</a>