วิธีใช้งาน WebAR โมเดลแผลไฟไหม้ 3 มิติ

ไฟล์ในชุดนี้
- index.html : หน้า WebAR เวอร์ชันใหม่ ใช้โมเดล GLB ที่คุณอัปโหลด
- base_basic_pbr.glb : โมเดล 3 มิติ

ไฟล์เดิมที่ต้องเก็บไว้ในโฟลเดอร์เดียวกันบน GitHub
- targets.mind : ไฟล์ Image Target ที่สร้างจากโปสเตอร์
- poster-burn-first-aid.png : โปสเตอร์ที่ใช้สแกน (เก็บไว้เป็นภาพอ้างอิง ไม่จำเป็นต้องโหลดในหน้าเว็บ)

วิธีอัปเดต GitHub
1. แตกไฟล์ ZIP นี้ในคอมพิวเตอร์
2. เข้า Repository: burn-first-aid-webar
3. อัปโหลด index.html และ base_basic_pbr.glb จากชุดนี้เข้าไปที่โฟลเดอร์หลัก (root)
4. ถ้ามีคำถามให้ Replace ไฟล์ index.html ให้เลือกแทนที่ไฟล์เดิม
5. ห้ามลบ targets.mind และ poster-burn-first-aid.png
6. กด Commit changes และรอ GitHub Pages อัปเดต
7. เปิด https://noomkub197-lab.github.io/burn-first-aid-webar/ ด้วย Chrome แล้วกด Ctrl+F5
8. กด “เริ่มสแกนโปสเตอร์” และอนุญาตกล้อง จากนั้นส่องโปสเตอร์
9. เมื่อพบโปสเตอร์ ให้ลากนิ้วหรือเมาส์บนภาพเพื่อหมุนโมเดล

ข้อควรทราบ
- ไฟล์ GLB มีขนาดใหญ่ประมาณ 27 MB จึงอาจใช้เวลาสักครู่ในการอัปโหลดและโหลดครั้งแรก
- ต้องวาง base_basic_pbr.glb ไว้ระดับเดียวกับ index.html ห้ามใส่ไว้ในโฟลเดอร์ย่อย เว้นแต่จะแก้ path ใน HTML
- โค้ดนี้ใช้ targetIndex: 0 ตามไฟล์ targets.mind เดิมที่อยู่ในโปรเจกต์
- การหมุนทำได้หลังกล้องตรวจพบโปสเตอร์แล้วเท่านั้น
- ถ้ากล้องยังไม่แสดงภาพ ปัญหาจะเป็นเรื่อง camera/browser/permission ไม่ใช่ไฟล์ GLB
