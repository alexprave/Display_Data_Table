# Match Activity Calendar

A simple, offline contribution-style calendar that visualizes your CS2 match history.

Even made a GitHub theme.
<img width="1200" height="247" alt="Image" src="https://github.com/user-attachments/assets/c73147d1-1767-40dd-8319-c398c4653a2f" />
---
Inspired by CSRep.gg activity graphs.
<img width="1200" height="247" alt="Image" src="https://github.com/user-attachments/assets/cddc4e6d-a887-468d-b837-d25e5c4bbeee" />
---

## How to use

1. Open the `Match.html` file in any browser (just double-click it).
2. Click the box **or** drag & drop your data file (`your_data.txt`).
3. The calendar will appear automatically.

No installation, no internet, no extra programs needed.

---

## Data file format (`your_data_filename.txt`)

The file must contain one day per line in this format:

### Example:

2025-09-13: 2
2025-09-15: 1
2025-10-05: 6
2026-01-19: 15
2026-03-12: 4


- Date must be in `YYYY-MM-DD` format
- After the colon put the number of matches that day
- You can add comments with "//" they are ignored 

---

## How to create the data file from your CS2 history


### From Leetify [leetify.com](https://leetify.com)

1. Go to your Progress Report, click on Your 2026 Q3 or the earliest listing
2. Manually note the days you played and how many matches
3. Write them in the format shown above
4. Save as `txt_filename.txt`


### But of course you can use any site you know that has a history like : 

   - [csrep.gg](https://csrep.gg)
   - [csstats.gg](https://csstats.gg/)



### If u have the data just export from Excel / Google Sheets
If you already have an Excel/Google Sheet with columns `Date` and `Matches`:

1. Make sure the date column is in `YYYY-MM-DD` format
2. Create a new column with the formula:

=TEXT(A2,"YYYY-MM-DD") & ": " & B2

3. Copy the results and paste them into a `.txt` file

---------------

## Tips

- You can keep adding new days to the bottom of the `.txt` file anytime.
- The calendar automatically adjusts to the date range in your file.
- Hover over any cell to see the exact date and number of matches.
- Works completely offline.

---

Made for personal use.  
Enjoy tracking your grind.

This is how it looks in your Browser
<img width="1273" height="367" alt="Image" src="https://github.com/user-attachments/assets/f2d00203-4d0d-44ee-bbc5-85288f454bed" />
