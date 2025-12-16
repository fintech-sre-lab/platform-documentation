# Post-mortem: 2024-12-20 Latency Spike

Summary: Simulated incident where increased external dependency latency caused higher request times.

Root cause: Downstream payment gateway slowed during peak traffic.

Actions: Add circuit-breaker tuning and more aggressive retries.
