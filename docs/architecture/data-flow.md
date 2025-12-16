# Data flow

Detailed flows: differences between ISO 8583 and 3DS paths.

Example:

1. Message arrives at ISO gateway
2. Parse fields and enrich
3. Score in fraud service
4. Persist velocity counters in Redis
