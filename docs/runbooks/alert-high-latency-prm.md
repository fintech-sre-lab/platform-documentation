# Runbook: Alert — High Latency

When latency-alert fires for the payment router (PRM):

1. Check Prometheus graphs for request latency.
2. Verify PRM pods are healthy.
3. If CPU high, scale up replicas.
