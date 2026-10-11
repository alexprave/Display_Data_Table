# CS2 Match Activity Calendar

Try here for free > [CS2 Heatmap](https://counter-strike-heatmap.netlify.app/)

A contribution-style calendar that visualizes your CS2 match history, inspired by activity graphs from CSRep.gg and GitHub.

## Screenshots

### Require only a SteamID64.
<img width="639" height="370" alt="Image" src="https://github.com/user-attachments/assets/9366eb69-6a1a-4b4a-88ef-3eb01db437ce" />

### Month view
<img width="1204" height="1079" alt="Image" src="https://github.com/user-attachments/assets/00005985-ba9c-4f0b-848f-99e7d44162cb" />

### Years view
<img width="1206" height="719" alt="Image" src="https://github.com/user-attachments/assets/2315e2d0-e6cb-412b-a557-9c6b261c9de9" />

### Themes
<img width="1202" height="1055" alt="Image" src="https://github.com/user-attachments/assets/44478f31-a7cf-4938-924e-fd7cefffc446" />

---

## Features

- **CS2 match activity data table** — see how many matches you played on each day.
- **Two calendar layouts**
  - **Years view:** a weekly contribution-style calendar, separated by year.
  - **Month view:** 12 horizontal month rows, with days running from left to right.
- **View switching** — Month view and Years view are mutually exclusive.
- **Show numbers** — toggle match counts inside calendar cells in either view.
- **Month markers** — optionally show month labels in Years view. This control is hidden in Month view, where it is not needed.
- **Multiple themes** — CSRep, GitHub, Leetify, and Windows XP.
- **Second-account support** — when second-account data is available, toggle it to include those matches in the calendar.
- **Hover details** — hover over a cell to see its date and match count.
- **Resizable calendar** — resize the calendar area to suit your screen.
- **Drag and drop** — drop a supported data file into the upload area, or click to select it. After loading, the upload area hides and the calendar is shown.

## Supported data files

The calendar supports these formats:

- `.txt` — plain-text daily match counts.
- `.csv` — comma-separated values.
- `.tsv` — tab-separated values.
- `.xlsx` — Excel workbook.

### TXT format

For plain-text files, use one day per line:

```text
2025-09-13: 2
2025-09-15: 1
2025-10-05: 6
2026-01-19: 15
2026-03-12: 4
```

- Dates must use `YYYY-MM-DD`.
- Put the number of matches after the colon.
- Lines containing comments beginning with `//` are ignored.

### CSV, TSV, and XLSX

For spreadsheet files, use columns containing the date and the number of matches, such as `Date` and `Matches`. Use dates in `YYYY-MM-DD` format where possible.

Example:

| Date | Matches |
| --- | ---: |
| 2025-09-13 | 2 |
| 2025-09-15 | 1 |
| 2025-10-05 | 6 |

## How to use

1. Open `Match.html` in a browser (usually by double-clicking it).
2. Click the upload area or drag and drop a supported data file.
3. The calendar will appear automatically after the file is loaded.
4. Use the controls to switch themes and layouts, show or hide numbers, and include second-account matches when available.

## Getting your match history

You can prepare the data manually from a match-history service such as:

- [Leetify](https://leetify.com)
- [CSRep](https://csrep.gg)
- [CSStats](https://csstats.gg)

The exact export options depend on the service. If you have the data in Excel or Google Sheets, you can also save it as CSV/XLSX or prepare a TXT file in the format above.

For a spreadsheet with `Date` in column A and `Matches` in column B, just hit File > Download > and chose one of supported files
```



## Tips

- Add new dated lines to your TXT file whenever you have more match data.
- The calendar adjusts to the date range found in the uploaded data.
- Hover over a cell to check the exact date and match count.
- Keep a backup of your source data so you can rebuild the calendar later.

## Notes

- The calendar itself runs in your browser. Some file types, especially `.xlsx`, may require an internet connection to load the spreadsheet-reading library.

---

Made for personal use. Enjoy tracking your grind.
