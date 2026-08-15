# Etihad Medical Centre · Fit Certificate Reports

Verified digital copies of medical examination reports issued by **Etihad Medical Centre Limited**, 48/A-B Baitul Khair, Purana Paltan, Dhaka.

## How this works

Every printed report carries a QR code encoding a unique URL like:

```
https://YOUR-USERNAME.github.io/reports/report_view.html?id={patient_id}
```

Scan → the browser opens the report image with a **Download / Print** button.

## Repository structure

```
report_view.html          ← the viewer page (opens on scan)
reports/
  260800008210.jpeg       ← one file per patient
  ...
```

## Adding a new report

1. Save the report image as `{patient_id}.jpeg` (lowercase extension).
2. Upload to the `reports/` folder — GitHub → **Add file → Upload files**, or:
   ```bash
   git add reports/NEWID.jpeg
   git commit -m "Add report NEWID"
   git push
   ```
3. Generate the QR for the new URL (see `github_pages_guide.html` in your local files) and paste it onto the printed certificate.

## Removing a report

Delete the image file. The URL 404s within a minute. Note: git history retains the file — for full deletion, rewrite history.

## Contact

Etihad Medical Centre Limited
E-mail: etihadmedicalbd@gmail.com
Web: www.etihadmedicalbd.com
