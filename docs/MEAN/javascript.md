# Javascript ES6

Javascipt was initally only limited to the browser running very minimal functions, but today we can use Javascript to even on the backend using execution frameworks like nodeJs.

This is great because you now don't have to master two languages (one for frontend and one for backend) to become a full stack engineer anymore.

While node is not the best on performace on the serverside, it can be tuned to be pretty good and will work for most scenarios.

The wide range of open source packages available in npm makes it a really attractive choice for web development.

There are a few crucial language features which you have to learn to write good code both on the frontend and backend.

<a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics">MDN</a> is overall a good place to learn javascript.

Pay special attention to the features listed below.

## Promises
A Quick Intro

<iframe width="560" height="315" src="https://www.youtube.com/embed/RvYYCGs45L4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

A bit more detailed demo

<iframe width="560" height="315" src="https://www.youtube.com/embed/PoRJizFvM7s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


!!! tldr "Resources"
    <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise">MDN</a> has a good post on promises


## Async / Await
Async / Await pattern is the natural extenstion of Promises and is nothing but syntactic sugar to make promises look condensed.
Any promise by default can be treated as an async function call and thus, any promise returning function can be awaited.

Promises in their native form have more control on parallel executions and should be preferred if concurrency is being considered to improve perfomance. It's harder to write concurrent tasks in the async/await syntax.

Quick Video Here

<iframe width="560" height="315" src="https://www.youtube.com/embed/vn3tm0quoqE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

!!! tldr "Resources"
    <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function">MDN</a> has a good post Async/Await

## RxJS
RxJS is basically an event processing pipeline. It's a very important tool to know before getting into Angular / React.
Events can be subscribed at multiple places in an application and so, this becomes a very handy tool to use in multi-component architectures like angular. Using RxJS, you may end up writing significantly less boilerplate code to pass data around.

Watch this video for a Quick Intro here

<iframe width="560" height="315" src="https://www.youtube.com/embed/PhggNGsSQyg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

!!! tldr "Resources"
    To master it, head over to the <a href="https://rxjs.dev/guide/overview">official page</a>.

