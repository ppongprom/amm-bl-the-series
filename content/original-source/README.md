# ต้นฉบับดิบ — Source of Truth ระดับล่างสุด

ไฟล์ในโฟลเดอร์นี้แปลงมาจาก `drive-download-20260920T072749Z-1-001.zip`
(.docx → .md ด้วย pandoc, `--wrap=none`) เพื่อไม่ให้เกิดปัญหาซ้ำแบบวันที่ 20 ก.ย. 2569
ที่แตกไฟล์ไว้ใน scratchpad ชั่วคราวแล้วหายไปตอน auto-cleanup — ไฟล์พวกนี้เขียนลง repo
ถาวรตั้งแต่แรกแทน

## ไฟล์ในนี้คืออะไร

- `ep01.md` – `ep10.md` — เนื้อเรื่องนิยายต้นฉบับเต็มทั้ง 10 ตอนแรก (Season 1)
- `continuity-bible.md` — ต้นฉบับดิบของ continuity bible (**ไม่ใช่** ฉบับทำงานที่แก้ไขต่อเนื่อง)
- `character-visual-prompts.md` — ต้นฉบับดิบของ character prompt (**ไม่ใช่** ฉบับทำงาน)
- `environment-reference-by-episode.md`, `environment-reference-prompts.md` — ยังไม่เคย
  ถูกนำมาใช้ในไฟล์ทำงานใดๆ ของ repo นี้มาก่อน (ยังไม่ตรวจสอบเนื้อหา)

## ⚠️ ห้ามสับสนกับไฟล์ทำงานใน `docs/`

`docs/continuity-bible.md` และ `docs/character-visual-prompts.md` คือ **ฉบับทำงานจริง**
ที่ถูกแก้ไข/เพิ่มกฎใหม่ต่อเนื่องหลังจากตรวจ generate จริง (Color Anchor Lock, Character
Scale Table, Fictional Weather Table, Brand/Logo Lock ฯลฯ — ดู commit history) —
**อ้างอิงงาน generate/เขียน shorts-prompt จาก `docs/` เท่านั้น อย่าอ้างจากโฟลเดอร์นี้**

โฟลเดอร์นี้มีไว้เป็น **ต้นฉบับอ้างอิงย้อนกลับ** เวลาต้องเช็คว่าเนื้อหาที่แก้ไปใน `docs/`
เบี่ยงจากต้นฉบับดิบไปมากแค่ไหน หรือกู้คืนข้อมูลที่อาจหลุดหายระหว่างแก้ไข — ไม่ใช่ที่แก้ไขต่อ

ตรวจสอบแล้ว (21 ก.ย. 2569): เนื้อหาสาระของ continuity-bible.md และ
character-visual-prompts.md ตรงกับ `docs/` ทุกจุดที่เทียบ (ส่วนสูง/น้ำหนักตัวละครทั้ง 10 คน
มีอยู่ในต้นฉบับดิบจริงอยู่แล้ว ไม่ใช่ข้อมูลที่แต่งขึ้นทีหลัง) — ต่างกันแค่ markdown formatting
และ section ใหม่ที่เพิ่มใน `docs/` เท่านั้น
