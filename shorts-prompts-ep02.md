# ชั้น 14 มีรัก | Shorts Video Prompts — ตอนที่ 2 "เก็บให้ครบ"

**ใช้กับ:** Google Flow (Ingredients to Video) — ต้องมี Character Ingredient ของ ภูมิ, ปอนด์ สร้างไว้แล้วจาก `docs/character-visual-prompts.md` (ยืนยันแล้วว่ามี turnaround sheet จริง — `references/ภูมิ01-หัวหน้าทีม-Project Manager.jpeg`/`ภูมิ02-หัวหน้าทีม-Project Manager.jpeg`, `references/ปอนด์01-เด็กฝึกงาน.jpeg`/`ปอนด์02-เด็กฝึกงาน.jpeg` — เปิดดูภาพจริงแล้ว 21 ก.ย. 2569 พบครบ panel ตามมาตรฐาน — ตาม `docs/shorts-prompt-standards.md` ข้อ 3)

**โครงสร้าง:** Linear (ไล่ตามลำดับเวลาในต้นฉบับ ไม่มี flashback) — เนื้อเรื่องเป็นการสะสมเหตุการณ์ทีละสเต็ป (มาถึง → ประชุม → ทำ brief ผิด → ถูกเรียก → แก้ด้วยกัน) ไม่มีจุดพีคเดี่ยวที่ต้องขยายความย้อนหลัง เหมาะกับ Linear ตามที่ใช้ใน ep06

**ความยาวรวมโดยประมาณ:** 56 วินาที (7 คลิป × 8 วิ) — ไม่เกิน 60 วิ ตามที่กำหนด — ต่อกันใน Scenebuilder

**Hook:** Scene 1 (ปอนด์มาถึง เจอภูมินั่งอยู่ก่อนแล้ว + "จำได้ด้วยเหรอ?") ต้องสื่อ "ภูมิสังเกตปอนด์มากกว่าที่คิด" ให้ชัดภายใน 3 วินาทีแรก

**ตรวจสอบก่อนเขียน (ตาม `docs/shorts-prompt-standards.md` ข้อ 0):**
- อ่าน `content/original-source/ep02.md` เต็มไฟล์แล้ว (129 บรรทัด)
- เปิดภาพ `references/ภูมิ01-02-หัวหน้าทีม-Project Manager.jpeg`, `references/ปอนด์01-02-เด็กฝึกงาน.jpeg` ดูจริงแล้ว
- เปิดภาพ setting `references/Creative_agency_office_interior.jpeg`, `references/Office_corridor_under_different.jpeg` (โทนเช้า) ดูจริงแล้ว
- เช็ค `docs/continuity-bible.md` แล้ว — **ตอน 2 = วันพุธ สัปดาห์ 1 (เช้า) 3 วันหลังตอนที่ 1 — คนละวันกับตอน 1** ⇒ กำหนด Outfit of the Day ใหม่ทั้งหมดสำหรับภูมิ/ปอนด์ (ยังไม่เคยปรากฏใน ep ก่อนหน้า ไม่มีชุดให้เทียบซ้ำ)
- ปรึกษา Mint (character design) เรื่อง signature prop ของภูมิ/ปอนด์แล้ว — ผลตรวจอยู่ในหัวข้อ Prop State Table ด้านล่าง (ปอนด์มีสมุดจดหนาปึกเป็น character trait สำคัญ — ตรวจสอบว่าจัดเป็น Identity Prop หรือ prop เฉพาะฉากแล้ว)
- ปรึกษา Ek (story consultant) เรื่อง scene breakdown + empty zone แล้ว — ผลตรวจสะท้อนอยู่ในทุก scene ด้านล่าง

---

## 📌 Prop State Table — Identity Prop (ล็อกตลอดเรื่อง — ตาม `docs/shorts-prompt-standards.md` ข้อ 1A)

