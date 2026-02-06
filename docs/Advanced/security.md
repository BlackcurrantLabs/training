# Application Security

Security is a product quality requirement, not a final release checklist.

## High-impact areas

- Authentication and authorization design
- Input validation and output encoding
- Secret management
- Dependency and supply chain risks
- Session and token handling
- Access control and least privilege

## Minimum secure coding baseline

- Validate all external input.
- Use parameterized queries.
- Hash passwords with strong algorithms.
- Enforce HTTPS and secure headers.
- Store secrets in a vault or secure env system.
- Run dependency vulnerability scans in CI.

## Resources

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/)
- [MDN Web Security](https://developer.mozilla.org/en-US/docs/Web/Security)
- [Node.js Security Best Practices](https://nodejs.org/en/learn/getting-started/security-best-practices)
- [Snyk Learn](https://learn.snyk.io/)
