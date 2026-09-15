# Distributed Systems

Distributed systems fail partially, concurrently, and unpredictably. Production design therefore focuses as much on failure semantics as on successful execution.

## Topics

- Timeouts
- Retries
- Exponential backoff and jitter
- Circuit breakers
- Idempotency
- Partial failure
- Delivery semantics
- Consistency models
- Distributed coordination
- Sagas and compensation
- Clock and ordering problems

## Baseline rules

- Every remote call needs an explicit timeout.
- Retries must be bounded and safe.
- Retryable operations should be idempotent.
- Backoff should include jitter.
- Failure of one dependency should not automatically cascade through the system.
- Duplicate messages should be expected when using at-least-once delivery.
- Operational behavior must be observable.

## Review questions

- What happens if this dependency is slow instead of down?
- What happens if a request succeeds but the response is lost?
- Can this operation safely execute twice?
- Where is the source of truth?
- How does the system recover after a partial failure?
- Which consistency guarantees does the business actually require?