# System Design

System design is about choosing architecture that can scale, stay maintainable, and handle failures.

## Core concepts

- Functional vs non-functional requirements
- Horizontal vs vertical scaling
- Stateless services and stateful dependencies
- Caching strategies
- Async processing using queues
- Idempotency and retry safety
- CAP tradeoffs and consistency levels

## Practice checklist

- Define expected traffic and data growth.
- Identify failure points in every dependency.
- Add timeouts, retries, and circuit breakers.
- Keep API and data contracts explicit.
- Plan migration and rollback before release.

## Resources

- [System Design Primer](https://github.com/donnemartin/system-design-primer)
- [Designing Data-Intensive Applications (book)](https://dataintensive.net/)
- [Google SRE Book](https://sre.google/sre-book/table-of-contents/)
- [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)
