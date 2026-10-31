# MyGame: HSK1 จับคู่คำศัพท์

แอปฝึกคำศัพท์ (จีน HSK1–2, ญี่ปุ่น N5, เกาหลี, กวางตุ้ง) มี 6 โหมด: จับคู่คำ, เติมคำ, เรียงประโยค, คำผสม, ฝึกฟัง, บทสนทนา

เป็นเว็บแอป (PWA) ที่ติดตั้งลงมือถือได้ และเล่นออฟไลน์ได้หลังจากเปิดครั้งแรก
ความคืบหน้าและคลังคำที่ตอบผิดจะเก็บไว้ในเครื่อง (localStorage)

## ไฟล์
- `index.html`: ตัวเกมทั้งหมด
- `manifest.webmanifest`, `icons/`: ชื่อแอปและไอคอนตอนติดตั้ง
- `sw.js`: service worker สำหรับเล่นออฟไลน์ (แก้ `index.html` แล้วให้เปลี่ยน `VERSION` ใน `sw.js` ด้วย)

## เปิดใช้งานผ่าน GitHub Pages
1. Settings → Pages → Source: *Deploy from a branch* → Branch `main` / `(root)` → Save
2. รอ 1–2 นาที แล้วเปิด `https://winmawin1.github.io/MyGame/`

## ติดตั้งลงมือถือ
- **iPhone (Safari):** ปุ่มแชร์ → "เพิ่มไปยังหน้าจอโฮม"
- **Android (Chrome):** เมนู ⋮ → "ติดตั้งแอป" / "เพิ่มลงในหน้าจอหลัก"

## รันในเครื่อง
```
python3 -m http.server 8000
```
แล้วเปิด http://localhost:8000
