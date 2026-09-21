# ชั้น 14 มีรัก | Shorts Video Prompts — ตอนที่ 7 "หูฟังข้างเดียว"

**ใช้กับ:** Google Flow (Ingredients to Video) — ต้องมี Character Ingredient ของ ดิว, นนท์ สร้างไว้แล้วจาก `character-visual-prompts.md` (✅ `@tan_v1` ที่ใช้ใน Scene 6 — ยืนยันแล้วว่ามี turnaround sheet จริง 2 ไฟล์ `references/แทน01-IT.jpeg`/`แทน02-IT.jpeg` — ตรวจภาพจริงแล้ว 21 ก.ย. 2569 ตาม `docs/shorts-prompt-standards.md` ข้อ 3)
**โครงสร้าง:** Hook-First (เปิดด้วยจุดพีค) → Flashback → Build-up → Payoff → ผีเห็นผี → Closing tag
**ความยาวรวมโดยประมาณ:** 56 วินาที (7 คลิป × 8 วิ) — ไม่เกิน 60 วิ ตามที่กำหนด — ต่อกันใน Scenebuilder
**Hook:** ภาพ + text overlay ในคลิปแรกต้องเรียกความสนใจได้ภายใน 3 วินาทีแรก (ดู Scene 1)

**แก้ไขเมื่อ 20 ก.ย. 2569** — ตรวจพบว่าหูฟังของดิว/นนท์เขียนไม่สอดคล้องกันข้าม scene (over-ear ↔
in-ear ↔ shared earbud) และไม่มี blocking ตายตัว โดย Beam/Bank/Mint ร่วมกับ Director Park —
แก้ไขตามมาตรฐานใหม่ใน `docs/shorts-prompt-standards.md` ทุก scene ในไฟล์นี้แล้ว

---

## 📌 Prop State Table — Identity Prop (ล็อกตลอดเรื่อง — ตาม `docs/shorts-prompt-standards.md` ข้อ 1A)

| ตัวละคร | Signature Prop | Spec อ้างอิง | สถานะเริ่มต้นของตอนนี้ |
|---|---|---|---|
| ดิว (`@dew_v1`) | worn **over-ear headphones**, slightly frayed cable | character-visual-prompts.md บรรทัด 631-633 | สวมครบทั้งสองข้าง จนถึง Scene 4 ที่ถอดลงมาคล้องคอ |
| นนท์ (`@non_v1`) | **stem-style wireless in-ear earbuds** with a short protruding stem (AirPods-like silhouette, not a rounded flush-fit bud — ยืนยันจากภาพ `references/นนท์01-Motion Graphic Designer.jpeg` เพิ่ม 21 ก.ย. 2569 หลัง Bank ตรวจพบว่า text spec เดิมไม่ระบุทรง) | character-visual-prompts.md บรรทัด 699-701 (ไม่ระบุทรง) + `references/นนท์01-02-Motion Graphic Designer.jpeg` (ground truth) | สวมครบทั้งสองข้าง จนถึง Scene 4 ที่ถอดข้างขวายื่นให้ดิว |

**หมายเหตุสำคัญ:** ดิวกับนนท์ใส่หูฟังคนละชนิดกันโดยเจตนา (signature prop ที่สื่อบุคลิก/สถานะต่าง
กัน) — ตลอดทั้งตอนนี้ **ห้ามให้ดิวเปลี่ยนไปใส่ in-ear และห้ามให้นนท์เปลี่ยนไปใส่ over-ear** ธีม
"หูฟังข้างเดียว" ทำผ่าน **action การยืม/คล้องคอ** ไม่ใช่การเปลี่ยนชนิด prop ของใครทั้งสิ้น

## 📌 Outfit State Table — Outfit of the Day (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 1B)

**Timeline:** ตอน 7 = วันพฤหัสบดี สัปดาห์ 3 (ค่ำ) ตาม `docs/continuity-bible.md` — ทั้ง 7 scene คือคืน OT
คืนเดียวกันต่อเนื่องกัน ดังนั้น outfit ต้อง**เหมือนกันเป๊ะทุก scene ภายในตอนนี้** (คนละเรื่องกับตอน
อื่นที่เป็นคนละวัน ซึ่งเปลี่ยน outfit ได้/ควรเปลี่ยนเพื่อสื่อว่าเป็นคนละวัน)

