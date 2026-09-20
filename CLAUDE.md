# คำสั่งสำหรับ Claude Code ในโปรเจกต์นี้

## ภาพรวมโครงการ

โปรเจกต์ short-form video (TikTok shorts) เพื่อ **personal branding ของคุณอั้ม** — แยกขาดจาก
แบรนด์ "อู่โปร" (parts-inventory) โดยสิ้นเชิง ไม่ผูกโลโก้/ชื่อบริษัทกับคอนเทนต์นี้เป็นทางการ

**ทิศทางที่เคาะไว้แล้ว (20 ก.ย. 2569)** — ปรึกษา Bodint (Business Director) + Mayuree
(Marketing Lead) ของ parts-inventory แล้ว คุณอั้มยืนยันทิศทาง:

> แยกแบรนด์ 100% ไม่ผูกโลโก้อู่โปร **แต่ narrative (ตัวตนที่นำเสนอ) ต้องมีเจ้าภาพเดียวกับ
> personal branding series ที่ Mayuree ดูแลอยู่แล้ว** (ซีรีส์ U-PRO Build Journal ใน
> parts-inventory) — ไม่แยกคนตรวจตัวตน กันไม่ให้เล่าเรื่องเป็นคนละคนกันระหว่างสองช่องทาง

เหตุผลเชิงธุรกิจ (Bodint): ลูกค้า B2B อู่ขนาดเล็กตัดสินใจซื้อจาก "ความน่าเชื่อถือของระบบ" ไม่ใช่
"ความบันเทิงของ founder" — โทน TikTok แบบ short-form เสี่ยงขัดกับ trust signal ที่อู่เล็กต้องการ
ก่อนฝากข้อมูลสต็อก/บัญชีทั้งร้าน จึงต้องแยกแบรนด์ชัดเจน แต่ไม่ตัดขาดตัวตนออกจากกันเลย เพราะจะทำให้
key message เรื่อง founder ไม่สอดคล้องกัน

## Persona ที่เกี่ยวข้อง — อ้างอิงจาก `~/.claude/agents/` เท่านั้น ห้าม copy

**🔴 กติกาบังคับ: ห้าม copy เนื้อหา persona definition เข้า repo นี้เด็ดขาด**

**เหตุที่ต้องมีกติกานี้ (พลาดจริง พบ 20 ก.ย. 2569)** — repo แยกอีกอัน
(`~/ugit/ammonium-ai-agents`) เคย copy persona definition ไฟล์มาเก็บเองทั้งชุด (16 ไฟล์)
ตรวจแล้วพบว่า**ทุกไฟล์เพี้ยนจากต้นฉบับหมด** (diff 18-78 บรรทัดต่อไฟล์ — `mayuree-marketing-lead.md`
ขาดกติกา 3 ก.ย. 2569 เรื่อง Build Journal ต้องผ่านธารินก่อน Bodint ทั้งหมด, ขาด
`_reference/SHARED_PROTOCOL.md` ทั้งเรื่อง) เพราะไม่มีใคร sync กลับตอนต้นฉบับอัปเดต — แก้แล้วด้วย
การลบไฟล์สำเนาทิ้งทั้งหมด แทนที่ด้วย symlink ชี้กลับ `~/.claude/agents/` ตรงๆ

⇒ Persona ทุกตัว (Chiwa, Mayuree, Bodint, Tharin, Saran ฯลฯ) เป็นไฟล์ระดับ **user**
(`~/.claude/agents/*.md`) ไม่ผูกกับ repo ไหนโดยเฉพาะอยู่แล้วในทางเทคนิค — เปิด session ทำงานใน
repo นี้แล้วเรียกผ่าน `Agent` tool ได้ทันทีโดยไม่ต้องตั้งอะไรเพิ่ม ไม่ต้องมีไฟล์ agent ของตัวเองใน
repo นี้เลย

**ข้อควรระวังตอนเรียก:** Chiwa/Mayuree/Bodint **ไม่มี**หัวข้อ "adapt to whichever repo you're
called in" ในตัว definition ของตัวเอง (ต่างจาก Preecha ที่มี) — เพราะถูกเขียนตอนที่มีแค่ repo
เดียวคือ parts-inventory ในหัวคนเขียน ⇒ **ทุกครั้งที่เรียกจาก repo นี้ ต้องให้บริบทงาน/repo ที่
ชัดเจนในคำสั่งเอง** (บอกว่านี่คือโปรเจกต์ personal branding แยกจากอู่โปร) ไม่ปล่อยให้เขาเดาบริบทเอง
เพราะ default ของเขายังอิงกับข้อมูล parts-inventory (เช่น `docs/PRICING_MODEL.md`,
`docs/architecture.md` ที่เป็นไฟล์ของ parts-inventory เท่านั้น ไม่มีอยู่ในนี้)

**อ้างอิงรายชื่อ+รายละเอียด persona เต็ม** → `~/ugit/parts-inventory/docs/PERSONA_PANEL.md`
(ไม่ copy เนื้อหามาไว้ในนี้ ด้วยเหตุผลเดียวกับข้างบน — ไฟล์ที่แช่แข็งจะเน่าทันทีที่ต้นฉบับอัปเดต)

## กติกาเชื่อมงานกับทีม Mayuree (ทีม Marketing/Content 8 persona)

