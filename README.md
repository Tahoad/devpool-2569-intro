# DevPool 2569 — หน้าเว็บแนะนำตัว

หน้าเว็บแนะนำตัวสำหรับภารกิจรอบคัดเลือก **DevPool 2569 #1 Mini Build Challenge**

โดย **ธตรฐ ไชยศรี (Thatarot Chaisri)** · ผบธ.กบล.ฉ.2

🌐 **เว็บไซต์ (Live):** https://devpool-2569-intro.vercel.app/

## มีอะไรบ้าง
- หน้าเว็บ frontend หน้าเดียว (`index.html`) — ไทย + อังกฤษ
- จัดหน้าด้วย CSS รองรับ **ธีมสว่าง/มืด** (ใช้ CSS variables)
- **Responsive** แสดงผลได้ทั้งมือถือและจอใหญ่
- Interactive ด้วย JavaScript **3 จุด**:
  1. **ปุ่มสลับธีมมืด/สว่าง** (Light/Dark mode)
  2. **ปุ่มเปิด/ปิดกล่องเหตุผลที่สมัคร**
  3. **ช่องค้นหาราคาหุ้น** — ดึงข้อมูลจริงจาก API ภายนอก (`fetch` + `async/await`)
- คอมเมนต์อธิบายโค้ดทุกบรรทัด (HTML / CSS / JS)

## เทคโนโลยี
- HTML5 + CSS3 (CSS variables สำหรับธีม)
- Vanilla JavaScript (ไม่ใช้ library)
- **Alpha Vantage API** — ข้อมูลราคาหุ้น (free tier: 25 ครั้ง/วัน)
- Deploy บน **Vercel**

## โครงสร้างไฟล์
```
devpool-2569-intro/
├── index.html      # หน้าเว็บทั้งหมด (HTML + CSS + JS รวมไฟล์เดียว)
├── avatar.jpg      # รูปโปรไฟล์
└── README.md       # ไฟล์นี้
```

## รันยังไง
เปิดไฟล์ `index.html` ด้วยเบราว์เซอร์ได้เลย — เป็น static page ไม่ต้องมี backend

## วิธีใช้ช่องค้นหาหุ้น
พิมพ์ชื่อย่อหุ้น (เช่น `AAPL`, `TSLA`, `NVDA`) แล้วกดปุ่ม **ค้นหา** หรือกด **Enter**
→ แสดงราคาล่าสุด + การเปลี่ยนแปลง (เขียว = ขึ้น ▲ / แดง = ลง ▼)
