# 🏆 President's Club Dashboard

Live BDR performance dashboard that pulls data directly from Google Sheets.

## Deploy to Vercel

```bash
cd presidents-club
npx vercel
```

Or connect this repo to Vercel for auto-deploys on push.

## Swap the Google Sheet

Open `index.html` and change the `SHEET_ID` constant at the top of the `<script>` block:

```js
const SHEET_ID = 'your-new-sheet-id-here';
```

The sheet ID is the long string in your Google Sheets URL:
`https://docs.google.com/spreadsheets/d/THIS_PART_HERE/edit`

## Requirements

- Sheet must be **publicly shared** (Anyone with the link → Viewer)
- First table must have a header row with "Rep" and "Totals" columns
- Expected columns: Rep | Meetings Set | Meetings Held | Show Rate | ARR | Supered | Totals
- Data auto-refreshes every 5 minutes
