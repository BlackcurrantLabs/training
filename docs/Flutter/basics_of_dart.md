# Dart

Dart is a programming language designed for client development, such as for the web and mobile apps. It is developed by Google and can also be used to build server and desktop applications. It is an object-oriented, class-based, garbage-collected language with C-style syntax.

<iframe width="560" height="315" src="https://www.youtube.com/embed/5F-6n_2XWR8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Sound null safety


Now Dart language supports sound null safety. When you opt into null safety, types in your code are non-nullable by default, meaning that variables can’t contain null unless you say they can. With null safety, your runtime null-dereference errors turn into edit-time analysis errors.

If you want a variable of type String to accept any string or the value null, give the variable a nullable type by adding a question mark (?) after the type name. For example, a variable of type String? can contain a string, or it can be null.

!!! tldr "Resources"
    To know more about Dart null sound safety, head over to the <a href="https://dart.dev/codelabs/null-safety">official codelab.</a>.

    To try official online Dart compiler, <a href="https://dartpad.dev">click here.</a>


## Asynchronous programming

Asynchronous operations let your program complete work while waiting for another operation to finish. Here are some common asynchronous operations:

●   Fetching data over a network. 

●   Writing to a database. 

●   Reading data from a file. 

Such asynchronous computations usually provide their result as a Future or, if the result has multiple parts, as a Stream. These computations introduce asynchrony into a program. To accommodate that initial asynchrony, other plain Dart functions also need to become asynchronous.

To interact with these asynchronous results, you can use the async and await keywords. Most asynchronous functions are just async Dart functions that depend, possibly deep down, on an inherently asynchronous computation.

    // Exapmle 

    Future<void> fetchUserOrder() {
        // Imagine that this function is fetching user info from another service or database.
        return Future.delayed(const Duration(seconds: 2), () => print('Large Latte'));
    }

    void main() {
        fetchUserOrder();
        print('Fetching user order...');
    }

Output: 

    Fetching user order...
    Large Latte

!!! tldr "Resources"
    To know more about Asynchronous programming, read <a href="https://dart.dev/codelabs/async-await">official documentation.</a>
