# 📊 คำนวน Trade Futures (Fixed PnL, Original Scale, PWA)

เวอร์ชันนี้กลับมาใช้ **ค่าสเกลจริง** (ไม่หาร 10) สำหรับ Position Value / Initial Margin / PnL  
ลิงก์เมื่อเปิด GitHub Pages: `https://<YOUR_USERNAME>.github.io/futures-calc/`

ไฟล์:
- `index.html` — แอปหลัก (ค่าสเกลจริง)
- `manifest.webmanifest` — PWA manifest
- `sw.js` — Service Worker (ออฟไลน์)
- `icons/` — ไอคอน 192/512
- `.nojekyll` — ปิด Jekyll

ใช้งาน:
1) แตก zip แล้วอัปโหลดไฟล์ทั้งหมดเข้า repo (public)
2) เปิด Settings → Pages → Deploy from a branch (main / root)
3) เปิดลิงก์ → Add to Home Screen ติดตั้งเป็นแอป
