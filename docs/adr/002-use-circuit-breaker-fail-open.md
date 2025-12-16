# ADR 002 — Use circuit breaker (fail-open)

Status: Accepted

Decision: Circuit breakers are used but configured to fail-open on timeout to prioritize availability.

Consequences: Faster fallback, but may allow degraded requests through.
