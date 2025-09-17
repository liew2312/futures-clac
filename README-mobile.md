
# Futures Calculator – PWA (ติดตั้งเป็นแอพมือถือ)

ไฟล์ชุดนี้ทำให้เว็บ `index.html` ติดตั้งเป็น **Progressive Web App (PWA)** ได้ทั้ง Android / iOS (Add to Home Screen)

## วิธีใช้งานบน GitHub Pages
1) อัปโหลดไฟล์ทั้งหมดไปยัง repo (เช่นสาขา `main`)
2) เปิดใช้งาน **GitHub Pages** (แนะนำโหมด **GitHub Actions**)
3) เปิด URL ของเว็บจาก Pages
4) บนมือถือ:
   - **Android (Chrome):** เมนู ⋮ → *Add to Home screen*
   - **iOS (Safari):** Share → *Add to Home Screen*

> เมื่อเปิดครั้งถัดไปจะทำงานแบบแอพ (เต็มหน้าจอ) และมี **offline cache** สำหรับไฟล์หลัก

## โครงสร้าง
```
.
├─ index.html
├─ manifest.webmanifest
├─ service-worker.js
└─ icons/
   ├─ icon-192.png
   ├─ icon-512.png
   ├─ icon-maskable-192.png
   └─ icon-maskable-512.png
```

## หมายเหตุ
- ถ้ามีการแก้ไขไฟล์ ควรเปลี่ยนเวอร์ชัน cache ใน `service-worker.js` (เช่น `-v2`) เพื่อให้ผู้ใช้ได้รับไฟล์ล่าสุด
- PWA นี้ไม่ใช้เซิร์ฟเวอร์พิเศษ—โฮสต์แบบ static ก็พอ (เช่น GitHub Pages, Cloudflare Pages)