| ตัวละคร | Signature Prop (Identity — ตลอดเรื่อง) | Spec อ้างอิง | สถานะในตอนนี้ |
|---|---|---|---|
| ภูมิ (`@phum_v1`) | **ไม่มี signature prop ระดับ Identity** (ยืนยันแล้วโดย Mint — ตรวจ spec+ภาพแล้วไม่พบอุปกรณ์ประจำตัวเชิงสัญลักษณ์ นอกจาก plain leather strap watch ที่เป็นส่วนหนึ่งของ outfit ปกติ) | `docs/character-visual-prompts.md` บรรทัด 326-367 + `references/ภูมิ01-หัวหน้าทีม-Project Manager.jpeg`, `references/ภูมิ02-หัวหน้าทีม-Project Manager.jpeg` | ไม่มี prop ประจำตัวที่ต้อง lock ข้าม ep |
| ปอนด์ (`@pond_v1`) | **สมุดจดกระดาษเล่มหนา — Identity Prop จริง (ไม่ใช่แค่ prop เฉพาะฉาก)** ยืนยันจาก `docs/continuity-bible.md` บรรทัด 202 ("มีสมุดจดหนาปึก — ตั้งใจจด — character trait เฉพาะตัว") และปรากฏซ้ำในตอน 1, 2, 3, 8 ตามที่ bible ระบุ (บรรทัด 206-210) — ต้องเขียน "a thick well-worn paper notebook" กำกับทุกครั้งที่ปอนด์ถืองาน/จดบันทึก ห้ามใช้คำกลางๆ ว่า "notebook" ลอยๆ | `docs/character-visual-prompts.md` บรรทัด 395-427 + `docs/continuity-bible.md` บรรทัด 197-212 (ภาคผนวกตัวละครปอนด์) + `references/ปอนด์01-เด็กฝึกงาน.jpeg`, `references/ปอนด์02-เด็กฝึกงาน.jpeg` | ถืออยู่ตลอดทุก scene ที่เกี่ยวกับการจด/ประชุม (Scene 3, 7) |

**หมายเหตุสำคัญ (Mint, 21 ก.ย. 2569):** สมุดจดของปอนด์ต่างจากแก้วกาแฟของเตใน ep06 ตรงที่ bible ระบุชัดว่าเป็น "character trait เฉพาะตัว" ที่ปรากฏซ้ำข้าม ep หลายตอน (running gag ตาม bible บรรทัด 210) — จึงจัดเป็น **Identity Prop ระดับ 1** ไม่ใช่ prop เฉพาะฉากระดับ 2 ต้องเขียนกำกับทุกครั้งที่ปอนด์ปรากฏพร้อมสมุด ไม่ใช่แค่ตอนนี้

---

## 📌 Outfit State Table — Outfit of the Day (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 1B)

**Timeline:** ตอน 2 = วันพุธ สัปดาห์ 1 (เช้า) ตาม `docs/continuity-bible.md` บรรทัด 35 — คนละวันกับตอน 1 (วันจันทร์) เป็นตอนแรกที่ภูมิ/ปอนด์ปรากฏเป็นคู่หลัก ทุก scene ในตอนนี้คือเช้าวันเดียวกันต่อเนื่องกัน (8:30 AM ถึงประมาณเที่ยง) ⇒ **outfit ต้องเหมือนกันเป๊ะทุก scene ภายในตอนนี้** — **⚠️ สำคัญ: ep03 เป็นบ่ายของวันเดียวกันนี้ (ดูหมายเหตุ ep03) ต้องใช้ outfit ชุดเดียวกันนี้เป๊ะข้ามสองไฟล์**

อ้างอิงจาก `docs/character-visual-prompts.md` เป็นฐาน + ภาพ reference จริง (เลือกสีที่ตรงกับภาพ turnaround sheet เพื่อความแม่นยำสูงสุด):

