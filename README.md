# Tiny App Starter (Static UI + Apps Script JSONP)

This is a single-file template for small decision/search apps.

## What it is
- Static UI hosted on GitHub Pages
- Data loaded from an Apps Script Web App (JSONP to avoid CORS)

## Setup
1) Copy this repo (Use as template)
2) Edit `index.html` config block:
   - `APP_TITLE`
   - `API_BASE` (Apps Script /exec URL)
   - `TREE` (your binary-choice ladder)
3) Enable GitHub Pages (Settings → Pages → main /root)

## Apps Script requirements
Your Apps Script `doGet(e)` must support JSONP:
- `?api=1&callback=NAME` returns `NAME({...});`

## Tagging rules
Your sheet should provide one of:
- `tags` array OR
- `Tags` comma-separated string

## Ship checklist
- [ ] Page loads + shows count
- [ ] Search works
- [ ] Ladder choices filter results
- [ ] No console errors
