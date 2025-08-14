[README.md](https://github.com/user-attachments/files/21780674/README.md)
# Google Sheets Live Dashboard

This is a **live-updating analytics dashboard** powered by Google Sheets and DataTables.

## 🚀 Features
- **Live data** pulled from Google Sheets (auto-refresh every 2 minutes)
- **Summary cards** with total entries, average score, and latest date
- **Sortable, searchable table** with pagination
- **Responsive design** for mobile and desktop
- **No backend required** — runs entirely in the browser

## 📊 How It Works
1. The dashboard fetches a **published CSV** version of your Google Sheet.
2. It parses the CSV and updates:
   - The **summary cards**
   - The **data table**
3. Data refreshes automatically without reloading the page.

## 📄 Setup
1. Publish your Google Sheet:
   - Open your sheet → **File → Share → Publish to the web**
   - Choose **Entire Document → CSV**
   - Copy the **Sheet ID** from the URL.
2. In `index.html`, replace:
   ```js
   const sheetURL = 'https://docs.google.com/spreadsheets/d/YOUR_SHEET_ID/pub?output=csv';
   ```
   with your Sheet ID.
3. Upload to GitHub and enable GitHub Pages.

## 🌐 Deploy on GitHub Pages
1. Create a **public repository** on GitHub.
2. Upload `index.html` (and optionally this README).
3. Go to **Settings → Pages**.
4. Under **Source**, choose the `main` branch and `/ (root)` folder.
5. Save — your dashboard will be live at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```

## 🛠 Technologies Used
- **HTML, CSS, JavaScript**
- [DataTables.js](https://datatables.net/)
- [Font Awesome](https://fontawesome.com/)

---
💡 *This dashboard is completely client-side — your data remains under your control in Google Sheets.*
