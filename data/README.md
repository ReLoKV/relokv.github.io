# Data and Field Notes

This release contains a proposed field dictionary, not experimental request
records. `schema.csv` specifies metadata requirements for future releases.
It is not a sample trace and does not claim that every field is implemented.

## Workload Scope

- Sequential conversations: histories grow over turns and may be revisited
  after intervening tasks.
- Parallel document tasks: multiple compatible adapters process a shared
  source document, subject to exact-prefix and version constraints.
- Negative cases include new sessions, new contexts, incompatible KV states,
  low reuse, and long return intervals.

Behavior order and request text are constructed separately. App-to-task,
adapter, and session mappings are experimental annotations, not native source
dataset labels. Actual dataset versions, selection rules, sample counts,
licenses, and split boundaries are not released in this version.

## Field Dictionary

See `schema.csv`. Units are part of each field definition. Request identifiers
must be remapped within the release, with no private identity mapping provided.
Timestamps should be relative to the replay origin when absolute dates are
unnecessary. These steps reduce direct disclosure but do not guarantee that
records cannot be reidentified.

Failed and timed-out requests remain present. Missing latency measurements
must remain missing, never replaced with zero.

Preparation is a separate event stream. A future release must document how
request records link to deduplicated preparation jobs, completion, cancellation,
expiry, and matching consumption.

## Access and Restrictions

No user conversation text, original behavioral trace, adapter checkpoint, or
measured result is distributed in this preview. A future release must specify
permissions and source access conditions before redistributing any data.
