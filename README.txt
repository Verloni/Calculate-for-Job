MasterPro WEB - stage 10 Realtime

Added:
- Supabase Realtime subscription for public.user_calculator_data;
- phone changes appear in the open Web page without manual refresh;
- Web changes appear in iOS without app relaunch;
- stale-state conflict protection remains;
- if a modal is open, a remote update is queued until the modal closes;
- focus/visibility refresh remains only as fallback.

Important:
Supabase Realtime must be enabled for table public.user_calculator_data.

Replace on GitHub:
- index.html
- service-worker.js
