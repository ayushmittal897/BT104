# CURRENT IMPLEMENTATION STAGE

## Purpose

This branch is reserved for the runnable Sentinel hybrid intrusion-detection implementation, separate from the Phase II planning material on `main`.

## Current implementation boundary

The local project contains:

- `sentinel-ids-source/` — React/TanStack dashboard.
- `backend/server.py` — local FastAPI inference API.
- `backend/live_capture.py` — bounded local TCP/UDP connection-metadata capture.
- `DOC-20261012-WA0010.py` — legacy offline CSV rule and Random Forest prediction workflow.
- `inspect_labels.py` — CICIDS label inspection utility.
- `submissions/` — Phase I, Phase II, Mid-Term, and Phase III capstone evidence.

## Local run procedure

Start the local API:

```powershell
cd "C:\DRIVE D\PROJECTS\CODEX_HYBRID_IDS"
.\.venv\Scripts\Activate.ps1
python -m uvicorn backend.server:app --host 127.0.0.1 --port 8000
```

In a second terminal, start the dashboard:

```powershell
cd "C:\DRIVE D\PROJECTS\CODEX_HYBRID_IDS\sentinel-ids-source"
npm install
npm run dev
```

Open `http://localhost:8080`.

## Security and repository policy

Do not commit CICIDS datasets, PCAP/PCAPNG files, local virtual environments, `node_modules`, `.env` files, or trained binary model artifacts. The repository should contain code, dependency manifests, configuration templates, documentation, and reproducible instructions only.

## Verification status

The branch and this guide were created on 2026-10-30. The local source transfer remains pending because the Codex terminal helper could not read the local working tree after Git ownership setup failed. Source files must be staged and committed from the user's local PowerShell session before this becomes a runnable GitHub branch.