| ตัวละคร | Outfit of the Day (ep07) | Spec/ภาพอ้างอิง | เปลี่ยนแปลงภายในตอนนี้หรือไม่ |
|---|---|---|---|
| ดิว (`@dew_v1`) | dark charcoal-grey (#3A3A3D) oversized short-sleeve t-shirt (visibly grey, **not pure black** — subtle grey logo print must stay visible on the chest) with a subtle grey logo print on the chest, grey tailored trousers, white sneakers | character-visual-prompts.md บรรทัด 631-633 + `references/ดิว01-Graphic Designer.jpeg`, `references/ดิว02-Graphic Designer.jpeg` | ไม่เปลี่ยนตลอดตอน (คืนเดียวกันทั้ง 7 scene) |
| นนท์ (`@non_v1`) | olive-green (#5C6B3C) cotton shirt-jacket with a structured collar and a row of front buttons (muted military green, **not brown, not tan, not khaki**) worn open over a light grey t-shirt, dark grey tailored trousers, white sneakers | character-visual-prompts.md บรรทัด 699-701 + `references/นนท์01-Motion Graphic Designer.jpeg`, `references/นนท์02-Motion Graphic Designer.jpeg` | ไม่เปลี่ยนตลอดตอน (คืนเดียวกันทั้ง 7 scene) |

**หมายเหตุสำคัญ:** Google Flow generate แต่ละ scene แยกกัน ไม่มี memory ข้าม prompt — **ทุก scene
ด้านล่างต้องมี outfit description เต็มของตัวละครที่ปรากฏซ้ำทุกครั้ง** (ไม่ใช่แค่ scene แรก) ห้าม
สมมติว่า Flow จะ "จำ" ชุดจาก scene ก่อนหน้าได้เอง — และถ้าตอนต่อไป (เช่น ep08 = คนละวัน) ให้กำหนด
Outfit of the Day ใหม่ ไม่ต้องใช้ชุดนี้ซ้ำ

**⚠️ Color Anchor Lock (พลาดจริง 21 ก.ย. 2569 — ดู `docs/shorts-prompt-standards.md` ข้อ 3B):**
generate Scene 1 ซ้ำ 2 ครั้งด้วย prompt เดิมเป๊ะ ได้สีเสื้อผ้าออกมาไม่ตรงกัน (olive-green (#5C6B3C) ↔ tan,
charcoal-grey (#3A3A3D) ↔ black) เพราะฉากใช้แสงอุ่นจัด ("warm desk-lamp glow") ที่กลืนสีได้ง่าย — **ทุก scene
ที่มีคำอธิบายสีต้องระบุคู่สีที่ห้ามเพี้ยนกำกับด้วย (ตามที่แก้ไว้ในตารางข้างบนแล้ว) และทุก scene ที่ใช้
แสงอุ่น/แสงสลัวต้องเติมคำเตือนกันสีเพี้ยนต่อท้าย Mood** — แก้ไปแล้วทุก scene ในไฟล์นี้ด้านล่าง

## 📌 เวลา/สภาพอากาศของตอนนี้ (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 5A)

**สภาพอากาศ (จาก `docs/continuity-bible.md` — Fictional Weather Table):** ท้องฟ้าแจ่มใส ไม่มีฝน
อากาศค่ำเย็นสบาย ชื้นเล็กน้อยแบบค่ำกรุงเทพฯ — **ใช้ซ้ำคำต่อคำทุก scene** ("clear night sky, no rain,
mild and slightly humid Bangkok evening air")

**เวลาเจาะจงต่อ scene (ทั้ง 7 scene คือคืนเดียวกันต่อเนื่องกัน — OT คืนแรกของดิว-นนท์):**

| Scene | เวลาโดยประมาณ | หมายเหตุ |
|---|---|---|
| 1 (Hook) | ~22:05 น. | ขยายจาก Scene 5 (เกิดหลัง Scene 5 ไปแล้วไม่กี่นาที) |
| 2 (Flashback) | ~20:00 น. | ตาม text overlay "3 ชั่วโมงก่อนหน้า" จาก Scene 1 |
| 3 | ~20:15 น. | ต่อจาก Scene 2 ไม่กี่นาที |
| 4 | ~20:30 น. | ต่อจาก Scene 3 |
| 5 | ~22:00 น. | payoff ที่ Scene 1 ขยายมา |
| 6 | ~22:10 น. | ไม่กี่นาทีหลัง Scene 5 |
| 7 | ~22:15 น. | ดิวตื่นทันทีหลัง Tan เดินผ่านไป |

## 📌 Blocking (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 2)

- **Layout:** โต๊ะทำงานสองตัวหันหน้าเข้าหากันแบบเฉียง (angled facing desks) ห่างกันประมาณ 1 เมตร
  มีเก้าอี้แบบมีล้อเลื่อนได้ทั้งคู่ — ใช้คำนี้ซ้ำทุก scene ห้าม paraphrase เป็น "adjacent"/"beside"
  แบบสลับความหมายไปมา
- **Camera-left / camera-right:** **นนท์อยู่ camera-left, ดิวอยู่ camera-right** ตลอดทั้งตอน
  (คงที่ทุก scene ที่ทั้งคู่ปรากฏร่วมกัน)
- **สัดส่วนตัวละคร (ตาม `docs/shorts-prompt-standards.md` ข้อ 5B):** ดิว 174cm/61kg vs นนท์
  170cm/56kg — ต่างกันแค่ 4cm ใกล้เคียงกัน ไม่ต้องเน้นความต่างของส่วนสูงมากในภาพ (ดูรายละเอียดที่
  `docs/continuity-bible.md` — Character Scale Table)

---

## ⚠️ ตัดสินใจก่อนเริ่ม: บทพูดจริง (native audio) หรือ silent + พากย์ทับ?

มีบทพูดสำคัญ 3 จุด (Scene 3, 6, 7) แนะนำให้ **generate คลิปทดสอบสั้นๆ 1 อันก่อน** ด้วยพรอมต์นี้:

```
Speaker: @non_v1. Line: "หูฟังพี่ดิว... ข้างซ้ายเสียงแผ่วมานานแล้วใช่ไหม".
Delivery: soft, casual, slightly hesitant, natural lip sync. Timing:
close-up shot on his face, quiet office ambience in background.
```

- ถ้าปากตรง เสียงไทยฟังเป็นธรรมชาติ → ใช้บทพูดจริงตามพรอมต์ด้านล่างได้เลย (ตัวเลือก A ในแต่ละ scene)
- ถ้าปาก/สำเนียงเพี้ยน → ใช้เวอร์ชัน silent (ตัวเลือก B) แล้วพากย์เสียงไทยทับตอนตัดต่อ

ทุก scene ที่มีบทพูดด้านล่างมีให้ทั้ง 2 แบบ

---

## 🎬 Scene 1 — HOOK (0:00-0:08) — เปิดด้วยจุดพีค ต้องเรียกความสนใจใน 3 วิแรก

**Ingredients:** `@dew_v1` (expression: sleepy exhausted), `@non_v1` (expression: soft restrained fondness)

**Text overlay ที่ใส่ตอนตัดต่อ (โผล่ตั้งแต่ 0:00-0:03):** *"ไหล่ข้างนึง กลายเป็นหมอน"*

**Composition:** close-up two-shot, eye-level, shallow depth of field — ภาพต้องดึงสายตาทันทีตั้งแต่เฟรมแรก ก่อน text overlay ขึ้นด้วยซ้ำ — Non on camera-left, Dew on camera-right (ตาม Blocking ด้านบน)

**Action:** Dew's head resting fully on Non's shoulder, eyes closed, peaceful; Non frozen completely still, eyes looking down at Dew with a soft restrained smile, one hand hovering motionless just above his own mouse

**Prop state (นี่คือช็อตขยายจาก Scene 5 — เกิดหลัง Scene 4 แล้ว):** Dew's own worn over-ear headphones hanging loose around his neck (ถอดลงมาคล้องคอตั้งแต่ Scene 4); Dew wearing Non's single in-ear earbud in his right ear, thin cable running down to Non's device; Non wearing his matching left in-ear earbud in his own left ear.

**ตัวเลือก A (มีเสียงพื้นหลัง ไม่มีบทพูด):**
```
Subject: @dew_v1, wearing a dark charcoal-grey (#3A3A3D) oversized short-sleeve
t-shirt (visibly grey, not pure black — the subtle grey logo print on
the chest must stay visible) and grey tailored trousers, sitting at his
angled facing desk with the edge of his computer monitor and keyboard
visible at the bottom of frame, asleep with his head resting on
@non_v1's shoulder, Dew's own worn over-ear headphones hanging loose
around his neck, Dew wearing one of Non's in-ear earbuds in his right
ear with a thin cable running to Non's device; @non_v1, wearing an
olive-green (#5C6B3C) cotton shirt-jacket with a structured collar and a row of front buttons (muted military green, not brown, not tan,
not khaki) open over a light grey t-shirt and dark grey trousers,
sitting at his own desk beside Dew with his mouse hand resting near his
keyboard, motionless, his matching left earbud still in his own ear,
mouse hand frozen mid-air.
Composition: close-up two-shot, eye-level, shallow depth of field, Non on
camera-left, Dew on camera-right, the bottom edge of both desks/monitors
just visible in frame beneath them, soft warm desk-lamp light, background
of a dim office softly blurred — completely empty except for the two of
them, no other coworkers visible anywhere in the frame or background.
Action: Dew's breathing slow and even, eyes fully closed, peaceful
expression; Non's eyes fixed gently on Dew's sleeping face, corner of his
mouth lifted in a small restrained smile, not moving a muscle.
Mood: approximately 10:05 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, near-silent office ambience, a single desk lamp's warm glow against
a mostly dark room, quiet intimate tenderness, cinematic muted evening
color grade — the warm lighting must not shift clothing colors: Non's
jacket stays visibly olive-green (#5C6B3C — not brown/tan), Dew's t-shirt stays
visibly charcoal-grey (#3A3A3D — not black).
```

**ตัวเลือก B (silent เต็มรูปแบบ — พากย์/เพลงทับ):**
```
Subject: @dew_v1, wearing a dark charcoal-grey (#3A3A3D) oversized short-sleeve
t-shirt (visibly grey, not pure black — the subtle grey logo print on
the chest must stay visible) and grey tailored trousers, sitting at his
angled facing desk with the edge of his computer monitor and keyboard
visible at the bottom of frame, asleep with his head resting on
@non_v1's shoulder, Dew's own worn over-ear headphones hanging loose
around his neck, Dew wearing one of Non's in-ear earbuds in his right
ear; @non_v1, wearing an olive-green (#5C6B3C) cotton shirt-jacket with a structured collar and a row of front buttons (muted military
green, not brown, not tan, not khaki) open over a light grey t-shirt and
dark grey trousers, sitting at his own desk beside Dew, motionless, his
matching left earbud still in his own ear.
Composition: close-up two-shot, eye-level, shallow depth of field, Non on
camera-left, Dew on camera-right, the bottom edge of both desks/monitors
just visible in frame beneath them.
Action: identical to option A, but no ambient office dialogue needed —
mood carried entirely by a soft instrumental music bed added in editing.
Mood: approximately 10:05 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, warm desk-lamp glow, dark quiet office, tender stillness, cinematic
muted evening color grade — warm lighting must not shift clothing
colors: Non's jacket stays visibly olive-green (#5C6B3C — not brown/tan), Dew's
t-shirt stays visibly charcoal-grey (#3A3A3D — not black).
```

---

## 🎬 Scene 2 — FLASHBACK ESTABLISHING (0:08-0:16)

**Ingredients:** `@dew_v1` (expression: calm focused), `@non_v1` (expression: calm focused)

**Text overlay ที่ใส่ตอนตัดต่อ:** *"3 ชั่วโมงก่อนหน้า — สองทุ่ม"*

**⚠️ Empty Zone Lock (ตัดสินใจโดย Ek, story consultant — ดู `docs/shorts-prompt-standards.md`
ข้อ 2C):** ต้นฉบับ ep07.txt บรรทัด 30 ระบุชัดว่า "สองทุ่มครึ่ง ชั้น 14 เหลือคนไม่กี่คน... ดิวกับนนท์
นั่งอยู่โซน creative" — ไม่มีใครอื่นถูกเอ่ยชื่อว่านั่งทำงานใกล้ๆ เลยตลอดทั้งตอน (คนที่เหลือมีแค่คิม
ซึ่งอยู่คนละห้อง กระจกฝ้าบัง มองไม่เห็นโซน creative) **ห้ามใช้คำกำกวม "mostly empty" — ต้องระบุ
ชัดว่าโซน creative ว่างเปล่าสนิท ไม่มีใครอื่นเลย** เพื่อให้ปมของตอนคือ "ดิวทนง่วงไม่ไหวเพราะรู้สึก
ปลอดภัยพอจะหลับได้" ไม่ใช่ "หลับทั้งที่มีคนมอง" (จะเปลี่ยนโทนเป็นเสี่ยง/บุ่มบ่ามเกินคาแรกเตอร์ดิว)

```
Subject: @dew_v1, wearing a dark charcoal-grey (#3A3A3D) oversized short-sleeve
t-shirt (visibly grey, not pure black) with a subtle grey logo print on
the chest, grey tailored trousers, and white sneakers, and @non_v1,
wearing an olive-green (#5C6B3C) cotton shirt-jacket with a structured collar and a row of front buttons (muted military green, not brown,
not tan, not khaki) open over a light grey t-shirt, dark grey trousers,
and white sneakers, sitting at angled facing desks about 1 meter apart
in the creative zone, which is completely empty except for the two of
them — no other coworkers visible anywhere in the frame or background,
all other desks in this zone empty and dark, each wearing their own
headphones, working normally.
Composition: medium-wide establishing shot, static camera, Non on
camera-left, Dew on camera-right, desk lamps and monitor glow as the main
light sources, all surrounding desks visibly empty and unlit in the
background, no other people anywhere in frame.
Action: Dew typing steadily on a graphic design layout, his worn over-ear
headphones on both ears with the frayed cable visible; Non working on a
motion-graphics timeline on his own screen, his in-ear headphones on both
ears, occasionally glancing over at Dew's monitor without speaking.
Mood: approximately 8:00 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, quiet late-evening office ambience, keyboard clicks, warm desk-lamp
glow against a mostly dark room behind them, the rest of the floor empty
and quiet — everyone else has already left for the night, calm focused
mood — warm lighting must not shift clothing colors: Non's jacket stays
visibly olive-green (#5C6B3C — not brown/tan), Dew's t-shirt stays visibly
charcoal-grey (#3A3A3D — not black).
```

*(Scene นี้ไม่ต้องมี dialogue — เป็นช็อตปูบริบทล้วนๆ)*

---

## 🎬 Scene 3 — THE HEADPHONE QUESTION (0:16-0:24)

**Ingredients:** `@dew_v1` (expression: quietly surprised), `@non_v1` (expression: hesitant but curious)

**Composition:** medium two-shot, eye-level, Non on camera-left, Dew on camera-right, both seated at their angled facing desks (same layout as Scene 2)

**Action:** Non stops typing, turns his head toward Dew; Dew pauses, pulls one **over-ear headphone earcup** off his left ear to listen — right earcup still fully on

**ตัวเลือก A (มีบทพูด):**
```
Subject: @non_v1, wearing an olive-green (#5C6B3C) cotton shirt-jacket with a structured collar and a row of front buttons (muted military
green, not brown, not tan, not khaki) open over a light grey t-shirt and
dark grey trousers, sitting at his angled facing desk with his monitor
and keyboard in frame, turning toward @dew_v1, @dew_v1, wearing a dark
charcoal-grey (#3A3A3D) oversized short-sleeve t-shirt (visibly grey, not pure
black) with a subtle grey logo print and grey tailored trousers, sitting
at his own desk with his monitor and keyboard in frame, pulling one
over-ear headphone earcup off his left ear to listen, right earcup still
on.
Composition: medium two-shot, eye-level, Non on camera-left, Dew on
camera-right, both desks with monitors and keyboards visible in frame,
same angled facing desk layout as Scene 2, soft desk-lamp lighting.
Action: Non leans slightly forward, hesitant but curious expression; Dew
tilts his head, mildly surprised at the question.
Dialogue — Speaker: @non_v1. Line: "หูฟังพี่ดิว... ข้างซ้ายเสียงแผ่วมานาน
แล้วใช่ไหม". Delivery: soft, hesitant, careful not to sound intrusive.
Speaker: @dew_v1. Line: "...สังเกตได้ไง?". Delivery: quietly surprised,
slight smile.
Mood: approximately 8:15 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, quiet late-evening office ambience, warm desk-lamp glow against a
mostly dark room, gentle intimate mood — warm lighting must not shift
clothing colors: Non's jacket stays visibly olive-green (#5C6B3C — not brown/tan),
Dew's t-shirt stays visibly charcoal-grey (#3A3A3D — not black).
```

**ตัวเลือก B (silent — พากย์ทับ):**
```
Subject: @non_v1, wearing an olive-green (#5C6B3C) cotton shirt-jacket with a structured collar and a row of front buttons (muted military
green, not brown, not tan, not khaki) open over a light grey t-shirt and
dark grey trousers, sitting at his desk with his monitor and keyboard in
frame, turning toward @dew_v1, @dew_v1, wearing a dark charcoal-grey (#3A3A3D)
oversized short-sleeve t-shirt (visibly grey, not pure black) and grey
tailored trousers, sitting at his own desk with his monitor and keyboard
in frame, pulling one over-ear headphone earcup off his left ear, right
earcup still on.
Composition: medium two-shot, eye-level, Non on camera-left, Dew on
camera-right, both desks with monitors and keyboards visible in frame.
Action: Non's mouth moves as if asking a hesitant question, eyebrows
slightly raised; Dew's mouth moves in a short surprised reply, head
tilting with a small smile.
Mood: approximately 8:15 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, quiet office ambience only, no audible dialogue, warm desk-lamp
glow against a mostly dark room, gentle intimate mood — warm lighting
must not shift clothing colors: Non's jacket stays visibly olive-green (#5C6B3C)
(not brown/tan), Dew's t-shirt stays visibly charcoal-grey (#3A3A3D — not black).
```

---

## 🎬 Scene 4 — SHARING THE EARBUD (0:24-0:32)

**Ingredients:** `@non_v1` (expression: casual, matter-of-fact), `@dew_v1` (expression: mildly touched, quiet acceptance)

**⚠️ Prop interaction — เขียนตาม Signature Prop Lock (ดู `docs/shorts-prompt-standards.md` ข้อ 1):**
over-ear (ดิว) กับ in-ear (นนท์) เป็นคนละชนิด ถอดแบ่งข้างกันไม่ได้ทางกายภาพ — Scene นี้จึงใช้
action "ยืม + คล้องคอ" แทน: **นนท์ถอด in-ear ข้างขวาของตัวเองยื่นให้ดิวใส่ชั่วคราว** ส่วน **ดิวถอด
over-ear ของตัวเองทั้งอันลงมาคล้องคอ** (ไม่ใช่ถอดข้างเดียวค้างหู) แล้วรับ earbud ของนนท์มาใส่หูขวา
— ยังคง signature prop เดิมของทั้งคู่ไว้ครบ ไม่มีใครเปลี่ยนชนิดหูฟัง แค่ "ยืม" ชั่วคราว

**⚠️ ทรง earbud (เพิ่ม 21 ก.ย. 2569 — ดู `docs/shorts-prompt-standards.md` ข้อ 1A):** in-ear ของ
นนท์เป็น**ทรง stem-style มีก้านยื่นสั้นๆ (คล้าย AirPods ไม่ใช่ทรงกลมเรียบแนบหู)** ตามภาพ
`references/นนท์01-Motion Graphic Designer.jpeg` — สำคัญเฉพาะ Scene นี้เพราะเป็น scene เดียวที่มี
action ถอด/ยื่น/ใส่ ต้องเขียนกำกับให้ Flow generate ทรงเดียวกันตลอดทั้ง action ไม่ใช่แค่ตอนถอด

**Blocking:** ก่อนยื่นของ นนท์ขยับเก้าอี้ (มีล้อเลื่อน) เข้าใกล้ดิวก่อน เพื่อให้ระยะเอื้อมถึงสมเหตุสมผล
(แก้ปัญหาเดิมที่ยื่นข้าม "gap between desks" โดยไม่มี action อธิบายว่าใครขยับ)

```
Subject: @non_v1, wearing an olive-green (#5C6B3C) cotton shirt-jacket with a structured collar and a row of front buttons (muted military
green, not brown, not tan, not khaki) open over a light grey t-shirt and
dark grey trousers, seated at his desk with his monitor and keyboard in
frame, rolling his office chair away from his desk closer to @dew_v1's
desk, then pulling out his own right stem-style wireless in-ear earbud
(short protruding stem, AirPods-like silhouette, not a rounded
flush-fit bud) and holding it out toward Dew; @dew_v1, wearing a dark
charcoal-grey (#3A3A3D) oversized short-sleeve
t-shirt (visibly grey, not pure black) and grey tailored trousers,
seated at his own desk with his monitor and keyboard in frame, lifting
his worn over-ear headphones off his head with both hands and letting
them hang around his neck.
Composition: close-up insert shot on the hand-off, then cutting to a
medium two-shot, Non on camera-left, Dew on camera-right, both desks with
monitors and keyboards visible in frame, as Dew takes the stem-style
earbud and puts it in his own right ear while Non puts his matching
left stem-style earbud back in his own left ear.
Action: Non holds his earbud out casually, as if it's the most normal
thing in the world; Dew looks at it for a beat, lifts his own over-ear
headphones off and lets them rest around his neck (frayed cable still
connected to his own device, now slack), then takes Non's earbud and puts
it in his right ear — their chairs now noticeably closer together,
shoulders nearly touching.
Dialogue — Speaker: @non_v1. Line: "ก็ผมใช้ข้างนึง พี่ดิวใช้ข้างนึง"
Delivery: matter-of-fact, casual, as if stating something obvious. (silent
version: Non's mouth moves saying the line casually while shrugging one
shoulder, no audible dialogue needed if using voiceover dub)
Mood: approximately 8:30 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, warm intimate desk-lamp lighting, quiet late-evening ambience, the
physical distance between them visibly closing, soft tender mood — warm
lighting must not shift clothing colors: Non's jacket stays visibly
olive-green (#5C6B3C — not brown/tan), Dew's t-shirt stays visibly charcoal-grey (#3A3A3D)
(not black).
```

---

## 🎬 Scene 5 — FALLING ASLEEP + THE SAVE (0:32-0:40) — Emotional Payoff

**Ingredients:** `@dew_v1` (expression: sleepy exhausted, transitioning from focused to drifting off), `@non_v1` (expression: soft restrained fondness, quietly protective)

**หมายเหตุ:** นี่คือช็อตที่ขยายความจาก Hook (Scene 1) ให้เห็นว่า "มันเกิดขึ้นได้ยังไง" — **Camera anchor
(แก้ตาม `docs/shorts-prompt-standards.md` ข้อ 2B — เดิมเขียนแค่ "same camera-left/right as Scene 1"
ลอยๆ ไม่พอ ต้องระบุมุม/ระยะ/ความสูงกล้องกำกับด้วย):** ใช้มุมกล้องเดียวกับ Scene 1 (eye-level,
close-up two-shot) แต่ระยะกล้องกว้างกว่าเล็กน้อย (medium two-shot) เพื่อไม่ให้ภาพซ้ำเป๊ะ — Non
camera-left, Dew camera-right เหมือน Scene 1, มุมกล้องตรงหน้าทั้งคู่ในระนาบเดียวกัน ไม่ใช่มุมเฉียง/
มุมข้าง/มุมหลัง

**Prop state (ต่อเนื่องจาก Scene 4):** Dew's own worn over-ear headphones still hanging loose around his neck; Dew still wearing Non's in-ear earbud in his right ear; Non still wearing his matching left earbud.

```
Subject: @dew_v1, wearing a dark charcoal-grey (#3A3A3D) oversized short-sleeve
t-shirt (visibly grey, not pure black) and grey tailored trousers,
sitting at his angled facing desk with his computer monitor and keyboard
in frame in front of him, his rolling office chair beneath him, leaning
back and slowly closing his eyes, head gradually tilting sideways, his
own worn over-ear headphones still hanging loose around his neck, one of
Non's in-ear earbuds still in his right ear; @non_v1, wearing an
olive-green (#5C6B3C) cotton shirt-jacket with a structured collar and a row of front buttons (muted military green, not brown, not tan, not
khaki) open over a light grey t-shirt and dark grey trousers, sitting at
his own angled facing desk with his monitor, keyboard, and mouse in
frame beside him, noticing Dew from the corner of his eye, his matching
left earbud still in his own ear.
Composition: medium two-shot, slightly wider than Scene 1, eye-level,
camera positioned directly in front of both desks (same front angle as
Scene 1, not from behind, not from the side), static camera, Non on
camera-left, Dew on camera-right, both desks with monitors, keyboards,
and desk lamps clearly visible in frame, same angled facing desk layout
as Scene 2-4, no other people present in the creative zone, all
background desks empty and dark.
Action: Dew's head drifts slowly down onto Non's shoulder as his eyes
fully close, breathing evens out; Non stays completely still for a beat,
then carefully reaches his mouse hand over to Dew's keyboard and presses
Ctrl+S to save Dew's open file, then quietly returns to his own work
one-handed, careful not to disturb him.
Mood: approximately 10:00 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, near-silent office ambience, warm desk-lamp glow against a mostly
dark room, the entire creative zone empty and quiet except for the two
of them, tender protective mood, cinematic muted evening color grade,
no dialogue — warm lighting must not shift clothing colors: Non's
jacket stays visibly olive-green (#5C6B3C — not brown/tan), Dew's t-shirt stays
visibly charcoal-grey (#3A3A3D — not black).
```

---

## 🎬 Scene 6 — TAN WITNESSES (0:40-0:48) — ผีเห็นผี Seed

**Ingredients:** `@tan_v1` (expression: understated wistful softness) ✅ **ยืนยันแล้วว่ามี turnaround sheet จริง 2 ไฟล์ (`references/แทน01-IT.jpeg`, `references/แทน02-IT.jpeg`) — ตรวจภาพจริงแล้ว 20 ก.ย. 2569 (Bank + Claude session 21 ก.ย. 2569 เปิดยืนยันซ้ำ) แก้ warning เดิม "ยังไม่ยืนยัน" ที่ล้าสมัยแล้วออก ตาม `docs/shorts-prompt-standards.md` ข้อ 3**

**⚠️ Camera anchor — เขียนตาม Setting/Furniture Lock + Blocking Lock (ดู
`docs/shorts-prompt-standards.md` ข้อ 2 และ 2A):** Scene นี้มีสอง camera subject พร้อมกัน (Tan
เคลื่อนที่เป็น foreground, ดิว-นนท์นิ่งเป็น background) — ต้องระบุมุม/ระยะกล้องของ**ทั้งสองส่วนแยก
กันให้เจาะจง** ไม่ใช่พึ่งคำอ้างอิงลอยๆ ว่า "same position as Scene 5" เพียงอย่างเดียว เพราะ Flow
ไม่มี memory ข้าม prompt คำอ้างอิงแบบนี้ไม่พอให้รักษามุมกล้องจริง (พบปัญหานี้จริงกับ Scene 6 รอบ
generate ที่สอง — ภาพออกมาเป็น close shot จากด้านหลัง/ข้างของดิว-นนท์ ทั้งที่ Scene 5 เป็น medium
two-shot ตรงๆ หน้า)

**⚠️ Empty Zone Lock (ตัดสินใจโดย Ek, story consultant — ดู `docs/shorts-prompt-standards.md`
ข้อ 2C):** จากรอบ generate เดียวกันนี้ พบว่ามีผู้หญิงนั่งทำงานอยู่ในเฟรมโดยไม่เคยปูมาก่อนว่ามีคนอื่น
ในออฟฟิศ — Ek ตรวจ ep07.txt ต้นฉบับยืนยันว่าโซน creative ว่างเปล่าสนิท ไม่มีใครอื่นนอกจากดิว-นนท์
เลยตลอดทั้ง scene (เดิมคำว่า "creative zone aisle" กว้างเกินไป ทำให้ Flow เติมคนเข้ามาเอง) —
แก้เป็นระบุชัดว่า "empty except for Dew and Non" ทุกจุด

```
Subject: @tan_v1 walking through the creative zone aisle at eye-level,
seen strictly from the side, camera perpendicular to his walking
direction, his face and front torso visible in true profile — not from
behind, not a three-quarter back angle — carrying an old laptop, in the
foreground of frame — the entire creative zone empty and quiet except
for Tan walking through it and Dew/Non at their desks, no other
coworkers anywhere in frame; in the background, @dew_v1's desk (Dew
wearing a dark charcoal-grey (#3A3A3D) oversized t-shirt, visibly grey not pure
black, his monitor and keyboard visible) and @non_v1's desk (Non wearing
an olive-green (#5C6B3C) jacket, muted military green, not brown/tan/khaki, his
monitor and keyboard visible) are positioned exactly as in Scene 5:
Non's desk on camera-left, Dew's desk on camera-right, both desks angled
facing each other about 1 meter apart, all other desks in the zone empty
and dark, the background camera positioned directly in front of both
desks, lens axis perpendicular to the line connecting Dew and Non's
faces, at seated eye-level — both of their faces visible from the front,
neither profile nor back visible, same medium two-shot front angle and
same camera height as Scene 5 — not from behind, not from the side, not
closer than Scene 5.
Composition: medium tracking shot from the side, following Tan's walking
pace in the foreground (camera perpendicular to Tan's path, true profile
view of Tan only), camera height and distance to Dew/Non's desks
unchanged from Scene 5's medium two-shot framing (background camera
axis stays front-on to Dew/Non, independent of Tan's side-tracking
camera), Non's desk on camera-left and Dew's desk on camera-right within
that unchanged background framing, both desks with monitors visible
softly out of focus behind Tan, all surrounding desks visibly empty and
unlit, no other people anywhere in frame besides Tan, Dew, and Non.
Action: Tan slows his steps when he notices the two of them — Dew's own
over-ear headphones hanging around his neck, a single thin earbud cable
still connecting Non's device to Dew's right ear, Dew asleep on Non's
shoulder; one of his hands briefly touches the front pocket of his
trousers where a small folded
note is kept, his eyes soften slightly, then he continues walking past
quietly without stopping.
Mood: approximately 10:10 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, dim office lighting, quiet ambient hum, the rest of the floor
empty and dark — everyone else has already gone home, understated
wistful mood, no dialogue, cinematic muted evening color grade — warm/
dim lighting must not shift clothing colors: Non's jacket stays visibly
olive-green (#5C6B3C — not brown/tan), Dew's t-shirt stays visibly charcoal-grey (#3A3A3D)
(not black).
```

---

## 🎬 Scene 7 — WAKING UP + CLOSING TAG (0:48-0:56)

**Ingredients:** `@dew_v1` (expression: sleepy, disoriented, then sincere), `@non_v1` (expression: feigned casualness, small lie)

**Prop state (closing action — คืนของกันตามที่ยืมมา ยืนยันว่า prop สองคนไม่เคยปนกันจริง):**
Dew removes Non's earbud from his own right ear and hands it back; Dew then lifts his own worn
over-ear headphones from around his neck back onto his head.

```
Subject: @dew_v1, wearing a dark charcoal-grey (#3A3A3D) oversized short-sleeve
t-shirt (visibly grey, not pure black) and grey tailored trousers,
sitting at his angled facing desk with his monitor and keyboard in
frame, startling slightly awake, lifting his head off @non_v1's
shoulder; @non_v1, wearing an olive-green (#5C6B3C) cotton shirt-jacket with a structured collar and a row of front buttons (muted military
green, not brown, not tan, not khaki) open over a light grey t-shirt and
dark grey trousers, sitting at his own desk with his monitor and
keyboard in frame, already back to looking at his own screen as if
nothing happened.
Composition: medium two-shot, eye-level, Non on camera-left, Dew on
camera-right, both desks with monitors and keyboards clearly visible in
frame, static camera.
Action: Dew blinks, disoriented, glancing at his own screen and noticing
his file is already saved; Non keeps his eyes on his monitor, feigning
casualness.
Dialogue — Speaker: @dew_v1. Line: "...หลับไปนานไหม?". Delivery: sleepy,
slightly embarrassed. Speaker: @non_v1. Line: "ไม่นาน". Delivery: flat,
too quick, not looking up — a small lie. Then @dew_v1 removes Non's
in-ear earbud from his own right ear and sets it on the desk between
them, then lifts his own worn over-ear headphones from around his neck
back onto his head, saying: "...ขอบคุณ". Delivery: quiet, sincere, small
smile.
Mood: approximately 10:15 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, warm desk-lamp lighting, quiet late-evening ambience, gentle
lingering warmth, cinematic muted evening color grade — warm lighting
must not shift clothing colors: Non's jacket stays visibly olive-green (#5C6B3C)
(not brown/tan), Dew's t-shirt stays visibly charcoal-grey (#3A3A3D — not black).
```

**ตัวเลือก B (silent — พากย์ทับ):**
```
Subject: same as above (dark charcoal-grey (#3A3A3D) t-shirt on Dew — visibly
grey, not pure black; olive-green (#5C6B3C) jacket on Non — muted military green,
not brown/tan/khaki).
Action: Dew's mouth moves asking a sleepy question; Non's mouth moves
with a short flat reply, eyes staying on his screen; Dew removes Non's
earbud from his own ear, sets it down, then puts his own over-ear
headphones back on from around his neck, mouths a quiet thank-you with a
small smile.
Mood: approximately 10:15 PM, clear night sky, no rain, mild and slightly humid Bangkok evening air, no audible dialogue, warm desk-lamp lighting, quiet ambience,
gentle lingering warmth — warm lighting must not shift clothing colors:
Non's jacket stays visibly olive-green (#5C6B3C — not brown/tan), Dew's t-shirt
stays visibly charcoal-grey (#3A3A3D — not black).
```

**Text overlay ปิดท้าย (ใส่ตอนตัดต่อ):** *ชั้น 14 มีรัก | ตอนต่อไป: คิม × ไอซ์ — แค่เห็นคนเหมือนกัน*

---

## ✅ Quality Gate — ผลการตรวจรอบเพิ่มเติม 21 ก.ย. 2569 (Color/Time/Weather/Scale/Logo)

ตรวจซ้ำ 2 รอบโดย Bank (Art Director) + agent สแกนอิสระ พบ 6 จุดพลาดจริง แก้ครบแล้ว (mostly-empty
Scene 1, expression tag ขาดทั้งไฟล์, turnaround sheet Tan ล้าสมัย) — จากนั้นคุณอั้มชี้จุดรั่วเพิ่ม
อีก 4 กลุ่มหลังตรวจ `docs/continuity-bible.md`:

- [x] **Hex Code Lock (ข้อ 3B)** — ทุกจุดที่มีชื่อสี olive-green/charcoal-grey มี hex ต่อท้ายครบ
      100% (ตรวจนับจริง: olive-green 22/22, charcoal-grey 23/23)
- [x] **Time/Weather Anchor Lock (ข้อ 5A)** — ทุก scene ระบุเวลาเจาะจง (20:00 → 22:15 ไล่ตาม
      Hook-First structure) และสภาพอากาศ "clear night sky, no rain, mild and slightly humid
      Bangkok evening air" ซ้ำคำต่อคำครบทุก Mood block (10/10)
- [x] **Character Scale Lock (ข้อ 5B)** — ดิว (174cm) vs นนท์ (170cm) ต่างกันแค่ 4cm ระบุไว้ในหัวข้อ
      Blocking แล้วว่าไม่ต้องเน้นความต่างมาก
- [x] **Brand/Logo Lock (ข้อ 2D)** — ตรวจแล้วไม่มี scene ไหนใน ep07 ที่แสดงป้าย/โลโก้บริษัท PRISM
      ในเฟรม ไม่ต้องแก้ไขเพิ่ม

## 📋 Checklist การผลิต

**ก่อนอื่น — ผ่าน Quality Gate ตาม `docs/shorts-prompt-standards.md` ข้อ 6 ก่อน (prop/blocking/ingredient/แสง/timeline) แล้วค่อยเริ่มขั้นตอนด้านล่าง:**

0. [x] ยืนยันว่ามี turnaround sheet ของ `@tan_v1` (Tan) สร้างไว้จริงแล้ว — ตรวจภาพจริง `references/แทน01-IT.jpeg`, `references/แทน02-IT.jpeg` (21 ก.ย. 2569) พบครบ 6 panel (front/back/side profile/half-body 3/4/close-up face) ตามมาตรฐาน ไม่ต้องปรับ Scene 6 อีก
1. [ ] Generate คลิปทดสอบบทพูดไทย (ด้านบนสุด) ก่อนตัดสินใจ A หรือ B
2. [ ] Generate Scene 1-7 ตามลำดับ (แต่ละคลิป 8 วิ)
3. [ ] เรียงคลิปใน Scenebuilder ตามลำดับ 1→2→3→4→5→6→7
4. [ ] ใส่ text overlay 3 จุด (ต้น Scene 1 ต้องขึ้นภายใน 3 วิแรก, ก่อน Scene 2, ท้าย Scene 7) ตอนตัดต่อ ไม่ต้องใส่ในพรอมต์ Flow
5. [ ] ถ้าเลือก silent version ให้พากย์เสียงไทยทับ Scene 3, 4, 7 ในโปรแกรมตัดต่อ (บทพูดมีให้ครบในพรอมต์ด้านบนแล้ว)
6. [ ] เช็คว่า Scene 1 (hook) เป็น 3 วินาทีแรกที่ดึงสายตาได้จริง — ถ้ารู้สึกภาพนิ่งไป ลองครอปให้ใกล้ยิ่งขึ้นหรือเพิ่ม subtle push-in camera move ตอน generate
7. [ ] เช็คคลิปที่ generate จริงว่าหูฟังของดิว/นนท์ตรงตาม Prop State Table ทุก scene (ดิว = over-ear ตลอด ยกเว้นคล้องคอ Scene 4-7, นนท์ = in-ear ตลอด) — ถ้าเพี้ยนให้ regenerate scene นั้นใหม่ก่อนต่อคลิป
8. [ ] เช็คคลิปที่ generate จริงว่าเห็นโต๊ะทำงาน/จอคอม/คีย์บอร์ดในเฟรมตามที่ prompt ระบุไว้ทุก scene ที่ตัวละครนั่งทำงาน (ไม่ใช่นั่งเก้าอี้ลอยๆ ไม่มี context) — ถ้า Flow ตัด furniture ออกไปเอง ให้เพิ่มคำเจาะจงขึ้น (เช่น "monitor clearly visible directly in front of him") แล้ว regenerate scene นั้นใหม่ก่อนต่อคลิป (พบปัญหานี้จริงกับ Scene 5 รอบ generate แรก — แก้ไปแล้วในไฟล์นี้)
9. [ ] เช็คคลิปที่ generate จริงว่ามุมกล้อง/ระยะกล้องต่อเนื่องกับ scene ก่อนหน้าจริง โดยเฉพาะ Scene 6 ที่ต้องคงมุมกล้องเดียวกับ Scene 5 (ไม่ใช่ close จากด้านหลัง/ข้าง) — และเช็คว่าไม่มีคนอื่นหลุดเข้ามาในเฟรมของโซน creative เลย (ต้องว่างเปล่าสนิทมีแค่ดิว/นนท์/แทนตามลำดับ scene) — ถ้าเพี้ยนให้เพิ่มคำเจาะจงขึ้นแล้ว regenerate scene นั้นใหม่ก่อนต่อคลิป (พบปัญหานี้จริงกับ Scene 6 รอบ generate ที่สอง — แก้ไปแล้วในไฟล์นี้ ทั้งเรื่องกล้องและเรื่องมีคนอื่นในเฟรม)
10. [ ] Export เป็น 9:16 ความยาวรวม ~56 วินาที พร้อมโพสต์

---

## 🔁 ใช้ Template นี้กับตอนอื่น

โครงสร้างนี้ (Hook-First → Flashback → Build-up → Payoff → ผีเห็นผี → Closing tag) ใช้ซ้ำได้กับทุกตอนที่มี "จุดพีค" ชัดเจน — ถ้าต้องการให้ทำ Shorts prompt แบบนี้ให้ตอนอื่นต่อ (เช่น ep06 "ดูแลตัวเองด้วย" หรือ ep08 "แค่เห็นคนเหมือนกัน") บอกเลขตอนมาได้เลยครับ
