# Architecture

The planned `packages/contracts` layer will define canonical cross-module data. The instrumentation SDK and reference applications will emit traces. `platform-core` will store traces and synchronously invoke reliability evaluation and governance decisions. `mlops` will own datasets, experiments, and the release quality gate. `apps/api` will wire the FastAPI HTTP boundary, while `apps/dashboard` will present results.

Packages must never import from apps. Reliability and governance will depend on contracts, and governance must not import reliability implementation classes. The directories are reserved; implementation files will be added as the project progresses.
