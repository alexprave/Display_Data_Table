# CS2 Match Activity Calendar

Try here the full version for free > [CS2 Heatmap](https://counter-strike-heatmap-v2.netlify.app/)
also the full version has multiple account support,
You can paste as many steamid64's as u want its gonna process all of them,
One by one and display all of them in the calendar Heatmap,
There is a button where u can toggle them on and off

A contribution-style calendar that visualizes your CS2 match history, inspired by activity graphs from CSRep.gg and GitHub.

## Screenshots

### Require only a SteamID64.
<img width="602" height="486" alt="Image" src="https://github.com/user-attachments/assets/e31f76dd-4092-4486-9639-194ebc93e123" />

### Game type Filters (even for HLTV pro matches)
<img width="1238" height="508" alt="Image" src="https://github.com/user-attachments/assets/8c78714d-8841-4a51-9b6b-e0cfbe6ca375" />

### Month view
<img width="1204" height="1079" alt="Image" src="https://github.com/user-attachments/assets/00005985-ba9c-4f0b-848f-99e7d44162cb" />

### Years view
<img width="1210" height="717" alt="Image" src="https://github.com/user-attachments/assets/e33ea6a5-da88-4936-9f6c-063b809249ca" />

### Themes
<img width="1202" height="1055" alt="Image" src="https://github.com/user-attachments/assets/44478f31-a7cf-4938-924e-fd7cefffc446" />

---

## Latest Updates

### Added Matches Breakdown in the popup
<img width="302" height="206" alt="Image" src="https://github.com/user-attachments/assets/783052fe-960c-41ed-9775-d1f7b3eb6d23" />

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
- **Hover details** — hover over a cell to see its date and match count, and Matches Breakdown.
- <img width="139" height="126" alt="Image" src="https://github.com/user-attachments/assets/7fcc077d-16fd-4be6-bd80-560ec61f3295" />
- **Resizable calendar** — resize the calendar area to suit your screen.
- **Drag and drop** — drop a supported data file into the upload area, or click to select it. After loading, the upload area hides and the calendar is shown.

## Supported data files

The calendar supports these formats:

- `.txt` — plain-text daily match counts.
- `.csv` — comma-separated values.
- `.tsv` — tab-separated values.
- `.xlsx` — Excel workbook.

### TXT format

The exported `.txt` file uses a **tab-separated table**, with one row per day.

```text
date	main-account	Premier	Competitive	Wingman	Faceit	HLTV
2025-09-13	2	2	0	0	0	0
2025-09-15	1	0	1	0	0	0
2025-10-05	6	4	0	2	0	0
2026-01-19	15	10	3	2	0	0
2026-03-12	4	2	0	0	2	0
```

### Columns

* `date` — Match date in `YYYY-MM-DD` format.
* `main-account` — Total matches across all included categories for that day.
* `Premier` — Premier matches.
* `Competitive` — Competitive matches.
* `Wingman` — Wingman matches.
* `Faceit` — Faceit matches.
* `HLTV` — HLTV matches.

**Note:** The example above is illustrative. The actual export includes the categories available in the source data. The `main-account` value is the combined total of the category counts for that day.

### Importing the File

1. Open the heatmap HTML file.
2. Upload the exported `.txt` file.
3. The calendar initially displays **All Matches**.
4. Use the category button to cycle through **All Matches** and the available individual categories.

CSV, TSV, and XLSX files with compatible date, total, and category columns are also supported.

### Legacy TXT Format

The older plain-text format is still supported for files that contain only daily totals:

```text
2025-09-13: 2
2025-09-15: 1
2025-10-05: 6
2026-01-19: 15
2026-03-12: 4
```

Legacy files display the overall match counts, but cannot be filtered by category because they do not contain category-specific data.


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
