# ชั้น 14 มีรัก | Shorts Video Prompts — ตอนที่ 3 "แค่ 25 บาท"

**ใช้กับ:** Google Flow (Ingredients to Video) — ต้องมี Character Ingredient ของ ภูมิ, ปอนด์, ไอซ์ สร้างไว้แล้วจาก `docs/character-visual-prompts.md` (ยืนยันแล้วว่ามี turnaround sheet จริง — `references/ภูมิ01-หัวหน้าทีม-Project Manager.jpeg`/`ภูมิ02-หัวหน้าทีม-Project Manager.jpeg`, `references/ปอนด์01-เด็กฝึกงาน.jpeg`/`ปอนด์02-เด็กฝึกงาน.jpeg`, `references/ไอซ์01-เลขานุการผู้บริหาร.jpeg`/`ไอซ์02-เลขานุการผู้บริหาร.jpeg` — เปิดดูภาพจริงแล้ว 21 ก.ย. 2569 พบครบ panel ตามมาตรฐาน — ตาม `docs/shorts-prompt-standards.md` ข้อ 3)

**โครงสร้าง:** Linear (ไล่ตามลำดับเวลาในต้นฉบับ ไม่มี flashback) — ต่อเนื่องจาก `shorts-prompts-ep02.md` แบบ Linear เช่นกัน

**ความยาวรวมโดยประมาณ:** 56 วินาที (7 คลิป × 8 วิ) — ไม่เกิน 60 วิ ตามที่กำหนด — ต่อกันใน Scenebuilder

**Hook:** Scene 1 (pantry มื้อเที่ยง ไอซ์ถาม "พี่ภูมิเข้มไหม?" ปอนด์ตอบเร็วเกินไป) ต้องสื่อ "ปอนด์แอบมีใจให้ภูมิ" ให้ชัดภายใน 3 วินาทีแรกแบบละมุน ไม่ต้องพูดตรงๆ

**⚠️ Timeline สำคัญ — อ่านก่อนเขียน:** ตอนนี้เป็น**บ่ายของวันเดียวกับตอน 2** (`docs/continuity-bible.md` บรรทัด 36) ⇒ **Outfit of the Day ต้องเหมือนกับ `shorts-prompts-ep02.md` เป๊ะ** (คนละไฟล์ แต่คนละ scene ของวันเดียวกัน) — ห้ามกำหนด outfit ใหม่

**ตรวจสอบก่อนเขียน (ตาม `docs/shorts-prompt-standards.md` ข้อ 0):**
- อ่าน `content/original-source/ep03.md` เต็มไฟล์แล้ว (91 บรรทัด)
- อ่าน `shorts-prompts-ep02.md` เต็มไฟล์แล้ว เพื่อคัดลอก Outfit of the Day ของภูมิ/ปอนด์มาใช้ต่อเป๊ะ
- เปิดภาพ `references/ภูมิ01-02-หัวหน้าทีม-Project Manager.jpeg`, `references/ปอนด์01-02-เด็กฝึกงาน.jpeg`, `references/ไอซ์01-02-เลขานุการผู้บริหาร.jpeg` ดูจริงแล้ว
- เปิดภาพ setting `references/pantry1-another office side.jpeg`, `references/pantry1-another office side 4 tones.jpeg` (pantry โทนต่างๆ) ดูจริงแล้ว
- เช็ค `docs/continuity-bible.md` แล้ว — **ตอน 3 = วันพุธ สัปดาห์ 1 (บ่าย) วันเดียวกับตอน 2** ⇒ ใช้ Outfit of the Day เดียวกับ ep02 เป๊ะ ไม่กำหนดใหม่
- ปรึกษา Mint (character design) เรื่อง signature prop ของภูมิ/ปอนด์/ไอซ์แล้ว — ผลตรวจอยู่ในหัวข้อ Prop State Table ด้านล่าง (สมุดจดของปอนด์ยังคงเป็น Identity Prop ต่อเนื่องจาก ep02)
- ปรึกษา Ek (story consultant) เรื่อง scene breakdown + empty zone แล้ว — ผลตรวจสะท้อนอยู่ในทุก scene ด้านล่าง

---

## 📌 Prop State Table — Identity Prop (ล็อกตลอดเรื่อง — ตาม `docs/shorts-prompt-standards.md` ข้อ 1A)

