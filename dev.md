# คำสั่ง

- Git คือ Version Control แบบ Distributed ตัวหนึ่ง เป็นระบบที่ใช้จัดเก็บและควบคุมการเปลี่ยนแปลงที่เกิดขึ้นกับไฟล์ชนิดใดก็ได้ ไม่ว่าจะเป็น Text File หรือ Binary File (จากนี้จะขอเรียก Text File หรือ Binary File รวมกันว่า Source Code)
- git init >> ไว้สร้าง Git repository
- git status >> ตรวจสอบสถานะไฟล์ของ working directory และ staging area
- git add >> เพิ่มไฟล์ the working directory เข้าสู่ staging area
- git commit >>เก็บประวัติการแก้ไขแบบถาวรจาก staging area ไว้ใน repository
- git fetch :เชคว่าเรากับgit มีไฟล์อะไรต่างกันไหม ***เชคเพื่อแก้ปัญหาอัพไฟล์แก้ไฟล์ไม่ได้ 
- git merge :เอาที่ต่างกันมาโหลดลงให้เหมือนกัน 
- git pull หรือทำทั้ง2อย่าง ***แก้ปัญหาอัพไฟล์แก้ไฟล์ไม่ได้ 
- git clone https://บลาๆ  :เอางานในgit มา
- git log --oneline :สิ่งที่เรา commit ใน 1บรรทัด
- git checktout --ชื่อไฟล์ :ไว้ย้อนกลับข้อความหรือโค้ดในไฟล์ทีนี้อยากจะ reset กู้คืนไฟล์ที่เผลอลบไป เช่น เผลอลบ index.html ก็เพียงแค่ใช้คำสั่ง 1
- git reset HEAD ชื่อไฟล์  :ถ้าเราดันเผลอลบ แล้วก็ยังไป add เข้าสู่ staged แล้ว ก็ต้องใช้  2
- git reset --soft “HEAD^” :แล้วถ้าเราดันไป commit มันซะแล้ว วิธีที่จะย้อนกลับไป commit ล่าสุด 3
- เกิดไฟล์หาย 
    ยังไม่ทำไรคือ ไม่add ไม่commit ทำ 1 
    add ไม่commit ทำ 2, 1 
    add ไม่commit ทำ 3,2,1
- git rm ไฟล์ : ลบไฟล์หลัง commit
- git add . :add ทีหลายๆตัว
- more ไฟล์ : อ่านข้อมูลในไฟล์
- git stash :เพื่อซ่อนสิ่งที่เราอัพเดทไว้ เก็บไว้เพื่อเรียกใช้ตอนหลัง *ซ่อนเอาไว้กันเพื่อใช้ไม่ได้เราก็จะได้ใช้ของเรา ใช้นี้เสร็จต้อง add ไฟล์ที่ซ่อนด้วย 
- git stash pop :เรียกที่เราซ่อนไว้ออกมา *เกิดไม่พอใจของเพื่ออยากเพิ่มของเราที่ซ่อนไว้
- git branch -a :ว่าเรามีสาขาหรือหน่วยที่เก็บ branch
- git branch -d :ลบ branch
- git branch ชื่อที่จะตั้ง :ตั้ง branch ใหม่
- git checkout ชื่อ : ย้ายไป branchนั้นๆ / กลับมาที่ commit number head เดิม
- git checkout -b ชื่อที่ตั้ง :สร้างและย้าย branch
- git merge (ควรใส่ --no-ff) (ชื่อbranch) :อัพข้อมูลจาก branch มา branchที่กำลังอยู่
- git log --online --decorate --graph :ดูกราฟเน็ต กด q เพื่อออก
- git branch -d ชื่อ: ลบ branch
- git push origin --delete ชื่อ: ลบ branch/tag ใน remote
- git checkout (ตัวเลขcommit number/ชื่อ tag) : เลื่อน head ไป commit ครั้งนั้น 1
- git tag ชื่อ: ไว้สร้าง tag 2
- git push --tag : อัพ tag ขึ้น github 3

## การติด tag ตรงตำแหน่งต่างๆ 1,2,3
- git tag -d ชื่อ: ลบ tag

## ซ่อนข้อมูล
- git add .
- git stash
- git pull
- git stash pop
- git add .
- git commit -m ""
- git push origin master


