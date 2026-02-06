# NextJS

<img src="/assets/nextjs.png">

We use NextJS to develop non-corporate / non-financial apps, 
that don't have strong regulatory requirements to host in a particular region ect.
Next behaves the best with vercel based deployments, in which we lack some finegrained conrols like VPC, public and private subnets ect.

Next is highly optimized for landing pages,
we can get some of the best lighthouse scores using next compared to Angular.

In the following sections, we will explore the relevant tools and open souce libraries from the React Ecosystem which make us stick to best practises and our everyday tasks can be sped up.

We don't use `create-react-app` schemantics for react projects as it's quite outdated. Even if the app does not require serverside rendering, we still use Next as it's highly optimized in code splitting and lazy loading.

!!! success "We use nextjs 14 with app router"
    Do not follow any tutorials for older next versions or pages router as things are significantly differnet there.

## Backend or no Backend ?

NextJS project has a place to put in API routes which means we don't have to create a seperate project for the backend like it's mandatory in Angular or Plain React. 
But the backend capabilities of NextJS are limited and when we need to run a more complex backend which has features like :

- queues
- crons
- stateful connections to outside world with static ips
- redis
- wss / socketio

We would need to run our own backend with express seperately.
This means that out project will have 2 backends, one powered with express and one with nextjs. 
There are many caveats in making this decision and many pros / cons have to be weighed which are always project specific. 
This is outside the scope of a fresher and a senior will make these decisions.

## Youtube channels

Subscribe for good quality content on React + Next Ecosystem and to be constantly updated with new developments in the ecosystem.

- <a href="https://www.youtube.com/@ByteGrad" target="_blank">https://www.youtube.com/@ByteGrad</a> 
- <a href="https://www.youtube.com/@t3dotgg" target="_blank">https://www.youtube.com/@t3dotgg</a> 

## Advanced nextjs topics to practice

- Rendering strategy tradeoffs (SSR, SSG, ISR, client rendering)
- Caching and revalidation strategy
- API error handling and typed contracts
- Performance budgets and Core Web Vitals
- Auth flows with middleware and role checks
- Monitoring production behavior

!!! tldr "Resources"
    - [Next.js Learn](https://nextjs.org/learn)
    - [Next.js Docs](https://nextjs.org/docs)
    - [React Docs](https://react.dev/learn)
    - [Vercel Architecture Patterns](https://vercel.com/guides)
    - [Web.dev Core Web Vitals](https://web.dev/articles/vitals)
