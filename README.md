# 📊 คำนวน Trade Futures (Fixed PnL, PWA)

เว็บคำนวณ Futures สำหรับมือถือ (ไฟล์พร้อมติดตั้งเป็น PWA): PnL • Target • Max Open • Liquidation
ลิงก์ (เมื่อเปิด GitHub Pages): `https://<YOUR_USERNAME>.github.io/futures-calc/`

## ใช้งาน
- เปิด `index.html` ได้ทันที หรืออัปขึ้น GitHub Pages เพื่อใช้งานออนไลน์ & ติดตั้งเป็นแอปได้
- PnL รองรับทั้ง **จำนวนเหรียญ (Qty)** หรือ **Position (USDT)**

## โครงสร้าง
- `index.html` — แอปหลัก
- `manifest.webmanifest` — PWA manifest
- `sw.js` — Service Worker (ออฟไลน์)
- `icons/icon-192.png`, `icons/icon-512.png` — ไอคอน
- `.nojekyll` — ปิดการประมวลผล Jekyll

## เปิด GitHub Pages
Settings → Pages → Source: *Deploy from a branch* → Branch: `main` / Folder: `/`