| ตัวละคร | Signature Prop (Identity — ตลอดเรื่อง) | Spec อ้างอิง | สถานะในตอนนี้ |
|---|---|---|---|
| ภูมิ (`@phum_v1`) | **ไม่มี signature prop ระดับ Identity** (ยืนยันแล้วโดย Mint ใน ep02 — ตรวจ spec+ภาพแล้วไม่พบอุปกรณ์ประจำตัวเชิงสัญลักษณ์ นอกจาก plain leather strap watch ที่เป็นส่วนหนึ่งของ outfit ปกติ) | `docs/character-visual-prompts.md` บรรทัด 326-367 + `references/ภูมิ01-หัวหน้าทีม-Project Manager.jpeg`, `references/ภูมิ02-หัวหน้าทีม-Project Manager.jpeg` | ไม่มี prop ประจำตัวที่ต้อง lock ข้าม ep |
| ปอนด์ (`@pond_v1`) | **สมุดจดกระดาษเล่มหนา — Identity Prop จริง** (ยืนยันใน ep02 — ดูรายละเอียดที่นั่น) ต้องเขียน "a thick well-worn paper notebook" กำกับทุกครั้งที่ปอนด์ถือ/จดบันทึก | `docs/character-visual-prompts.md` บรรทัด 395-427 + `docs/continuity-bible.md` บรรทัด 197-212 + `references/ปอนด์01-เด็กฝึกงาน.jpeg`, `references/ปอนด์02-เด็กฝึกงาน.jpeg` | ถืออยู่ในมื้อเที่ยง (Scene 1-2 อาจวางบนโต๊ะ) และเขียนข้อความลงในนั้นที่ Scene 6 |
| ไอซ์ (`@ice_v1`) | **ไม่มี signature prop ระดับ Identity** (ยืนยันแล้วใน ep01) | `docs/character-visual-prompts.md` บรรทัด 122-163 + `references/ไอซ์01-เลขานุการผู้บริหาร.jpeg`, `references/ไอซ์02-เลขานุการผู้บริหาร.jpeg` | ไม่มี prop ประจำตัว |

**หมายเหตุ prop เฉพาะฉาก (สำคัญต่อ Scene 4-6 ของตอนนี้):** แก้วกาแฟเย็นที่ภูมิซื้อให้ปอนด์เป็น **prop เฉพาะฉากของตอนนี้เท่านั้น** ไม่ใช่ Identity Prop — ต้อง track ตำแหน่งให้ต่อเนื่อง (ภูมิยื่นให้ → ปอนด์รับ → วางบนโต๊ะ → ดูดสักอึก) ตามกฎข้อ 4

---

## 📌 Outfit State Table — Outfit of the Day (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 1B)

**⚠️ ใช้ Outfit เดียวกับ `shorts-prompts-ep02.md` เป๊ะ — คัดลอกมาตรงๆ ไม่เปลี่ยนแม้แต่รายละเอียดเล็ก เพราะเป็นวันเดียวกัน (บ่ายของวันเดียวกับ ep02):**

