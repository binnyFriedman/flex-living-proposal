# proposals

הצעות מחיר, חשבוניות וכלים נלווים שאני שולח ללקוחות. כל מסמך הוא קובץ HTML עצמאי (RTL, גופן Heebo) שניתן לפתוח בדפדפן, להדפיס או לשמור כ‑PDF.

A collection of the price quotes, invoices, and supporting tools I send to clients. Each document is a self‑contained HTML file you can open in the browser, print, or save as PDF.

## מבנה / Structure

הכל שטוח בשורש הפרויקט. תבנית, חתימה ולוגו (בעתיד) משותפים ברמה העליונה. כל מסמך ללקוח נקרא לפי `{date}-{client}-{type}`.

Everything lives flat at the repo root. Template, signature, and logo (later) are shared at the top level. Each client document is named `{date}-{client}-{type}`.

```
.
├── index.html                              # דף הבית
├── template.html                           # תבנית ליצירת הצעות חדשות
├── signature.png                           # חתימה משותפת
├── signature-pad.html                      # כלי ליצירת/עדכון החתימה
├── 2026-07-03-flex-living-quote.html
├── 2026-07-03-flex-living-invoice-01.html
├── 2026-07-03-flex-living-quote.pdf
├── 2026-07-03-flex-living-logo.png
├── 2026-07-08-malka-shimoni-quote.html
└── 2026-07-08-malka-shimoni-quote.pdf
```

## שמות קבצים / File naming

```
YYYY-MM-DD-{client}-{type}.{ext}
```

| type | דוגמה |
|------|--------|
| `quote` | `2026-07-08-malka-shimoni-quote.html` |
| `invoice-01` | `2026-07-03-flex-living-invoice-01.html` |
| `quote.pdf` | ייצוא PDF |
| `logo` | לוגו ספציפי ללקוח (אם נדרש) |

## הוספת הצעה חדשה / Adding a new quote

1. העתיקו את `template.html` לשם חדש: `YYYY-MM-DD-client-quote.html`
2. מלאו את התוכן והחליפו את `[placeholders]`
3. החתימה נטענת אוטומטית מ-`signature.png` בשורש
4. הוסיפו כרטיס מקשר ב-`index.html`
