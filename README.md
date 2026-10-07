# Dashboard Summary Produksi — Realtime

Dashboard statis (HTML + Chart.js) yang membaca data **realtime** langsung dari Google Spreadsheet via CSV export.

- Sumber: `https://docs.google.com/spreadsheets/d/1WUtM91KRz_wqn-O0PUUxkmVlNH121b-lO2LprzOFIcM/export?format=csv&gid=380089557`
- Auto-refresh tiap 60 detik (dapat diubah di UI, min 15 dtk)
- Filter: Bulan, Shift, Produk, Leader + pencarian
- Deploy: Vercel (static, tanpa build step)

## Jalankan lokal

Buka `index.html` di browser, atau:

```bash
npx serve .
```

## Deploy ke Vercel

```bash
vercel --prod
```

Pastikan sharing Google Sheet = **Anyone with the link → Viewer** agar fetch CSV berhasil.
