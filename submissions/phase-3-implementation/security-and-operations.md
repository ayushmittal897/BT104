# Security and Operations

- Bind the API to `127.0.0.1` only.
- Restrict browser access to local dashboard origins.
- Accept only approved CSV feature inputs.
- Keep captured connection metadata in memory; do not store payloads.
- Exclude datasets, PCAP files, local models, dependencies, and secrets from Git.
- Treat any flagged result as an analyst lead, not automatic proof or a response action.

Before production deployment, add exact live feature extraction, independent evaluation, authentication, audit logging, storage controls, and analyst escalation procedures.