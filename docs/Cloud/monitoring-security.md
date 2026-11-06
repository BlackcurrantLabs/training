# Monitoring, Observability & Security

## Topics

- Monitoring vs. observability (metrics, logs, traces)
- Prometheus - scraping metrics, basic PromQL queries
- Grafana - building dashboards, setting alerts
- Security basics: least privilege, never committing secrets to Git, basic image vulnerability scanning, HTTPS/TLS
- Incident response basics: on-call, runbooks, postmortems

## How to learn

- [Prometheus Docs](https://prometheus.io/docs/introduction/overview/) and [Grafana Docs](https://grafana.com/docs/) - both free, official.
- [Google SRE Book](https://sre.google/sre-book/table-of-contents/) - read at least the first few chapters.

## How to practice

Add Prometheus + Grafana to a Kubernetes cluster and build one dashboard showing CPU, memory, and request count. Set up an alert on error rate, and write a one-page runbook for it.

## Resources

- [Prometheus Docs](https://prometheus.io/docs/introduction/overview/)
- [Grafana Docs](https://grafana.com/docs/)
- [Google SRE Book](https://sre.google/sre-book/table-of-contents/)
