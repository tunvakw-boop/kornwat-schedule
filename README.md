# Kornwat Garden Resort — Employee Schedule

Mobile-friendly employee schedule web app for Kornwat Garden Resort.

## Features
- Tap cells to cycle: ทำงาน → OFF → ครึ่งวัน
- Excel-style month tabs at bottom, `+` to clone next month forward
- Editable Name + Position via popup
- Public holidays marked with ★
- Group/tour names on a vertical footer row per day
- Cloud sync via Supabase (multi-device)
- Export to PNG and PDF
- Works offline (localStorage cache)

## Tech
- Single `index.html` — no build step
- Supabase (REST API) for cloud storage
- html2canvas + jsPDF (loaded from cdnjs) for export
- Sarabun font (Google Fonts)

## Data
Stored in Supabase table `public.schedule_months` (one row per month, JSONB data).
