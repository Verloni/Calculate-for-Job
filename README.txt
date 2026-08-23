MasterPro WEB - stage 11 canonical sync

Synchronization model:
- Supabase is the single source of truth.
- Each client writes _sync.source metadata.
- Own Realtime echo is ignored.
- Foreign Realtime updates are applied immediately.
- 2-second read-only fallback handles temporary WebSocket drops.
- Before save, the browser checks whether another client has newer data.
- Stale local state cannot resurrect deleted projects.

Replace on GitHub:
- index.html
- service-worker.js
