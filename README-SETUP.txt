GGCalendar - GitHub Pages Ready Package

Files:
1. index.html
   - Renamed from GigiCalendar.html because GitHub Pages automatically serves index.html.
   - Modified so a new browser/device automatically fetches ./ggcalendar-backup.json
     when it has no existing local GGCalendar task data.
   - After initial load, edits continue to save in that browser's localStorage.

2. ggcalendar-backup.json
   - Your uploaded JSON backup, unchanged.
   - Contains 242 task records plus settings.

3. ggcalendar-export.csv
   - Regenerated from the JSON so it contains all 242 task records.
   - CSV is for backup/export/reference. The app itself uses JSON for import/initial loading.

IMPORTANT:
- GitHub Pages is normally public on the internet. Anyone with access to the site/files
  may be able to read the calendar data.
- Changes made inside the calendar app are stored only in that browser/device.
  They do NOT automatically write back to GitHub or synchronize to other devices.
- To distribute a newer master calendar to new devices, replace ggcalendar-backup.json
  in the GitHub repository with a newer exported JSON backup.
