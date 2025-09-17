
# Futures Calculator (Static HTML)

ตัวคำนวณ Futures: PnL / ROI / Target / Max / Liquidation (ไฟล์เดียว จบ)  
รองรับการใส่ **Symbol**, แปลง **Position (USDT) ➜ Qty** อัตโนมัติ และ **บันทึกภาพ PNG** พร้อมแสดง Symbol สีฟ้าเด่น

## ใช้กับ GitHub Pages (วิธีที่ง่ายสุด)
1) สร้าง Repo ใหม่บน GitHub (Public แนะนำ) เช่น `futures-calculator`
2) ดาวน์โหลดไฟล์ ZIP นี้ แล้วแตกไฟล์
3) อัปโหลดไฟล์ทั้งหมด (`index.html`, `favicon.svg`, โฟลเดอร์ `.github/workflows/`) เข้าไปใน repo
4) ไปที่ **Settings → Pages**  
   - เลือก **Source: GitHub Actions** (ไม่ต้องใช้ branch `gh-pages`)
5) ไปที่ **Actions** ดู Workflow ชื่อ **Deploy to GitHub Pages** รันให้สำเร็จ 1 ครั้ง
6) กลับมาที่ **Settings → Pages** จะเห็น URL ของเว็บไซต์ พร้อมใช้งานทันที

> ถ้าต้องการใช้ custom domain: ไปที่ **Settings → Pages** เพิ่มโดเมน แล้วตั้งค่า DNS (CNAME) ตามที่ GitHub บอก

## โครงสร้างไฟล์
```
.
├─ index.html                # แอพหลักไฟล์เดียว
├─ favicon.svg               # ไอคอน
└─ .github/
   └─ workflows/
      └─ deploy.yml          # GitHub Actions สำหรับ Pages
```

## ปรับแต่ง
- เปลี่ยนชื่อโปรเจกต์/โลโก้/สี ได้ที่ `index.html` (ส่วน `<style>` และ `<header>`)
- ถ้าจะเปิดโหมด `main → /docs` ก็ได้: ย้าย `index.html` ไปไว้ในโฟลเดอร์ `docs/` แล้วปิด GitHub Actions
- หากต้องการเพิ่ม Banner/ขั้นตอนใน PNG แจ้งผมได้เลยครับ
