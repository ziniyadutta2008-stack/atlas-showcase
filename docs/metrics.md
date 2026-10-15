# Selected metrics

Read from the public aggregate endpoint on 15 October 2026. The endpoint returns these totals only. It does not return user identifiers, report text, or trace identifiers.

| Metric | Value | Scope |
| --- | --- | --- |
| Combined score | 56 / 100 | Judge average across 7 saved reports |
| Groundedness | 56 / 100 | Judge average across 7 saved reports |
| Citation correctness | 66 / 100 | Judge average across 7 saved reports |
| Structured-output validity | 100% | 7 of 7 chart payloads have a type and a data series the report page can draw |
| Agent completion rate | 100% | 8 of 8 finished jobs completed. 9 jobs are still pending and never started, so they are not in this rate |
| Unsupported-claim rate | 43% | Judge average across 7 saved reports |
| Retrieval hit rate | 1 of 2 | Portfolio Analyst traces that called the vector index and finished. The trace store does not record how many passages came back |
| p95 latency | 102.5s | p95 of the Financial Planner trace. 2 runs |
| Recorded cost/run | $0.00 | Recorded average because Nova Pro has no price in this project. 12,541 tokens across 7 model calls |

How to read the cost and latency figures:

- The recorded cost is the Langfuse average. It is not the AWS bill, and it is not a median.
- p95 latency is the Financial Planner trace across 2 runs. It is not an API gateway latency.

The public site summarises four of these figures as: 100% successful runs, p95 102.5s, 100% structured-output validation, and $0.00 recorded cost/run.
