# proposals

הצעות מחיר, חשבוניות וכלים נלווים שאני שולח ללקוחות. כל מסמך הוא קובץ HTML עצמאי (RTL, גופן Heebo) שניתן לפתוח בדפדפן, להדפיס או לשמור כ‑PDF.

A collection of the price quotes, invoices, and supporting tools I send to clients. Each document is a self‑contained HTML file you can open in the browser, print, or save as PDF.

## מבנה / Structure

כל לקוח/עסקה יושב בתיקייה עצמאית משלו, וכל הקבצים הקשורים אליו (הצעה, חשבונית, PDF, לוגו, חתימה) נמצאים באותה תיקייה. שמות הקבצים מציינים את תפקידם.

Each client/deal lives in its own self‑contained folder; every file for that deal (proposal, invoice, PDF, logo, signature) sits together. File names state their purpose.

```
.
├── index.html                  # דף הבית – ריכוז כל ההצעות והחשבוניות
├── signature-pad.html          # כלי: יצירת קובץ חתימה (PNG)
├── flex-living-riba-roja/
│   ├── proposal.html           # הצעת מחיר
│   ├── invoice-01.html         # חשבונית
│   ├── proposal.pdf            # ייצוא PDF
│   ├── el-fortin-logo.png      # לוגו הלקוח
│   └── signature.png           # חתימה
└── malka-shimoni/
    ├── proposal.html
    └── signature.png
```

## הוספת הצעה חדשה / Adding a new quote

1. צרו תיקייה חדשה לפי שם הלקוח/העסקה (למשל `acme-corp/`).
2. הוסיפו את הקבצים בשמות תפקיד: `proposal.html`, `invoice-01.html`, `signature.png` וכו'. הכי פשוט להעתיק תיקייה קיימת כתבנית.
3. נכסים בתוך התיקייה מקושרים בנתיב יחסי מקומי (למשל `signature.png`), כך שהתיקייה נשארת עצמאית.
4. הוסיפו כרטיס מקשר בקובץ `index.html`.