**ส่ง request ผ่าน Mayuree จุดเดียว** — ไม่เรียก persona ลูกทีม (อารีย์/พิมพ์ใจ/อาทิตย์/ปิ่นแก้ว/
กันตะ/ฟ้าใส/ปายฝัน/กิ๊บเก๋) ตรงๆ เอง เหตุผล: ถ้าไม่ผ่านเธอ เธอจะมองไม่เห็นภาพรวมว่าทีมโดนดึงไปกี่ทาง
พร้อมกัน เสี่ยง overload

**Request form สั้น 4 ช่อง** เวลาขอยืมทีม:
1. Persona ที่ต้องการ + ปริมาณงานต่อสัปดาห์
2. บรีฟย่อ (สั้นๆ ว่าต้องการอะไร)
3. ผู้อนุมัติฝั่ง TikTok/repo นี้ (คุณอั้มเอง)
4. ยืนยันผ่านด่านตรวจตามหัวข้อถัดไป

**สถานะทีม 8 persona ณ วันที่ตั้ง repo นี้ (20 ก.ย. 2569 — เช็คสถานะสดกับ Mayuree ก่อนใช้จริง
เพราะอาจเปลี่ยนได้):**

| Persona | สถานะกับงาน TikTok |
|---|---|
| อารีย์ (Market Analyst), ปายฝัน (Idea Validator), กิ๊บเก๋ (QA) | ✅ ใช้ได้เลย overhead ต่ำ |
| พิมพ์ใจ (Copywriter) | ⚠️ ต้องกำหนด scope/quota ก่อน — สคริปต์สั้น TikTok คนละสไตล์จาก AIDA/PAS ยาวที่ทำอยู่ |
| อาทิตย์ (Visual Creator) | ⚠️ ต้องเช็ค scope ก่อน — เดิมทำภาพนิ่ง ไม่ใช่ตัดต่อวิดีโอ |
| ปิ่นแก้ว, กันตะ, ฟ้าใส | 🔴 ห้ามแตะเด็ดขาด — ปิดใช้งานอยู่ รอ Saran ตรวจ PDPA/human-in-the-loop ก่อน |

## ด่านตรวจเนื้อหาก่อนเผยแพร่

**ลำดับบังคับ: ธาริน (ตรวจภาษา) → Bodint (ตรวจเนื้อหา/ไม่ขัดแย้งกับ narrative เดิม) → คุณอั้ม
(ตัดสินใจสุดท้าย)**

- **คุณอั้มเป็นผู้ตัดสินใจสุดท้ายเรื่อง content ของ repo นี้เต็มที่** — ไม่ต้องรอ Mayuree/Bodint
  อนุมัติเป็น authority เพราะนี่คือ personal branding ใช้เวลา/ทรัพยากรส่วนตัว ไม่ใช่งบทีมอู่โปร
- **แต่มี guardrail บังคับ sync 2 จุด (ไม่ใช่ authority แต่ต้องแจ้ง/ขอก่อน):**
  - คลิปที่พูดถึงอู่โปรตรงๆ (ราคา, feature, อ้างชื่อบริษัท) → **แจ้ง Mayuree ล่วงหน้า** เพื่อ align
    messaging (ไม่ใช่ขออนุมัติ แค่แจ้งให้ทีมรู้)
  - คลิปที่กระทบ partnership/ราคาที่ยังไม่ประกาศ → **ต้องผ่าน Bodint ก่อน** (เข้าเงื่อนไข 🔴E
    ของ Bodint ตามที่นิยามไว้ใน `bodint-business-director.md` อยู่แล้ว)
- ตรวจสคริปต์**ก่อนถ่าย** ไม่ใช่ตรวจคลิปที่ตัดต่อเสร็จแล้ว — แก้ทีหลังแพงกว่า (บทเรียนจาก Mayuree)

## โครงสร้างโฟลเดอร์

```
amm-bl-the-series/
├── CLAUDE.md   ← ไฟล์นี้
├── docs/       ← มติ/บทเรียนเฉพาะ repo นี้ (ถ้ามี) — ไม่ copy PERSONA_PANEL.md มาไว้ที่นี่
├── scripts/    ← automation (เช่น export/upload TikTok API) — ยังไม่มีตอนตั้ง repo
└── content/    ← สคริปต์/storyboard/raw footage metadata
                   (ไฟล์วิดีโอจริงพิจารณา external storage แยก ไม่ commit เข้า git
                   เพราะไฟล์ใหญ่เกินจะเก็บใน git repo ปกติ — ยังไม่ได้ตัดสินใจว่าใช้ที่ไหน)
```

## สิ่งที่ไม่ต้องทำ (กันสับสนกับ parts-inventory)

- ไม่ต้อง copy กฎ `npm run build`, RLS, คอมเมนต์ภาษาไทยบังคับ, migration idempotent จาก
  parts-inventory มาใช้ที่นี่ — ไม่เกี่ยวกับงาน content/video เลย ถ้าจะมีกติกาเฉพาะ repo นี้เอง
  ให้เพิ่มทีหลังตามบทเรียนจริงที่เกิดขึ้น ไม่ใช่เดาล่วงหน้า
- ไม่มี orchestrator/fleet dispatch แบบ parts-inventory (`docs/PARALLEL_AGENTS.md` +
  `scripts/orchestrator/orchestrator`) — repo นี้ไม่มีกลไกนั้น งานที่ต้องมอบหมายให้ persona
  ใช้ `Agent` tool เรียกตรงๆ ในเซสชัน ไม่ใช่ผ่าน fleet