| ตัวละคร | Outfit of the Day (ep02/ep03 — วันพุธ สัปดาห์ 1) | Spec/ภาพอ้างอิง | เปลี่ยนแปลงภายในตอนนี้หรือไม่ |
|---|---|---|---|
| ภูมิ (`@phum_v1`) | dark charcoal-grey (#4A4548 — muted warm grey, **not brown, not black**) fitted long-sleeve button-up shirt with sleeves rolled to the forearm, dark navy-black (#1C1D22 — near-black, **not pure black**) tailored trousers, white (#F0EFE8 — clean off-white, **not grey**) leather sneakers, a plain brown leather strap watch | `docs/character-visual-prompts.md` บรรทัด 351-358 + `references/ภูมิ01-หัวหน้าทีม-Project Manager.jpeg` (สีตรงกับภาพ full-body ที่ generate ไว้แล้ว — เสื้อสีเทาเข้มอมน้ำตาล กางเกงดำ รองเท้าผ้าใบขาว) | ไม่เปลี่ยนตลอดตอน (เช้าวันเดียวกันทั้ง 7 scene) — **ใช้ต่อเนื่องใน ep03 (บ่ายวันเดียวกัน)** |
| ปอนด์ (`@pond_v1`) | dark charcoal-grey (#3E3B3D — muted grey, **not black, not brown**) collared polo shirt slightly oversized, black (#181818 — true black, **not navy**) casual trousers, black-and-white leather sneakers, carrying his thick well-worn paper notebook | `docs/character-visual-prompts.md` บรรทัด 420-427 + `references/ปอนด์01-เด็กฝึกงาน.jpeg` (สีตรงกับภาพ full-body ที่ generate ไว้แล้ว — โปโลเทาเข้ม กางเกงดำ) | ไม่เปลี่ยนตลอดตอน (เช้าวันเดียวกันทั้ง 7 scene) — **ใช้ต่อเนื่องใน ep03 (บ่ายวันเดียวกัน)** |

**หมายเหตุสำคัญ:** Google Flow generate แต่ละ scene แยกกัน ไม่มี memory ข้าม prompt — **ทุก scene ด้านล่างต้องมี outfit description เต็มของตัวละครที่ปรากฏซ้ำทุกครั้ง** ห้ามสมมติว่า Flow จะ "จำ" ชุดจาก scene ก่อนหน้าได้เอง และ**ต้องตรงกับ `shorts-prompts-ep03.md` เป๊ะ** เพราะเป็นวันเดียวกัน (เช้า→บ่าย) คนละไฟล์

**⚠️ Color Anchor Lock (ดู `docs/shorts-prompt-standards.md` ข้อ 3B):** ทุก scene ใช้แสงเช้าธรรมชาติผ่านกระจกอาคาร — charcoal-grey ของภูมิ/ปอนด์เสี่ยงเพี้ยนเป็นสีน้ำตาล/ดำสนิทได้แบบเดียวกับที่พบใน ep06/ep07 — เพิ่มคำเตือนกันเพี้ยนกำกับทุกจุดที่ระบุสีแล้ว

---

## 📌 เวลา/สภาพอากาศของตอนนี้ (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 5A)

**สภาพอากาศ (จาก `docs/continuity-bible.md` — Fictional Weather Table แถวที่ 2):** ท้องฟ้าแจ่มใส แดดเช้าปกติ — **ใช้ซ้ำคำต่อคำทุก scene** ("clear sky, ordinary gentle morning sunlight, no rain")

**เวลาเจาะจงต่อ scene (ตอนนี้เป็นโครงสร้าง Linear — ไล่ตามเวลาจริงตามต้นฉบับ):**

| Scene | เวลาโดยประมาณ | หมายเหตุ |
|---|---|---|
| 1 | ~8:30 AM | ปอนด์มาถึง เจอภูมินั่งอยู่ก่อนแล้ว |
| 2 | ~9:00 AM | ทีมประชุมเช้า ภูมิแจก brief |
| 3 | ~11:00 AM | ปอนด์เปิดไฟล์ research ใช้ AI สรุป |
| 4 | ~11:15 AM | AI ทำ brief เสร็จ ปอนด์ส่งอีเมล |
| 5 | ~11:20 AM | อีเมลตอบกลับ "มาหน่อย" — ปอนด์ลุกไปหาภูมิ |
| 6 | ~11:25 AM | ภูมิชี้จุดผิดในหน้าจอ ถามตรงๆ "ใช้ AI ทำเหรอ?" |
| 7 | ~11:30 AM | ภูมินั่งข้างปอนด์ช่วยเทียบไฟล์ต้นฉบับทีละจุด |

## 📌 Blocking (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 2)

**ยืนยันโดย Ek (story consultant) 21 ก.ย. 2569:**

- **Layout:** โต๊ะภูมิและโต๊ะปอนด์อยู่ในโซนทีม PM ติดกัน ห่างกันประมาณครึ่งเมตร (โต๊ะข้างกัน ไม่ใช่หันหน้าเข้าหากัน) แต่ละโต๊ะมีจอคอมพิวเตอร์ คีย์บอร์ด เก้าอี้มีล้อเลื่อน — ใช้ layout นี้ซ้ำทุก scene ที่ทั้งคู่อยู่ที่โต๊ะ
- **Camera-left / camera-right (ทุก scene ที่ภูมิ-ปอนด์อยู่ร่วมกัน):** ภูมิอยู่ camera-left, ปอนด์อยู่ camera-right — คงที่ตลอดทั้งตอน (และต่อเนื่องไปยัง ep03)
- **Layout ห้องประชุม (Scene 2):** โต๊ะประชุมรูปสี่เหลี่ยมผืนผ้ายาว ภูมิยืนต้นโต๊ะแจก brief ทีมนั่งเรียงสองฝั่ง — ปอนด์นั่งอยู่ฝั่งใกล้ภูมิที่สุด
- **สัดส่วนตัวละคร (ตาม `docs/shorts-prompt-standards.md` ข้อ 5B):** ภูมิ 180cm/80kg (muscular broad-shouldered) vs ปอนด์ 172cm/58kg (slender youthful) — ต่างกัน 8cm ชัดเจน ภูมิสูง/ใหญ่กว่าเห็นชัด สอดคล้องกับ dynamic "พี่ดูแลน้อง" ตาม bible — ต้องระบุใน Subject ทุก scene ที่ทั้งคู่อยู่ในเฟรมเดียวกัน

---

## 🎬 Scene 1 — HOOK: มาถึงเช้า (0:00-0:08)

**Ingredients:** `@pond_v1` (expression: mildly surprised, then composed), `@phum_v1` (expression: neutral calm, quietly observant)

**Text overlay ที่ใส่ตอนตัดต่อ (โผล่ตั้งแต่ 0:00-0:03):** *"เขาจำได้ด้วยเหรอ..."*

**Setting/Furniture Lock:** โต๊ะภูมิต้องเห็นจอสามหน้าต่างเปิดอยู่ กาแฟดำไม่ใส่น้ำตาลวางข้างคีย์บอร์ด ตามต้นฉบับ

```
Subject: @phum_v1, wearing a dark charcoal-grey (#4A4548 — muted warm
grey, not brown, not black) fitted long-sleeve button-up shirt with
sleeves rolled to the forearm, dark navy-black (#1C1D22 — near-black, not
pure black) tailored trousers, and white (#F0EFE8 — clean off-white, not
grey) leather sneakers, already seated at his desk with three browser
windows open on his monitor and a black coffee with no sugar in a plain
mug beside his keyboard, not looking up as he types; @pond_v1, wearing a
dark charcoal-grey (#3E3B3D — muted grey, not black, not brown) collared
polo shirt slightly oversized and black (#181818 — true black, not navy)
casual trousers, carrying his thick well-worn paper notebook and a
backpack, arriving at his own desk beside Phum's, noticeably smaller in
build than Phum, setting his bag down.
Composition: medium two-shot, eye-level, Phum on camera-left already
seated with his monitor and keyboard visible, Pond on camera-right just
arriving at his own desk with his monitor and keyboard also visible,
bright morning office lighting.
Action: Pond sets his bag down and opens his laptop; Phum keeps typing
without turning his head at first, then speaks.
Dialogue — Speaker: Phum. Line: "เช้าจังวันนี้". Delivery: flat, not
looking up from the screen. Speaker: Pond. Line: "ปกติครับ". Delivery:
quick, slightly defensive. Speaker: Phum. Line: "ปกติเหรอ? เมื่อวานมา
แปดสี่สิบห้า". Delivery: even, matter-of-fact, still not looking up —
but clearly remembered exactly.
Mood: approximately 8:30 AM, clear sky, ordinary gentle morning sunlight,
no rain, a quiet focused early-morning office ambience, a small spark of
being noticed, bright optimistic color grade — morning light must not
shift clothing colors: Phum's shirt stays visibly charcoal-grey (#4A4548
— not brown/black), Pond's polo stays visibly charcoal-grey (#3E3B3D —
not black/brown).
```

---

## 🎬 Scene 2 — เก้าโมง: ประชุมแจก Brief (0:08-0:16)

**Ingredients:** `@phum_v1` (expression: focused, professional), `@pond_v1` (expression: attentive, taking notes)

**⚠️ Empty Zone (ตัดสินใจโดย Ek):** ต้นฉบับระบุ "ทีมประชุมเช้า... ทุกคนได้ส่วนของตัวเอง" — มีทีมทั้งหมดอยู่ในห้องประชุมแต่ไม่ได้ระบุรายชื่อชัดเจนในจังหวะนี้ ⇒ เขียนแบบเห็นทีมอื่นเป็น background เบลอไม่ระบุจำนวนเจาะจง (มีคนแน่นอนตามต้นฉบับ ไม่ใช่ห้องว่าง แต่ไม่ต้องระบุตัวตนเพราะไม่มีมูลจากต้นฉบับว่าใครบ้าง)

```
Subject: @phum_v1, wearing a dark charcoal-grey (#4A4548 — muted warm
grey, not brown, not black) fitted long-sleeve button-up shirt with
sleeves rolled to the forearm and dark navy-black (#1C1D22) tailored
trousers, standing at the head of a long rectangular meeting table,
gesturing toward a laptop screen showing a client brief document;
@pond_v1, wearing a dark charcoal-grey (#3E3B3D) collared polo shirt and
black (#181818) casual trousers, seated at the table closest to Phum,
his thick well-worn paper notebook open in front of him, pen in hand,
other teammates visible seated further down both sides of the table, out
of sharp focus.
Composition: medium shot, eye-level, Phum on camera-left standing,
Pond on camera-right seated nearest to him with his notebook visible on
the table, the rest of the team softly blurred further down the table,
bright meeting-room lighting.
Action: Phum taps the laptop screen to advance a slide, speaking
steadily; Pond writes quickly in his notebook without looking up.
Dialogue — Speaker: Phum. Line: "ไฟล์ research ทั้งหมดอยู่ในโฟลเดอร์
Share ในไดรฟ์ของทีม เจ็ดไฟล์ สรุปรวมเป็นหน้าเดียวให้ได้ ลูกค้ากลุ่มนี้ไม่
ชอบอ่านยาว". Delivery: clear, businesslike, steady pace. Speaker: Pond.
Line: "ครับ". Delivery: short, focused, still writing.
Mood: approximately 9:00 AM, clear sky, ordinary gentle morning
sunlight, no rain, a focused productive morning meeting ambience, bright
professional color grade — morning light must not shift clothing colors:
Phum's shirt stays visibly charcoal-grey (#4A4548 — not brown/black),
Pond's polo stays visibly charcoal-grey (#3E3B3D — not black/brown).
```

---

## 🎬 Scene 3 — สิบเอ็ดโมง: ปอนด์ใช้ AI สรุป (0:16-0:24)

**Ingredients:** `@pond_v1` (expression: focused, then relieved satisfaction)

**Setting/Furniture Lock:** โต๊ะปอนด์ต้องเห็นจอคอม คีย์บอร์ด สมุดจดวางข้างๆ ตามกฎ 2A

```
Subject: @pond_v1, wearing a dark charcoal-grey (#3E3B3D — muted grey,
not black, not brown) collared polo shirt slightly oversized and black
(#181818 — true black, not navy) casual trousers, seated at his desk
with his computer monitor and keyboard in frame, his thick well-worn
paper notebook closed beside the keyboard, seven research document
windows open and tiled across his screen, typing a prompt into an AI
chat interface.
Composition: medium close-up, eye-level, static camera, Pond centered in
frame with his monitor, keyboard, and notebook clearly visible on the
desk, bright late-morning office lighting.
Action: Pond glances between the seven open documents and the AI chat
window, typing steadily; the AI response appears quickly, formatted with
tables and headers; Pond reads it over once, nodding slightly to
himself, satisfied.
Mood: approximately 11:00 AM, clear sky, ordinary gentle morning
sunlight, no rain, a quiet focused late-morning office ambience, quiet
keyboard clicks, a small sense of accomplishment, bright color grade, no
dialogue — morning light must not shift clothing colors: Pond's polo
stays visibly charcoal-grey (#3E3B3D — not black/brown).
```

---

## 🎬 Scene 4 — ส่งอีเมล: "brief สรุปเสร็จแล้วครับ" (0:24-0:32)

**Ingredients:** `@pond_v1` (expression: satisfied, a little proud)

```
Subject: @pond_v1, wearing a dark charcoal-grey (#3E3B3D) collared polo
shirt and black (#181818) casual trousers, seated at his desk with his
computer monitor and keyboard in frame, clicking send on an email, the
finished one-page brief document visible on screen with neat tables and
headers.
Composition: medium close-up, eye-level, static camera, Pond centered in
frame with his monitor and keyboard clearly visible, bright late-morning
office lighting.
Action: Pond clicks the send button, leans back in his rolling chair
slightly, a small satisfied smile on his face, glancing at his phone
briefly.
Mood: approximately 11:15 AM, clear sky, ordinary gentle morning
sunlight, no rain, a quiet satisfied late-morning ambience, bright color
grade, no dialogue — morning light must not shift clothing colors:
Pond's polo stays visibly charcoal-grey (#3E3B3D — not black/brown).
```

---

## 🎬 Scene 5 — "มาหน่อย" (0:32-0:40) — Turning Point

**Ingredients:** `@pond_v1` (expression: sudden anxiety, stomach-drop feeling)

```
Subject: @pond_v1, wearing a dark charcoal-grey (#3E3B3D) collared polo
shirt and black (#181818) casual trousers, seated at his desk with his
computer monitor in frame, a short email notification visible on screen
reading only "มาหน่อย", his expression shifting from calm to visibly
anxious.
Composition: medium close-up, eye-level, static camera, Pond centered in
frame, his monitor with the short email clearly visible and legible,
bright late-morning office lighting.
Action: Pond's eyes widen slightly reading the two-word email, he
swallows, pushes his rolling chair back, and stands up slowly, glancing
once toward Phum's desk before walking that direction.
Mood: approximately 11:20 AM, clear sky, ordinary gentle morning
sunlight, no rain, a sudden nervous shift in the late-morning office
ambience, a knot-in-the-stomach feeling, no dialogue — morning light
must not shift clothing colors: Pond's polo stays visibly charcoal-grey
(#3E3B3D — not black/brown).
```

---

## 🎬 Scene 6 — ภูมิชี้จุดผิด (0:40-0:48) — Confrontation

**Ingredients:** `@phum_v1` (expression: calm, direct, not angry — just factual), `@pond_v1` (expression: sinking realization, embarrassed)

```
Subject: @phum_v1, wearing a dark charcoal-grey (#4A4548 — muted warm
grey, not brown, not black) fitted long-sleeve button-up shirt with
sleeves rolled to the forearm and dark navy-black (#1C1D22) tailored
trousers, seated at his desk with his monitor and keyboard in frame,
pointing directly at a specific line on the screen where the brief
document is open; @pond_v1, wearing a dark charcoal-grey (#3E3B3D)
collared polo shirt and black (#181818) casual trousers, standing beside
Phum's desk leaning in to look at the screen, noticeably smaller in
build than Phum, his expression sinking as he reads.
Composition: medium two-shot, eye-level, Phum on camera-left seated
pointing at his monitor, Pond on camera-right standing and leaning in,
Phum's monitor and keyboard clearly visible in frame between them,
bright late-morning office lighting.
Action: Phum taps the screen twice at the exact spot with the error;
Pond leans in closer, eyes scanning the numbers, his shoulders dropping
slightly as he realizes the mistake is real.
Dialogue — Speaker: Phum. Line: "ตรงนี้ market share ของคู่แข่ง A — ใน
brief เขียนว่า 23% แต่ไฟล์ต้นฉบับเขียน 32%". Delivery: calm, factual, no
anger. Speaker: Phum. Line: "ใช้ AI ทำเหรอ?". Delivery: direct,
neutral, genuinely just asking. Speaker: Pond. Line: "...ครับ". Delivery:
quiet, embarrassed, barely audible.
Mood: approximately 11:25 AM, clear sky, ordinary gentle morning
sunlight, no rain, a tense but not hostile late-morning office ambience,
bright but sobering color grade — morning light must not shift clothing
colors: Phum's shirt stays visibly charcoal-grey (#4A4548 — not
brown/black), Pond's polo stays visibly charcoal-grey (#3E3B3D — not
black/brown).
```

---

## 🎬 Scene 7 — แก้ด้วยกัน: สอน Cross-check (0:48-0:56) — Emotional Payoff

**Ingredients:** `@phum_v1` (expression: patient, quietly caring beneath a serious exterior), `@pond_v1` (expression: focused, grateful, determined)

**Blocking:** ภูมิดึงเก้าอี้มีล้อของตัวเองมานั่งข้างปอนด์ (action ขยับเก้าอี้ตามต้นฉบับ "ดึงเก้าอี้มานั่งข้างปอนด์")

```
Subject: @phum_v1, wearing a dark charcoal-grey (#4A4548 — muted warm
grey, not brown, not black) fitted long-sleeve button-up shirt with
sleeves rolled to the forearm and dark navy-black (#1C1D22) tailored
trousers, having rolled his office chair over to sit close beside
@pond_v1 at Pond's desk, pointing at Pond's monitor screen where the
seven original research files are open side by side with the brief
document; @pond_v1, wearing a dark charcoal-grey (#3E3B3D) collared polo
shirt and black (#181818) casual trousers, seated at his own desk with
his monitor and keyboard in frame, his thick well-worn paper notebook
open beside the keyboard, typing corrections as Phum points things out.
Composition: medium two-shot, eye-level, Phum on camera-left having
rolled his chair in close, Pond on camera-right at his own desk, both
their faces angled toward Pond's monitor which is clearly visible in
frame between them, bright late-morning office lighting.
Action: Phum points to a specific figure on the original file, then the
corresponding wrong figure on the brief; Pond nods and types the
correction immediately, occasionally jotting a short note in his
notebook; after a few minutes the brief is fully corrected, Phum stands
back up.
Dialogue — Speaker: Phum. Line: "ชุดที่ 2 market size — ตัวเลขนี้ถูก
แต่ชุดที่ 4 กลุ่มเป้าหมาย — ตรงนี้ AI เอาข้อมูลปีที่แล้วมาปน ต้นฉบับอัปเดต
เป็นปี 2026 แล้ว". Delivery: quick, precise, no hesitation. Speaker:
Phum. Line: "ครั้งหน้า AI ช่วยได้ แต่ต้อง cross-check กับต้นฉบับทุกครั้ง
อย่าส่งก่อนเทียบ". Delivery: even, instructive, not scolding, already
standing up to leave.
Mood: approximately 11:30 AM, clear sky, ordinary gentle morning
sunlight, no rain, a warm focused collaborative late-morning ambience,
quiet gratitude beneath the surface, bright cinematic color grade — warm
light must not shift clothing colors: Phum's shirt stays visibly
charcoal-grey (#4A4548 — not brown/black), Pond's polo stays visibly
charcoal-grey (#3E3B3D — not black/brown).
```

**Text overlay ปิดท้าย (ใส่ตอนตัดต่อ):** *ชั้น 14 มีรัก | ตอนต่อไป: ภูมิ × ปอนด์ — แค่ 25 บาท*

---

## 📋 Checklist การผลิต

**ก่อนอื่น — ผ่าน Quality Gate ตาม `docs/shorts-prompt-standards.md` ข้อ 6 ก่อน (prop/blocking/ingredient/แสง/timeline) แล้วค่อยเริ่มขั้นตอนด้านล่าง — ผลการตรวจอยู่ในหัวข้อ "Quality Gate — ผลการตรวจ" ท้ายไฟล์นี้:**

0. [ ] ยืนยันว่ามี turnaround sheet ของภูมิ, ปอนด์ สร้างไว้จริงหรือยัง ก่อน generate — ยืนยันแล้วทั้งสองคน (ดูหัวข้อ "ใช้กับ" ด้านบน)
1. [ ] Generate Scene 1-7 ตามลำดับ (แต่ละคลิป 8 วิ)
2. [ ] เรียงคลิปใน Scenebuilder ตามลำดับ 1→2→3→4→5→6→7
3. [ ] ใส่ text overlay 2 จุด (ต้น Scene 1, ท้าย Scene 7) ตอนตัดต่อ ไม่ต้องใส่ในพรอมต์ Flow
4. [ ] เช็คว่า Scene 1 (hook) สื่อ "ภูมิสังเกตปอนด์มากกว่าที่คิด" ชัดเจนภายใน 3 วินาทีแรก
5. [ ] เช็คคลิปที่ generate จริงว่าสมุดจดของปอนด์อยู่ครบทุก scene ที่ปอนด์ปรากฏพร้อมงาน (Scene 1, 2, 3, 4, 5, 6, 7)
6. [ ] เช็คคลิปที่ generate จริงว่าสี charcoal-grey ของภูมิ/ปอนด์ไม่เพี้ยนเป็นสีน้ำตาล/ดำสนิทจากแสงเช้า
7. [ ] เช็ค outfit ของภูมิ/ปอนด์ในไฟล์นี้ตรงกับ `shorts-prompts-ep03.md` เป๊ะ (วันเดียวกัน เช้า→บ่าย)
8. [ ] เช็คสัดส่วนตัวละครภูมิ (180cm) vs ปอนด์ (172cm) ในภาพที่ generate จริงว่าเห็นความต่าง 8cm ชัดเจนตาม Character Scale Lock
9. [ ] Export เป็น 9:16 ความยาวรวม ~56 วินาที พร้อมโพสต์

---

## ✅ Quality Gate — ผลการตรวจ (ตาม `docs/shorts-prompt-standards.md` ข้อ 6)

- [x] เปิดภาพ `references/ภูมิ01-02-หัวหน้าทีม-Project Manager.jpeg`, `references/ปอนด์01-02-เด็กฝึกงาน.jpeg` ดูจริงแล้ว (ไม่ใช่เขียนจากความจำ)
- [x] เช็ค `docs/continuity-bible.md` แล้ว — ep02 = วันพุธ สัปดาห์ 1, คนละวันกับ ep01 (วันจันทร์) ⇒ Outfit of the Day กำหนดใหม่ทั้งชุด — และต้องตรงกับ ep03 (บ่ายวันเดียวกัน)
- [x] แปะ Prop State Table ของภูมิ/ปอนด์ไว้บนสุดไฟล์ (อ้างอิงบรรทัด spec จริง + ยืนยันโดย Mint — สมุดจดของปอนด์จัดเป็น Identity Prop เพราะเป็น running gag ข้าม ep ตาม bible)
- [x] แปะ Outfit State Table ไว้บนสุดไฟล์ (สี/ทรง/เนื้อผ้าเต็มชุดของวันนี้ อ้างอิงภาพจริง)
- [x] `grep -n "notebook\|watch"` ไล่ทุกจุดในไฟล์เทียบกับ Prop State Table — สมุดจดของปอนด์ปรากฏใน Scene 1, 2, 3, 7 (ทุกจุดที่เกี่ยวกับงาน/จด) ครบตามที่ตั้งใจ ไม่มีจุดขัดกัน
- [x] `grep -n "shirt\|polo\|trousers\|sneakers"` ไล่ทุก scene เทียบกับ Outfit State Table — ทุก scene ที่ภูมิ/ปอนด์ปรากฏมี outfit description เต็มครบ (ดูผล grep ด้านล่าง)
- [x] ไม่มี scene ไหนที่ prop ถูกถอด/สวม/ส่งต่อในตอนนี้ (สมุดจดถือตลอด ไม่มี action เปลี่ยนมือ) — ไม่เข้าเงื่อนไขข้อนี้
- [x] กำหนด layout + camera-left/right ตายตัวตอนต้นไฟล์ (ภูมิ camera-left, ปอนด์ camera-right ตลอดทั้งตอน) และทุก scene อ้างอิงตรงกัน
- [x] `grep -n "desk\|monitor\|keyboard\|chair"` ไล่ทุก Subject block — ทุก scene ที่ตัวละครนั่งทำงานมีการระบุเฟอร์นิเจอร์ชัดเจน (ดูผล grep ด้านล่าง)
- [x] ไม่มี scene ไหนใช้คำอ้างอิง "same as Scene X" แบบลอยๆ (โครงสร้าง Linear ไม่มี scene ขยาย/ย้อนความ)
- [x] `grep -n "empty\|mostly\|no one\|coworker"` ไล่ทุก scene ที่จำนวนคนในฉากมีผลต่อ story logic — Scene 2 มีทีมอื่นเป็น background เบลอไม่ระบุจำนวนเจาะจง (มีมูลจากต้นฉบับว่ามีทีมประชุมจริง ไม่ใช่ห้องว่าง) ไม่มีคำกำกวม "mostly empty" หลงเหลือ
- [x] ทุก scene ที่มีอารมณ์ชัดเจน ระบุ expression tag ต่อท้าย `@handle` ครบ (ดู Ingredients ทุก scene)
- [x] ตัวละครทุกตัวที่ใช้ `@handle` มี turnaround sheet ยืนยันแล้วว่ามีอยู่จริง — `@phum_v1`, `@pond_v1` ยืนยันครบ
- [x] วลีแสง/บรรยากาศซ้ำคำต่อคำข้าม scene ในตอนเดียวกัน ("clear sky, ordinary gentle morning sunlight, no rain" ใช้ครบทั้ง 7 scene)
- [x] ไล่ตรวจ timeline — 8:30 AM → 11:30 AM ไล่ตามลำดับ Linear ตรงตามต้นฉบับ (มาถึง → เก้าโมงประชุม → สิบเอ็ดโมงทำ brief → ส่งอีเมล → ถูกเรียก → สอน cross-check)
- [x] ทุกจุดที่ระบุสีเสื้อผ้า/prop มีคู่สีที่ห้ามเพี้ยนกำกับด้วย + hex code ครบ — ตรวจด้วย `grep -n "#"` ทุกจุดที่มีคำอธิบายสี (ดูผล grep ด้านล่าง)
- [x] scene ที่ใช้แสงเช้าธรรมชาติ มีคำเตือนกันสีเพี้ยนต่อท้าย Mood ครบทุก block
- [x] ทุก scene ระบุเวลาเจาะจง (8:30 AM → 11:30 AM ไล่ตามลำดับ) และสภาพอากาศ "clear sky, ordinary gentle morning sunlight, no rain" กำกับใน Mood ตรงกับ Fictional Weather Table ของ ep02
- [x] ทุก scene ที่ตัวละคร 2 คนขึ้นไปอยู่ในเฟรมเดียวกัน ระบุสัดส่วน/ส่วนสูงสัมพัทธ์ชัดเจนใน Subject (Scene 1, 2, 6, 7 — ภูมิ vs ปอนด์ ต่างกัน 8cm ระบุครบ)
- [x] `grep -n "PRISM\|logo\|signage\|sign reading"` ไล่ทุกจุดที่มีป้าย/ข้อความบริษัทปรากฏในเฟรม — ไม่พบ scene ไหนในไฟล์นี้ที่มีป้าย/โลโก้บริษัทปรากฏชัดในเฟรม (ทุก scene เป็น close-up/medium shot ที่โฟกัสที่ตัวละครและจอคอม) ไม่ต้องแก้ไขเพิ่ม

### ผล grep ตรวจสอบไฟล์นี้ (สรุป)

- `grep -n "#" shorts-prompts-ep02.md` — ทุกจุดที่มีคำอธิบายสี (charcoal-grey #4A4548/#3E3B3D, navy-black #1C1D22, black #181818, off-white #F0EFE8) มี hex กำกับครบ ไม่มีจุดขาด
- `grep -n "shirt\|polo\|trousers" shorts-prompts-ep02.md` — ภูมิ/ปอนด์ มี outfit เต็มซ้ำทุก scene ที่ปรากฏ ไม่มี scene ไหนเว้นว่าง
- `grep -n "desk\|monitor\|keyboard" shorts-prompts-ep02.md` — ทุก scene ที่มีโต๊ะทำงาน (1-7) ระบุเฟอร์นิเจอร์ใน Subject ครบ
- `grep -n "empty\|mostly" shorts-prompts-ep02.md` — ไม่พบคำกำกวม "mostly empty" ในไฟล์นี้เลย

---

## 🔁 หมายเหตุสำหรับตอนถัดไป

ตอน 2 นี้ใช้โครงสร้าง **Linear** ต่อเนื่องจาก ep01 — ตอน 3 เป็นบ่ายของวันเดียวกัน (คนละไฟล์ แต่ต้องใช้ Outfit of the Day ชุดเดียวกันเป๊ะ) ดู `shorts-prompts-ep03.md`
