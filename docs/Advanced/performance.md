# Performance Engineering

Performance work is not guesswork. Measure first, optimize second, then re-measure.

## What to optimize

- API latency (p50, p95, p99)
- Throughput under load
- Database query performance
- Frontend page load and interaction speed
- Build and deployment times

## Practical workflow

1. Establish baseline metrics.
2. Profile bottlenecks (CPU, memory, I/O, queries).
3. Optimize one bottleneck at a time.
4. Validate improvements with repeatable tests.
5. Set alerts for regressions.

## Resources

- [Web.dev Performance](https://web.dev/learn/performance/)
- [Node.js Diagnostics Guide](https://nodejs.org/en/learn/diagnostics)
- [PostgreSQL EXPLAIN](https://www.postgresql.org/docs/current/using-explain.html)
- [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview)
- [k6 Load Testing](https://k6.io/docs/)
