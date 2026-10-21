# NearExpiry — Stock & Expiry Alert System

A beginner-friendly manual-testing project built with HTML, CSS and vanilla JavaScript. It runs in the browser and stores demo data in `localStorage`.

## How to run
1. Extract the ZIP file.
2. Open `index.html` in Chrome, Edge, or Firefox.
3. Start with Dashboard, then explore the 10 modules in the sidebar.

No server, package installation, or build step is required.

## 10 modules
1. Dashboard — product totals, low-stock, near-expiry and expired summaries.
2. Products — add, edit, search, filter, and prevent duplicate SKU values.
3. Categories — add categories and prevent deleting categories in use.
4. Suppliers — add and view supplier contacts.
5. Stock In — increase quantity and optionally update batch/expiry details.
6. Stock Out — decrease quantity while preventing negative inventory.
7. Expiry Alerts — filter and export alerts.
8. Reports — inventory value and stock summary with CSV export.
9. Activity Log — track key actions and clear the log.
10. Settings — configure low-stock and near-expiry thresholds; reset demo data.

## Main workflow
Add product → choose category and supplier → record incoming stock → monitor expiry/stock alerts → record stock out → review reports and activity log.

## Manual testing ideas
- Add product with missing required fields.
- Add duplicate SKU (should be blocked).
- Add quantity 0 and a negative quantity.
- Try stock-out quantity greater than available stock.
- Test expiry dates yesterday, today, and at the configured threshold.
- Change alert thresholds and confirm Dashboard/Alerts update.
- Try deleting a category that still has products.
- Export CSV and verify headings and rows.
- Reset demo data and confirm sample data returns.

## Important limitations
This is a front-end demo. Data is stored only in the current browser. It has no real authentication, backend, multi-user synchronization, or real supplier integration. The stock-in form updates a product's displayed batch/expiry for simplicity; a production system should store separate batch records.