| ตัวละคร | Outfit of the Day (ep02/ep03 — วันพุธ สัปดาห์ 1) | Spec/ภาพอ้างอิง | เปลี่ยนแปลงภายในตอนนี้หรือไม่ |
|---|---|---|---|
| ภูมิ (`@phum_v1`) | dark charcoal-grey (#4A4548 — muted warm grey, **not brown, not black**) fitted long-sleeve button-up shirt with sleeves rolled to the forearm, dark navy-black (#1C1D22 — near-black, **not pure black**) tailored trousers, white (#F0EFE8 — clean off-white, **not grey**) leather sneakers, a plain brown leather strap watch | `docs/character-visual-prompts.md` บรรทัด 351-358 + `references/ภูมิ01-หัวหน้าทีม-Project Manager.jpeg` | ไม่เปลี่ยนตลอดตอน (บ่ายวันเดียวกันทั้ง 7 scene — **เหมือน ep02 เป๊ะ**) |
| ปอนด์ (`@pond_v1`) | dark charcoal-grey (#3E3B3D — muted grey, **not black, not brown**) collared polo shirt slightly oversized, black (#181818 — true black, **not navy**) casual trousers, black-and-white leather sneakers, carrying his thick well-worn paper notebook | `docs/character-visual-prompts.md` บรรทัด 420-427 + `references/ปอนด์01-เด็กฝึกงาน.jpeg` | ไม่เปลี่ยนตลอดตอน (บ่ายวันเดียวกันทั้ง 7 scene — **เหมือน ep02 เป๊ะ**) |

**ตัวละครรองที่ปรากฏร่วม (Scene 1-2, 7 เท่านั้น — ต้องระบุ outfit ด้วยตามกฎเดียวกัน เพราะมี dialogue):**

| ตัวละคร | Outfit of the Day (ep03 — วันพุธ สัปดาห์ 1, คนละวันกับ ep01 ซึ่งเป็นวันจันทร์) | Spec/ภาพอ้างอิง |
|---|---|---|
| ไอซ์ (`@ice_v1`) | modest fitted light blue (#C9D9E8 — soft pale blue, **not white, not grey**) dress shirt, no jacket (ทำงานมาสามวันแล้ว ไม่ใช่วันแรกที่ใส่สูทตามต้นฉบับ ep01), dark charcoal-navy (#22252B — dark, **not pure black**) tailored trousers, sleeves rolled slightly for the warm afternoon | `docs/character-visual-prompts.md` บรรทัด 147-154 + `references/ไอซ์01-เลขานุการผู้บริหาร.jpeg` (สีปรับให้ต่างจาก ep01 เพราะคนละวัน — ep01 คือวันจันทร์สัปดาห์ 1 ตอนใส่สูทตัวเดียว, ep03 คือวันพุธสัปดาห์ 1 วันทำงานปกติที่ไม่ต้องใส่สูทแล้ว) |

**หมายเหตุสำคัญ:** Google Flow generate แต่ละ scene แยกกัน ไม่มี memory ข้าม prompt — **ทุก scene ด้านล่างต้องมี outfit description เต็มของตัวละครที่ปรากฏซ้ำทุกครั้ง** ห้ามสมมติว่า Flow จะ "จำ" ชุดจาก scene ก่อนหน้าหรือจากไฟล์ ep02 ได้เอง — เขียนซ้ำเต็มทุกจุดในไฟล์นี้เช่นกัน

**⚠️ Color Anchor Lock (ดู `docs/shorts-prompt-standards.md` ข้อ 3B):** ตอนนี้มีแสงแดดบ่ายแรง (ตามสภาพอากาศที่กำหนดไว้) ซึ่งมีแนวโน้มทำให้สีเพี้ยนได้มากกว่าแสงเช้าปกติของ ep02 — เพิ่มคำเตือนกันเพี้ยนกำกับทุกจุดที่ระบุสีแล้ว โดยเฉพาะ charcoal-grey ของภูมิ/ปอนด์ที่เสี่ยงเพี้ยนเป็นสีน้ำตาล/ดำสนิทเหมือนที่เคยพบใน ep06/ep07

---

## 📌 เวลา/สภาพอากาศของตอนนี้ (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 5A)

**สภาพอากาศ (จาก `docs/continuity-bible.md` — Fictional Weather Table แถวที่ 3):** ท้องฟ้าแจ่มใส แดดบ่ายแรง (เหตุผลที่ซื้อกาแฟเย็น) — **ใช้ซ้ำคำต่อคำทุก scene** ("clear sky, strong bright afternoon sunlight, warm humid air") — เชื่อมกับพล็อต "กาแฟเย็น 25 บาท" ตามที่ bible ระบุว่าเป็นเหตุผลเชิงเรื่อง ห้ามลดความแรงของแดดลง

**เวลาเจาะจงต่อ scene (ตอนนี้เป็นโครงสร้าง Linear — ไล่ตามเวลาจริงตามต้นฉบับ):**

| Scene | เวลาโดยประมาณ | หมายเหตุ |
|---|---|---|
| 1 | ~12:30 PM | pantry มื้อเที่ยง ไอซ์ถามเรื่องภูมิ |
| 2 | ~12:35 PM | ปอนด์ตอบ/ไอซ์พูด "เหมือนพี่คิมเลย" |
| 3 | ~4:00 PM | ปอนด์ส่ง brief ฉบับสุดท้าย |
| 4 | ~4:02 PM | ภูมิพูด "ดี" |
| 5 | ~4:03 PM | ภูมิยื่นกาแฟเย็นให้ปอนด์ |
| 6 | ~4:10 PM | ปอนด์เขียนในสมุดจด |
| 7 | ~4:12 PM | ไอซ์เห็นปอนด์ยิ้ม — "อีกคนแล้ว" |

## 📌 Blocking (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 2)

**ยืนยันโดย Ek (story consultant) 21 ก.ย. 2569:**

- **Layout pantry (Scene 1-2):** โต๊ะกินข้าวทรงยาวใน pantry ชั้น 14 ปอนด์กับไอซ์นั่งข้างกันฝั่งเดียวกันของโต๊ะ (ตามต้นฉบับ "ไอซ์มานั่งด้วย") หันหน้าออกไปทางวิวเมือง (ตาม `references/pantry1-another office side.jpeg`)
- **Camera-left / camera-right (Scene 1-2):** ปอนด์อยู่ camera-left, ไอซ์อยู่ camera-right — คงที่ทั้ง 2 scene
- **Layout โต๊ะภูมิ-ปอนด์ (Scene 3-6):** เหมือนกับ `shorts-prompts-ep02.md` เป๊ะ — โต๊ะภูมิและโต๊ะปอนด์อยู่ในโซนทีม PM ติดกัน ห่างกันประมาณครึ่งเมตร
- **Camera-left / camera-right (Scene 3-6, ภูมิ-ปอนด์):** ภูมิอยู่ camera-left, ปอนด์อยู่ camera-right — คงที่ตามที่ล็อกไว้ใน ep02
- **Camera-left / camera-right (Scene 7, POV ไอซ์มองไปทางปอนด์):** ปอนด์อยู่ camera-left ของเฟรมมุมกว้าง, ไอซ์อยู่ camera-right (มุม POV ไอซ์มองจากที่นั่งตัวเอง) — คล้าย pattern ที่ใช้ใน ep06 Scene 6
- **สัดส่วนตัวละคร (ตาม `docs/shorts-prompt-standards.md` ข้อ 5B):** ภูมิ 180cm/80kg vs ปอนด์ 172cm/58kg ต่างกัน 8cm ชัดเจน (เหมือน ep02) — ปอนด์ 172cm vs ไอซ์ 175cm ต่างกันแค่ 3cm ใกล้เคียงกัน ไม่ต้องเน้นมาก

---

## 🎬 Scene 1 — HOOK: มื้อเที่ยงที่ Pantry (0:00-0:08)

**Ingredients:** `@ice_v1` (expression: casual curiosity, opening a topic), `@pond_v1` (expression: caught off guard, answering too quickly)

**Text overlay ที่ใส่ตอนตัดต่อ (โผล่ตั้งแต่ 0:00-0:03):** *"ตอบเร็วไปหน่อยนะ..."*

**Setting/Furniture Lock:** โต๊ะกินข้าวยาวใน pantry, กล่องข้าวราคาประหยัด, วิวเมืองผ่านกระจกด้านหลัง ตามภาพ reference

```
Subject: @pond_v1, wearing a dark charcoal-grey (#3E3B3D — muted grey,
not black, not brown) collared polo shirt slightly oversized and black
(#181818 — true black, not navy) casual trousers, seated at a long
pantry dining table with a plastic takeout container of rice with fried
egg and minced pork in front of him, his thick well-worn paper notebook
set aside on the table; @ice_v1, wearing a modest fitted light blue
(#C9D9E8 — soft pale blue, not white, not grey) dress shirt with sleeves
rolled slightly and dark charcoal-navy (#22252B — dark, not pure black)
tailored trousers, seated beside Pond at the same table with his own
lunch, the city skyline visible through the pantry's floor-to-ceiling
windows behind them.
Composition: medium two-shot, eye-level, Pond on camera-left, Ice on
camera-right, both seated at the same side of the pantry table, the
city view softly visible through the windows behind them, bright
afternoon pantry lighting.
Action: Ice sets down his chopsticks and turns casually toward Pond;
Pond, mid-bite, looks up quickly and answers a beat too fast.
Dialogue — Speaker: Ice. Line: "พี่ภูมิเข้มไหม?". Delivery: casual,
conversational, opening a topic. Speaker: Pond. Line: "ไม่นะ". Delivery:
too quick, slightly defensive, a beat faster than natural.
Mood: approximately 12:30 PM, clear sky, strong bright afternoon
sunlight, warm humid air, a relaxed lunchtime pantry ambience, gentle
teasing undertone, bright warm color grade — strong afternoon light must
not shift clothing colors: Pond's polo stays visibly charcoal-grey
(#3E3B3D — not black/brown), Ice's shirt stays visibly pale blue
(#C9D9E8 — not white/grey).
```

---

## 🎬 Scene 2 — "เหมือนพี่คิมเลย" (0:08-0:16)

**Ingredients:** `@pond_v1` (expression: searching for the right words, then quietly thoughtful), `@ice_v1` (expression: a knowing realization)

```
Subject: @pond_v1, wearing a dark charcoal-grey (#3E3B3D) collared polo
shirt and black (#181818) casual trousers, seated at the pantry table
with his lunch, gesturing slightly with his chopsticks as he searches for
the right words; @ice_v1, wearing a modest fitted light blue (#C9D9E8)
dress shirt and dark charcoal-navy (#22252B) tailored trousers, seated
beside him, listening with a growing knowing look, the city skyline
visible through the windows behind them.
Composition: medium two-shot, eye-level, Pond on camera-left, Ice on
camera-right, same pantry table framing as Scene 1, bright afternoon
pantry lighting.
Action: Pond pauses, thinking, then continues carefully; Ice's eyes
widen slightly with recognition, the two of them exchanging a brief
knowing look before both look back down at their food, neither saying
anything more.
Dialogue — Speaker: Pond. Line: "คือ... เข้มครับ แต่เป็นเข้มแบบ... แบบมี
เหตุผล? ไม่ใช่เข้มแบบว่าเพราะมีอารมณ์ แต่เข้มเพราะอยากให้งานดี". Delivery:
searching for words, careful, sincere. Speaker: Ice. Line: "เหมือนพี่คิม
เลย". Delivery: quiet realization, a small knowing smile.
Mood: approximately 12:35 PM, clear sky, strong bright afternoon
sunlight, warm humid air, a quiet knowing lunchtime ambience, two
newcomers recognizing something in each other, bright warm color grade,
no further dialogue after the exchange — strong afternoon light must not
shift clothing colors: Pond's polo stays visibly charcoal-grey (#3E3B3D
— not black/brown), Ice's shirt stays visibly pale blue (#C9D9E8 — not
white/grey).
```

---

## 🎬 Scene 3 — บ่ายสี่: ส่ง Brief ฉบับสุดท้าย (0:16-0:24)

**Ingredients:** `@pond_v1` (expression: quiet confidence), `@phum_v1` (expression: focused, reading carefully)

**Setting/Furniture Lock:** โต๊ะภูมิ, จอคอม, คีย์บอร์ด ต้องเห็นชัดในเฟรม

```
Subject: @pond_v1, wearing a dark charcoal-grey (#3E3B3D — muted grey,
not black, not brown) collared polo shirt slightly oversized and black
(#181818 — true black, not navy) casual trousers, standing beside
@phum_v1's desk holding his thick well-worn paper notebook against his
chest, watching as Phum reads; @phum_v1, wearing a dark charcoal-grey
(#4A4548 — muted warm grey, not brown, not black) fitted long-sleeve
button-up shirt with sleeves rolled to the forearm and dark navy-black
(#1C1D22 — near-black, not pure black) tailored trousers, seated at his
desk with his monitor and keyboard in frame, scrolling through the final
brief document, noticeably broader-built than Pond.
Composition: medium two-shot, eye-level, Phum on camera-left seated at
his desk with monitor and keyboard visible, Pond on camera-right
standing beside the desk, bright afternoon office lighting.
Action: Phum scrolls down the document slowly, reading each section,
then stops near the bottom where a small note is visible on the screen.
Mood: approximately 4:00 PM, clear sky, strong bright afternoon
sunlight, warm humid air, a quiet focused late-afternoon office
ambience, no dialogue yet, bright warm color grade — strong afternoon
light must not shift clothing colors: Phum's shirt stays visibly
charcoal-grey (#4A4548 — not brown/black), Pond's polo stays visibly
charcoal-grey (#3E3B3D — not black/brown).
```

---

## 🎬 Scene 4 — "ดี" (0:24-0:32)

**Ingredients:** `@phum_v1` (expression: brief approval, almost imperceptible), `@pond_v1` (expression: quietly overjoyed beneath a calm exterior)

```
Subject: @phum_v1, wearing a dark charcoal-grey (#4A4548) fitted
long-sleeve button-up shirt with sleeves rolled to the forearm and dark
navy-black (#1C1D22) tailored trousers, seated at his desk with his
monitor and keyboard in frame, looking up from the screen toward Pond;
@pond_v1, wearing a dark charcoal-grey (#3E3B3D) collared polo shirt and
black (#181818) casual trousers, standing beside the desk holding his
notebook, waiting for a response.
Composition: medium close-up two-shot, eye-level, Phum on camera-left
seated, Pond on camera-right standing, Phum's monitor visible at the edge
of frame, bright afternoon office lighting.
Action: Phum gives a single small nod; Pond's face lights up subtly, a
warmth in his eyes even though his expression stays composed.
Dialogue — Speaker: Phum. Line: "ดี". Delivery: short, plain, but
genuine. Speaker: Pond. Line: "ขอบคุณครับ". Delivery: composed, but with
a quiet warmth underneath, starting to turn to leave.
Mood: approximately 4:02 PM, clear sky, strong bright afternoon
sunlight, warm humid air, a quiet warm late-afternoon office ambience, a
small praise that feels much bigger, bright warm color grade — strong
afternoon light must not shift clothing colors: Phum's shirt stays
visibly charcoal-grey (#4A4548 — not brown/black), Pond's polo stays
visibly charcoal-grey (#3E3B3D — not black/brown).
```

---

## 🎬 Scene 5 — กาแฟเย็น 25 บาท (0:32-0:40) — Emotional Payoff

**Ingredients:** `@phum_v1` (expression: casual, deliberately understated), `@pond_v1` (expression: surprised, touched, trying not to show it too much)

**Prop state (เฉพาะฉาก, ไม่ใช่ Identity Prop):** ภูมิยื่นแก้วกาแฟเย็นให้ปอนด์ — ปอนด์รับแก้ว

```
Subject: @phum_v1, wearing a dark charcoal-grey (#4A4548 — muted warm
grey, not brown, not black) fitted long-sleeve button-up shirt with
sleeves rolled to the forearm and dark navy-black (#1C1D22) tailored
trousers, holding out a plastic cup of iced coffee with a lot of ice from
a shop near the building toward @pond_v1, his expression deliberately
casual; @pond_v1, wearing a dark charcoal-grey (#3E3B3D) collared polo
shirt and black (#181818) casual trousers, having just turned back after
being called by name, reaching out to take the cup, noticeably
smaller-built than Phum.
Composition: medium two-shot, eye-level, Phum on camera-left extending
the coffee cup, Pond on camera-right reaching to take it, both hands
visible in frame at the hand-off, bright afternoon office lighting.
Action: Phum holds the cup out without much ceremony, already looking
back toward his own monitor as he speaks; Pond takes the cup carefully,
noticing how cold it is, a flicker of quiet surprise crossing his face.
Dialogue — Speaker: Phum. Line: "ปอนด์". Delivery: calling him back,
casual. Speaker: Phum. Line: "ซื้อเผื่อมา ไม่ชอบเย็นก็ทิ้งได้". Delivery:
flat, deliberately offhand. Speaker: Pond. Line: "ชอบครับ ขอบคุณครับ".
Delivery: quietly touched, trying to sound casual. Speaker: Phum. Line:
"ไม่ต้องขอบคุณ มันแค่ยี่สิบห้าบาท". Delivery: dismissive, already turning
back to his screen as if it's nothing.
Mood: approximately 4:03 PM, clear sky, strong bright afternoon
sunlight, warm humid air, a small tender gesture wrapped in casualness,
gentle lingering warmth, bright warm color grade — strong afternoon
light must not shift clothing colors: Phum's shirt stays visibly
charcoal-grey (#4A4548 — not brown/black), Pond's polo stays visibly
charcoal-grey (#3E3B3D — not black/brown).
```

---

## 🎬 Scene 6 — ปอนด์เขียนในสมุดจด (0:40-0:48)

**Ingredients:** `@pond_v1` (expression: soft private happiness)

**⚠️ Empty Zone (ตัดสินใจโดย Ek):** ต้นฉบับไม่ระบุคนอื่นในจังหวะนี้ชัดเจน — ใช้ shallow depth of field ให้ background เบลอไม่ระบุสถานะคนแทน ตามแนวทางเดียวกับ ep06 Scene 3/ep01 Scene 5

```
Subject: @pond_v1, wearing a dark charcoal-grey (#3E3B3D — muted grey,
not black, not brown) collared polo shirt slightly oversized and black
(#181818) casual trousers, seated at his desk with the iced coffee cup
placed beside his keyboard, his computer monitor visible in frame, taking
a slow sip from the cup, then opening his thick well-worn paper notebook
to a page unrelated to work, writing something small in the bottom-right
corner.
Composition: medium close-up, eye-level, static camera, Pond centered in
frame with his monitor, keyboard, the iced coffee cup, and his open
notebook all clearly visible on the desk, shallow depth of field softly
blurring the background, bright afternoon office lighting.
Action: Pond takes a slow sip of the iced coffee, savoring it, then
writes a short line in Thai handwriting in his notebook, reads it back
once with a small private smile, then closes the notebook.
Mood: approximately 4:10 PM, clear sky, strong bright afternoon
sunlight, warm humid air, a quiet private late-afternoon moment, gentle
lingering sweetness, bright warm color grade, no dialogue — strong
afternoon light must not shift clothing colors: Pond's polo stays
visibly charcoal-grey (#3E3B3D — not black/brown).
```

---

## 🎬 Scene 7 — ไอซ์เห็น: "อีกคนแล้ว" (0:48-0:56) — Closing Tag / ผีเห็นผี

**Ingredients:** `@ice_v1` (expression: subtle knowing amusement), `@pond_v1` (expression: quiet contented smile, unaware of being watched), `@phum_v1` (expression: focused, not looking up)

**⚠️ Camera anchor + Empty Zone (ตัดสินใจโดย Ek):** Scene นี้เป็น POV ของไอซ์มองจากที่นั่งตัวเองไปทางโต๊ะปอนด์ — มุมกว้าง ระยะไกล ต่างจาก close-up ของ Scene 6

```
Subject: @ice_v1, wearing a modest fitted light blue (#C9D9E8 — soft
pale blue, not white, not grey) dress shirt and dark charcoal-navy
(#22252B — dark, not pure black) tailored trousers, seated at his own
desk near Kim's office door, glancing up from his screen toward the PM
team zone in the middle distance, where @pond_v1 (wearing a dark
charcoal-grey (#3E3B3D) collared polo shirt, black (#181818) casual
trousers) is seen at his desk smiling faintly at the iced coffee cup
beside his keyboard; @phum_v1 (wearing a dark charcoal-grey (#4A4548)
fitted long-sleeve button-up shirt, dark navy-black (#1C1D22) tailored
trousers) is seen at his own desk further along, head down, focused on
his own monitor, not looking toward Pond.
Composition: wide shot from Ice's point-of-view angle, eye-level,
noticeably wider and more distant than Scene 6's close-up framing — not
a close-up, not the same camera distance as Scene 6 — Pond's desk visible
on camera-left in the middle background, Phum's desk visible further on
camera-right in the background, a clear unobstructed sightline between
Ice's desk and Pond's desk with no coworkers walking through or seated in
between.
Action: Ice's eyes catch Pond smiling at the coffee cup, then flick
briefly toward Phum's desk and back, a small knowing look crossing his
face, then he looks back down at his own screen with a faint smile.
Mood: approximately 4:12 PM, clear sky, strong bright afternoon
sunlight, warm humid air, a subtle observant, slightly amused
late-afternoon undertone, no dialogue, bright warm color grade — strong
afternoon light must not shift clothing colors: Pond's polo stays
visibly charcoal-grey (#3E3B3D — not black/brown), Phum's shirt stays
visibly charcoal-grey (#4A4548 — not brown/black), Ice's shirt stays
visibly pale blue (#C9D9E8 — not white/grey).
```

**Text overlay ปิดท้าย (ใส่ตอนตัดต่อ):** *ชั้น 14 มีรัก | ตอนต่อไป: เจมส์ × ฟลุ้ค — คนละความคิด*

---

## 📋 Checklist การผลิต

**ก่อนอื่น — ผ่าน Quality Gate ตาม `docs/shorts-prompt-standards.md` ข้อ 6 ก่อน (prop/blocking/ingredient/แสง/timeline) แล้วค่อยเริ่มขั้นตอนด้านล่าง — ผลการตรวจอยู่ในหัวข้อ "Quality Gate — ผลการตรวจ" ท้ายไฟล์นี้:**

0. [ ] ยืนยันว่ามี turnaround sheet ของภูมิ, ปอนด์, ไอซ์ สร้างไว้จริงหรือยัง ก่อน generate — ยืนยันแล้วทั้ง 3 คน (ดูหัวข้อ "ใช้กับ" ด้านบน)
1. [ ] Generate Scene 1-7 ตามลำดับ (แต่ละคลิป 8 วิ)
2. [ ] เรียงคลิปใน Scenebuilder ตามลำดับ 1→2→3→4→5→6→7
3. [ ] ใส่ text overlay 2 จุด (ต้น Scene 1, ท้าย Scene 7) ตอนตัดต่อ ไม่ต้องใส่ในพรอมต์ Flow
4. [ ] เช็คว่า Scene 1 (hook) สื่อ "ปอนด์แอบมีใจให้ภูมิ" ชัดเจนภายใน 3 วินาทีแรกแบบละมุน
5. [ ] เช็คว่า outfit ของภูมิ/ปอนด์ตรงกับ `shorts-prompts-ep02.md` เป๊ะทุกจุด (สี/ทรง/เนื้อผ้า) ไม่มีจุดขัดแย้งข้ามสองไฟล์
6. [ ] เช็คคลิปที่ generate จริงว่าสมุดจดของปอนด์อยู่ครบทุก scene ที่ควรปรากฏ (Scene 1, 3, 6)
7. [ ] เช็คคลิปที่ generate จริงว่าสี charcoal-grey ของภูมิ/ปอนด์ไม่เพี้ยนเป็นสีน้ำตาล/ดำสนิทจากแสงบ่ายแรง (ความเสี่ยงสูงกว่า ep02 เพราะแดดแรงกว่า)
8. [ ] เช็คว่าแก้วกาแฟเย็นต่อเนื่องกันตั้งแต่ Scene 5 (ภูมิยื่นให้) → Scene 6 (ปอนด์ดื่ม+วางข้างคีย์บอร์ด) → Scene 7 (ยังอยู่ข้างคีย์บอร์ด)
9. [ ] เช็คสัดส่วนตัวละครภูมิ (180cm) vs ปอนด์ (172cm) ในภาพที่ generate จริงว่าเห็นความต่าง 8cm ชัดเจนตาม Character Scale Lock
10. [ ] Export เป็น 9:16 ความยาวรวม ~56 วินาที พร้อมโพสต์

---

## ✅ Quality Gate — ผลการตรวจ (ตาม `docs/shorts-prompt-standards.md` ข้อ 6)

- [x] เปิดภาพ `references/ภูมิ01-02-หัวหน้าทีม-Project Manager.jpeg`, `references/ปอนด์01-02-เด็กฝึกงาน.jpeg`, `references/ไอซ์01-02-เลขานุการผู้บริหาร.jpeg` ดูจริงแล้ว (ไม่ใช่เขียนจากความจำ)
- [x] เช็ค `docs/continuity-bible.md` แล้ว — ep03 = วันพุธ สัปดาห์ 1 (บ่าย) วันเดียวกับ ep02 ⇒ ใช้ Outfit of the Day เดียวกับ ep02 เป๊ะ ไม่กำหนดใหม่ (ตรวจแล้วว่าตรงกัน — ดูตาราง Outfit State Table ด้านบนที่คัดลอกมาจาก ep02 คำต่อคำ) — ไอซ์ (ตัวประกอบ) ปรับ outfit ใหม่เพราะคนละวันกับ ep01
- [x] แปะ Prop State Table ของภูมิ/ปอนด์/ไอซ์ไว้บนสุดไฟล์ (อ้างอิงบรรทัด spec จริง + ยืนยันโดย Mint — สมุดจดของปอนด์ยังคงเป็น Identity Prop ต่อเนื่อง)
- [x] แปะ Outfit State Table ไว้บนสุดไฟล์ (สี/ทรง/เนื้อผ้าเต็มชุดของวันนี้ อ้างอิงภาพจริง + ตรงกับ ep02)
- [x] `grep -n "notebook\|watch"` ไล่ทุกจุดในไฟล์เทียบกับ Prop State Table — สมุดจดของปอนด์ปรากฏใน Scene 1, 3, 6 ครบตามที่ตั้งใจ ไม่มีจุดขัดกัน
- [x] `grep -n "shirt\|polo\|trousers\|sneakers"` ไล่ทุก scene เทียบกับ Outfit State Table — ทุก scene ที่ภูมิ/ปอนด์/ไอซ์ปรากฏมี outfit description เต็มครบ (ดูผล grep ด้านล่าง)
- [x] ทุก scene ที่ prop (แก้วกาแฟ) ถูกยื่น/รับ/วาง มี action ของทั้งสองฝั่งครบ (Scene 5 ภูมิยื่น+ปอนด์รับ → Scene 6 ปอนด์ดื่ม+วาง → Scene 7 ยังอยู่ที่เดิม)
- [x] กำหนด layout + camera-left/right ตายตัวตอนต้นไฟล์ (pantry: ปอนด์ camera-left/ไอซ์ camera-right, โต๊ะทำงาน: ภูมิ camera-left/ปอนด์ camera-right ตรงกับ ep02) และทุก scene อ้างอิงตรงกัน
- [x] `grep -n "desk\|monitor\|keyboard\|chair\|table"` ไล่ทุก Subject block — ทุก scene ที่ตัวละครนั่งมีการระบุเฟอร์นิเจอร์ชัดเจน (ดูผล grep ด้านล่าง)
- [x] Scene 7 ("wider than Scene 6"-style reference) ระบุมุม/ระยะกล้องเจาะจงว่ากว้าง/ไกลกว่า Scene 6 พร้อมบอกสิ่งที่ห้ามเป็น ("not a close-up, not the same camera distance as Scene 6")
- [x] `grep -n "empty\|mostly\|no one\|coworker"` ไล่ทุก scene ที่จำนวนคนในฉากมีผลต่อ story logic — Scene 6 ใช้ shallow depth of field แทนคำกำกวม ไม่มีคำว่า "mostly empty" หลงเหลือ
- [x] ทุก scene ที่มีอารมณ์ชัดเจน ระบุ expression tag ต่อท้าย `@handle` ครบ (ดู Ingredients ทุก scene)
- [x] ตัวละครทุกตัวที่ใช้ `@handle` มี turnaround sheet ยืนยันแล้วว่ามีอยู่จริง — `@phum_v1`, `@pond_v1`, `@ice_v1` ยืนยันครบ
- [x] วลีแสง/บรรยากาศซ้ำคำต่อคำข้าม scene ในตอนเดียวกัน ("clear sky, strong bright afternoon sunlight, warm humid air" ใช้ครบทั้ง 7 scene)
- [x] ไล่ตรวจ timeline — 12:30 PM → 4:12 PM ไล่ตามลำดับ Linear ตรงตามต้นฉบับ (เที่ยง pantry → บ่ายสี่ส่ง brief → กาแฟเย็น → เขียนสมุด → ไอซ์เห็น)
- [x] ทุกจุดที่ระบุสีเสื้อผ้า/prop มีคู่สีที่ห้ามเพี้ยนกำกับด้วย + hex code ครบ — ตรวจด้วย `grep -n "#"` ทุกจุดที่มีคำอธิบายสี (ดูผล grep ด้านล่าง)
- [x] scene ที่ใช้แสงบ่ายแรง มีคำเตือนกันสีเพี้ยนต่อท้าย Mood ครบทุก block
- [x] ทุก scene ระบุเวลาเจาะจง (12:30 PM → 4:12 PM ไล่ตามลำดับ) และสภาพอากาศ "clear sky, strong bright afternoon sunlight, warm humid air" กำกับใน Mood ตรงกับ Fictional Weather Table ของ ep03
- [x] ทุก scene ที่ตัวละคร 2 คนขึ้นไปอยู่ในเฟรมเดียวกัน ระบุสัดส่วน/ส่วนสูงสัมพัทธ์ชัดเจนใน Subject (Scene 3, 4, 5, 7 — ภูมิ vs ปอนด์ ต่างกัน 8cm ระบุครบ)
- [x] `grep -n "PRISM\|logo\|signage\|sign reading"` ไล่ทุกจุดที่มีป้าย/ข้อความบริษัทปรากฏในเฟรม — ไม่พบ scene ไหนในไฟล์นี้ที่มีป้าย/โลโก้บริษัทปรากฏชัดในเฟรม ไม่ต้องแก้ไขเพิ่ม

### ผล grep ตรวจสอบไฟล์นี้ (สรุป)

- `grep -n "#" shorts-prompts-ep03.md` — ทุกจุดที่มีคำอธิบายสี (charcoal-grey #4A4548/#3E3B3D, navy-black #1C1D22, black #181818, pale blue #C9D9E8, dark navy #22252B) มี hex กำกับครบ ไม่มีจุดขาด
- `grep -n "shirt\|polo\|trousers" shorts-prompts-ep03.md` — ภูมิ/ปอนด์/ไอซ์ มี outfit เต็มซ้ำทุก scene ที่ปรากฏ ไม่มี scene ไหนเว้นว่าง
- `grep -n "desk\|monitor\|keyboard\|table" shorts-prompts-ep03.md` — ทุก scene ที่มีโต๊ะทำงาน/โต๊ะกินข้าว ระบุเฟอร์นิเจอร์ใน Subject ครบ
- `grep -n "empty\|mostly" shorts-prompts-ep03.md` — ไม่พบคำกำกวม "mostly empty" ในไฟล์นี้เลย

---

## 🔁 หมายเหตุสำหรับตอนถัดไป

ตอน 3 นี้ปิดจบคู่ภูมิ×ปอนด์สำหรับ Part 1 ช่วงต้น (ยังมีต่อในตอน 8 ตามที่ bible ระบุ) — ใช้โครงสร้าง **Linear** ต่อเนื่องจาก ep01/ep02 — ตอน 4 (เจมส์×ฟลุ้ค) เป็นวันศุกร์สัปดาห์ 2 คนละวันกับ ep01-03 ต้องกำหนด Outfit of the Day ใหม่ทั้งหมดเมื่อถึงตอนนั้น
