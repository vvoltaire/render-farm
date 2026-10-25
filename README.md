# Render Farm `upcoming`

A distributed rendering system for my [C++ path tracer](https://github.com/vvoltaire/path-tracer). It splits render jobs into tiles and runs them across a pool of autoscaling Kubernetes workers.

**Planned:**
- Coordinator service that splits renders into tiles and schedules them across workers
- Worker heartbeats and lease-based reassignment when a worker fails
- Autoscaling workers on Kubernetes based on queue depth
- Live dashboard showing tiles completing in real time
- Benchmarks of render time across 1, 4, and 16 workers

Development starts once the path tracer is complete.
