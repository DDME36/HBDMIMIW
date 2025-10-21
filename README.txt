Microsite วันเกิด "มิมิว" (Static ZIP)

วิธีเปิด
1) แตกไฟล์ ZIP แล้วดับเบิลคลิกเปิด index.html ด้วยเบราว์เซอร์ (Chrome, Safari, Edge) ได้ทันทีแบบออฟไลน์
2) เสียงจะเริ่มเล่นหลังจากกดปุ่ม "เริ่ม" ครั้งแรก (ตามนโยบาย Autoplay ของเบราว์เซอร์)

โครงสร้างไฟล์
- index.html
- /assets
  - /images   (img01.jpg … img12.jpg)
  - /video    (placeholder.mp4)
  - /audio    (ambient.mp3)
  - /fonts    (ฟอนต์ Mali/Sarabun ที่ฝังภายใน)
- /css/styles.css
- /js/main.js, /js/confetti.js, /js/fireworks.js
- /vendor/gsap.min.js, /vendor/ScrollTrigger.min.js
- /data/config.json

วิธีแก้ไขข้อความ/ฟอนต์/สี
- ชื่อ/คำทักทาย: แก้ไฟล์ index.html หรือปรับค่าใน /data/config.json แล้วค้นหาใช้งานในไฟล์หากต้องการเชื่อมต่อภายหลัง
- ข้อความซับไตเติล/ไทม์ไลน์/จดหมาย: แก้ใน index.html โดยตรง (ภาษาไทยทั้งหมด)
- สีหลัก: แก้ไขตัวแปรใน :root ที่ไฟล์ /css/styles.css (เช่น --peach, --cream, --accent, --text)
- ฟอนต์: ใช้ Mali สำหรับหัวข้อ และ Sarabun สำหรับเนื้อหา ฟอนต์ถูกบันเดิลไว้ใน /assets/fonts

การเปลี่ยนรูป/วิดีโอ/เสียง
- แทนที่ภาพใน /assets/images (ชื่อไฟล์เดิม img01.jpg … img12.jpg หรือแก้ src ใน index.html)
- แทนที่วิดีโอใน /assets/video/placeholder.mp4 แล้วชื่อเดิม หรือแก้ src ของ <video id="surpriseVideo"> ใน index.html
- แทนที่เสียงใน /assets/audio/ambient.mp3

แอนิเมชันและอินเทอร์แอ็กชัน
- ใช้ GSAP + ScrollTrigger แบบไฟล์ท้องถิ่นใน /vendor
- พาร์รัลแลกซ์ Hero, เอฟเฟกต์เข้า/เฟดของไทม์ไลน์, ซองจดหมายเปิด, กล่องของขวัญ+คอนเฟ็ตติ, ปุ่มของขวัญสุดท้าย+ดอกไม้ไฟ
- รองรับ prefers-reduced-motion เพื่อลดแอนิเมชันหนักอัตโนมัติ

หมายเหตุ
- เหมาะสำหรับอุปกรณ์มือถือและเดสก์ท็อป ความกว้างสูงสุด 1100px
- สามารถอัปโหลดขึ้น GitHub Pages ได้ทันที (Static) หากต้องการ
