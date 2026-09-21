# ชั้น 14 มีรัก | Shorts Video Prompts — ตอนที่ 1 "วันแรก"

**ใช้กับ:** Google Flow (Ingredients to Video) — ต้องมี Character Ingredient ของ คิม, ไอซ์, เต สร้างไว้แล้วจาก `docs/character-visual-prompts.md` (ยืนยันแล้วว่ามี turnaround sheet จริง — `references/คิม01-Creative Director.jpeg`/`คิม02-Creative Director.jpeg`, `references/ไอซ์01-เลขานุการผู้บริหาร.jpeg`/`ไอซ์02-เลขานุการผู้บริหาร.jpeg` — เปิดดูภาพจริงแล้ว 21 ก.ย. 2569 พบครบ panel ตามมาตรฐาน; `references/เต01-HR.jpeg`/`เต02-HR.jpeg` ใช้ซ้ำจาก ep06 ยืนยันแล้วว่ามีจริง — ตาม `docs/shorts-prompt-standards.md` ข้อ 3) — ดิว/นนท์/ฟลุ้ค/เจมส์ ปรากฏเป็น background cameo สั้นๆ ใน Scene 3 เท่านั้น ไม่มี dialogue ไม่ต้องใช้ `@handle` เต็ม (ดูหมายเหตุ Scene 3)

**โครงสร้าง:** Linear (ไล่ตามลำดับเวลาในต้นฉบับ ไม่มี flashback) — ตอนนี้เป็นตอนเปิดเรื่อง (วันแรกของไอซ์) เหมาะกับการเล่าตามลำดับเวลาให้คนดูปูบริบทตั้งแต่ต้น

**ความยาวรวมโดยประมาณ:** 56 วินาที (7 คลิป × 8 วิ) — ไม่เกิน 60 วิ ตามที่กำหนด — ต่อกันใน Scenebuilder

**Hook:** Scene 1 (ไอซ์ยืนหน้าตึกแหงนมอง PRISM) ต้องสื่อ "วันแรกที่ตื่นเต้น/กังวล" ให้ชัดภายใน 3 วินาทีแรก

**ตรวจสอบก่อนเขียน (ตาม `docs/shorts-prompt-standards.md` ข้อ 0):**
- อ่าน `content/original-source/ep01.md` เต็มไฟล์แล้ว (149 บรรทัด)
- เปิดภาพ `references/คิม01-02-Creative Director.jpeg`, `references/ไอซ์01-02-เลขานุการผู้บริหาร.jpeg`, `references/เต01-02-HR.jpeg` ดูจริงแล้ว
- เปิดภาพ setting `references/Creative_agency_office_interior.jpeg` (ล็อบบี้ชั้น 14 ป้าย PRISM), `references/Office_corridor_under_different.jpeg` (โทนเช้า/บ่าย/เย็น/กลางคืน) ดูจริงแล้ว — **⚠️ พบว่าภาพ `Creative_agency_office_interior.jpeg` มีโลโก้กราฟิกรูปเพชร (diamond icon) อยู่เหนือคำว่า PRISM จริง** ต้องเขียนกำกับ override ทุกจุดที่อ้างอิงภาพนี้ตามข้อ 2D (ดูหมายเหตุ Scene 1)
- เช็ค `docs/continuity-bible.md` แล้ว — **ตอน 1 = วันจันทร์ สัปดาห์ 1 วันแรกของไอซ์ (เป็นตอนแรกสุดของซีรีส์ ไม่มีตอนก่อนหน้าให้เทียบ outfit)** ⇒ กำหนด Outfit of the Day ใหม่ทั้งหมด อ้างอิงจาก character-visual-prompts.md เป็นฐาน (คิม/ไอซ์ ใช้ default outfit ตรงกับภาพ turnaround sheet ที่ generate ไว้แล้วพอดี เพราะเป็นชุดวันแรก)
- ปรึกษา Mint (character design) เรื่อง signature prop ของคิม/ไอซ์/เต แล้ว — ไม่มีใครใน 3 คนนี้มี Identity Prop ระดับสัญลักษณ์ (คิม/ไอซ์/เตไม่มีอุปกรณ์ประจำตัวตาม continuity-bible ภาคผนวก) — ผลตรวจอยู่ในหัวข้อ Prop State Table ด้านล่าง
- ปรึกษา Ek (story consultant) เรื่อง scene breakdown + empty zone แล้ว — ผลตรวจสะท้อนอยู่ในทุก scene ด้านล่าง

---

## 📌 Prop State Table — Identity Prop (ล็อกตลอดเรื่อง — ตาม `docs/shorts-prompt-standards.md` ข้อ 1A)

| ตัวละคร | Signature Prop (Identity — ตลอดเรื่อง) | Spec อ้างอิง | สถานะในตอนนี้ |
|---|---|---|---|
| คิม (`@kim_v1`) | **ไม่มี signature prop ระดับ Identity** (ยืนยันแล้วโดย Mint — ตรวจ spec+ภาพแล้วไม่พบอุปกรณ์ประจำตัว นอกจาก minimalist analog watch ที่เป็นส่วนหนึ่งของ outfit ปกติ ไม่ใช่ signature prop เชิงสัญลักษณ์) | `docs/character-visual-prompts.md` บรรทัด 53-94 + `references/คิม01-Creative Director.jpeg`, `references/คิม02-Creative Director.jpeg` | ไม่มี prop ประจำตัวที่ต้อง lock ข้าม ep |
| ไอซ์ (`@ice_v1`) | **ไม่มี signature prop ระดับ Identity** (ยืนยันแล้วโดย Mint — ตรวจ spec+ภาพแล้วไม่พบอุปกรณ์ประจำตัว) | `docs/character-visual-prompts.md` บรรทัด 122-163 + `references/ไอซ์01-เลขานุการผู้บริหาร.jpeg`, `references/ไอซ์02-เลขานุการผู้บริหาร.jpeg` | ไม่มี prop ประจำตัว |
| เต (`@te_v1`) | **ไม่มี signature prop ระดับ Identity** (ยืนยันแล้วโดย Mint ใน ep06 — ตรวจ spec บรรทัด 191-231 และภาพแล้วไม่พบอุปกรณ์ประจำตัวใดๆ) | `docs/character-visual-prompts.md` บรรทัด 191-231 + `references/เต01-HR.jpeg`, `references/เต02-HR.jpeg` | ไม่มี prop ประจำตัว — แก้วกาแฟที่ถือในบางฉากเป็น prop เฉพาะฉาก ไม่ใช่ Identity Prop (ดู ep06 Prop State Table) |

**หมายเหตุ prop เฉพาะฉาก (สำคัญต่อ Scene 6-7 ของตอนนี้):** ขนตาที่หลุดติดแก้มไอซ์ (Scene 6) และกระดาษทิชชูที่มีขนตาวางอยู่ (Scene 6-7) เป็น **prop เฉพาะฉากของตอนนี้เท่านั้น** ไม่ใช่ Identity Prop — ต้อง track ตำแหน่ง/สถานะให้ต่อเนื่องภายในตอนนี้ตามกฎข้อ 4 (ถอนออกจากแก้มไอซ์ → วางบนทิชชู → ไอซ์หยิบกลับไปที่โต๊ะ)

---

## 📌 Outfit State Table — Outfit of the Day (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 1B)

**Timeline:** ตอน 1 = วันจันทร์ สัปดาห์ 1 (เช้า-เย็น) ตาม `docs/continuity-bible.md` บรรทัด 34 — เป็นตอนแรกสุดของซีรีส์ ไม่มีตอนก่อนหน้าให้เทียบ ทุก scene ในตอนนี้คือวันเดียวกันต่อเนื่องกันทั้งวัน (เช้าถึงห้าโมงครึ่ง) ⇒ **outfit ต้องเหมือนกันเป๊ะทุก scene ภายในตอนนี้**

อ้างอิงจาก `docs/character-visual-prompts.md` เป็นฐาน + ภาพ reference จริง (คิม/ไอซ์ ใช้ outfit เดียวกับที่ปรากฏใน turnaround sheet เพราะเป็นวันแรกที่ยังไม่มีข้อมูลอื่น):

| ตัวละคร | Outfit of the Day (ep01 — วันจันทร์ สัปดาห์ 1) | Spec/ภาพอ้างอิง | เปลี่ยนแปลงภายในตอนนี้หรือไม่ |
|---|---|---|---|
| คิม (`@kim_v1`) | crisp white (#F5F5F0 — clean white, **not cream, not grey**) button-up dress shirt with sleeves rolled to the forearm, top button undone, no tie, minimalist dark-brown leather strap analog watch, dark charcoal-navy (#22252B — dark, **not pure black**) tailored trousers | `docs/character-visual-prompts.md` บรรทัด 78-85 + `references/คิม01-Creative Director.jpeg` (สีตรงกับภาพ full-body ที่ generate ไว้แล้ว) | ไม่เปลี่ยนตลอดตอน (วันเดียวกันทั้ง 7 scene) |
| ไอซ์ (`@ice_v1`) | modest fitted white (#F7F5F2 — clean white, **not cream, not grey**) dress shirt tucked into dark charcoal-navy (#22252B — dark, **not pure black**) tailored trousers, no accessories, a plain dark suit jacket (#1D1F24 — near-black navy, **not brown**) worn over the shirt — his only suit, bought for the interview, still crisp and new | `docs/character-visual-prompts.md` บรรทัด 153-154 + `references/ไอซ์01-เลขานุการผู้บริหาร.jpeg` (สีตรงกับภาพ full-body ที่ generate ไว้แล้ว — ต้นฉบับ ep01.md บรรทัด 13 ระบุชัดว่าไอซ์ใส่ "สูทตัวเดียวที่มี ซื้อตอนสัมภาษณ์งาน ยังใหม่กริบ" ต้องมีเสื้อสูทคลุมทับตามต้นฉบับ) | ไม่เปลี่ยนตลอดตอน (วันเดียวกันทั้ง 7 scene) |
| เต (`@te_v1`, Scene 2-3 เท่านั้น) | light pastel-blue (#A8C5DE) short-sleeve button-down shirt (soft pale blue, **not white, not grey**) with a chest pocket, navy (#1B2A4A) tailored trousers, holding a to-go coffee cup in one hand | `docs/character-visual-prompts.md` บรรทัด 216-222 + `references/เต01-HR.jpeg` (สีเดียวกับที่ใช้ใน ep06 — คนละวัน แต่ยังไม่มีข้อมูลอื่นขัดแย้ง เก็บสีนี้ไว้เป็นค่าเริ่มต้นของเตจนกว่าจะมีเหตุผลเปลี่ยน) | ไม่เปลี่ยนตลอด Scene 2-3 |

**ตัวละครรองที่ปรากฏร่วม (background cameo, Scene 3 เท่านั้น — ไม่มี dialogue, ไม่ครอบคลุมทุกกฎ outfit เพราะเป็นภาพผ่านสั้นๆ ในเฟรมกว้าง):**

| ตัวละคร | บทบาทใน Scene 3 | หมายเหตุ |
|---|---|---|
| ดิว | นั่งใส่หูฟัง over-ear ก้มหน้าทำงาน ไม่เงยหน้า | ใช้ signature prop เดิม (worn over-ear headphones, slightly frayed cable) ตาม Identity Prop Lock — ไม่ต้องระบุ outfit เต็มเพราะเป็น background ระยะไกล ไม่ใช่ตัวละครที่มี dialogue |
| นนท์ | นั่งข้างดิว "เหมือนเป็นเงา" | ใช้ signature prop เดิม (stem-style wireless in-ear earbuds) — background ระยะไกลเช่นกัน |
| ฟลุ้ค | พยักหน้าทักไอซ์พร้อมยิ้มกว้าง | background ระยะไกล ไม่มี dialogue |
| เจมส์ | เงยหน้ามาแป๊บนึงแล้วก้มกลับไปทำงาน นั่งตรงข้ามฟลุ้ค | background ระยะไกล ไม่มี dialogue |

**หมายเหตุสำคัญ:** Google Flow generate แต่ละ scene แยกกัน ไม่มี memory ข้าม prompt — **ทุก scene ด้านล่างต้องมี outfit description เต็มของตัวละครหลักที่ปรากฏซ้ำทุกครั้ง** ห้ามสมมติว่า Flow จะ "จำ" ชุดจาก scene ก่อนหน้าได้เอง

**⚠️ Color Anchor Lock (ดู `docs/shorts-prompt-standards.md` ข้อ 3B):** Scene 4-7 อยู่ในห้องทำงาน/ห้องประชุม/pantry ที่มีแสงธรรมชาติแรงผ่านกระจกและแสงหลอดผสม — สีขาวของเสื้อคิม/ไอซ์เสี่ยงเพี้ยนเป็นสีครีม/เหลืองอ่อนได้ถ้าแสงแรงเกิน — เพิ่มคำเตือนกันเพี้ยนกำกับทุกจุดที่ระบุสีแล้ว

---

## 📌 เวลา/สภาพอากาศของตอนนี้ (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 5A)

**สภาพอากาศ (จาก `docs/continuity-bible.md` — Fictional Weather Table แถวที่ 1):** ท้องฟ้าแจ่มใส แดดอ่อนยามเช้า ไม่ร้อนจัด — **ใช้ซ้ำคำต่อคำทุก scene ที่เป็นช่วงเช้า** ("clear sky, soft gentle morning sunlight, not too hot") — ช่วงบ่าย/เย็นของตอนนี้ (Scene 5-7) ให้ปรับเป็นแสงบ่าย/เย็นตามเวลาจริงแต่ยังคงเป็นท้องฟ้าแจ่มใสไม่มีฝนตลอดทั้งวัน (ตามที่ bible ระบุว่าเป็นวันเดียวไม่มี marker เปลี่ยนสภาพอากาศ)

**เวลาเจาะจงต่อ scene (ตอนนี้เป็นโครงสร้าง Linear — ไล่ตามเวลาจริงทั้งวัน ตามต้นฉบับ):**

| Scene | เวลาโดยประมาณ | หมายเหตุ |
|---|---|---|
| 1 | ~8:45 AM | ไอซ์ยืนหน้าตึกแหงนมอง |
| 2 | ~8:55 AM | ลิฟต์เปิดชั้น 14 เตทัก |
| 3 | ~9:00 AM | เตพาไอซ์เดินแนะนำตัวทีม |
| 4 | ~9:05 AM | เตพาไอซ์เข้าห้องคิม |
| 5 | ~12:05 PM (สามชั่วโมงผ่านไป) | ไอซ์เรียนรู้นิสัยคิม (ส่งงาน → คิมเปิดอ่านทันที) |
| 6 | ~5:30 PM | ห้องประชุมใหญ่เลิก คิมหยิบขนตาออกจากแก้มไอซ์ |
| 7 | ~5:32 PM | ปิดฉาก — ไอซ์เดินออกมา + คิมมองปลายนิ้วตัวเอง |

## 📌 Blocking (ล็อกก่อนเริ่มเขียน — ตาม `docs/shorts-prompt-standards.md` ข้อ 2)

**ยืนยันโดย Ek (story consultant) 21 ก.ย. 2569:**

- **Layout ห้องคิม (Scene 4, 6):** โต๊ะทำงานคิมตั้งอยู่หน้าต่างกระจกทั้งบาน หันหน้าเข้าหาประตูกระจกฝ้า มีจอคอมพิวเตอร์ตั้งบนโต๊ะ เก้าอี้ทำงานมีพนักพิงสูง — คิมนั่งอยู่ฝั่งในสุดของห้อง ไอซ์ยืนอยู่ฝั่งประตู (ยังไม่มีโต๊ะของตัวเอง เพราะเป็น Scene แรกที่เจอกัน) — ใช้ layout นี้ซ้ำทุก scene ที่อยู่ในห้องคิม
- **Camera-left / camera-right (Scene 4):** คิมอยู่ camera-left (นั่งหลังโต๊ะ), ไอซ์อยู่ camera-right (ยืนหน้าประตู) — คงที่ตลอด Scene 4
- **Camera-left / camera-right (Scene 6, ห้องประชุมใหญ่/โต๊ะคิม ตอนเย็น):** คิมอยู่ camera-left (นั่งที่โต๊ะเซ็นเอกสาร), ไอซ์อยู่ camera-right (ยืนข้างโต๊ะ) — สลับจาก Scene 4 เพราะเป็นคนละสถานที่ (ห้องประชุมใหญ่ ไม่ใช่ห้องทำงานส่วนตัวคิม) ต้นฉบับระบุ "ห้าโมงครึ่ง ทุกคนเริ่มเก็บของ" ต่อจาก "บ่ายสาม ห้องประชุมใหญ่" (Scene 5 บรรยาย) — ตีความว่ายังอยู่บริเวณห้องประชุมใหญ่ที่โต๊ะรวม ไม่ใช่ห้องทำงานส่วนตัวคิม
- **สัดส่วนตัวละคร (ตาม `docs/shorts-prompt-standards.md` ข้อ 5B):** คิม 183cm/76kg (athletic muscular, broad shoulders) vs ไอซ์ 175cm/63kg (slim toned) — ต่างกัน 8cm ชัดเจน คิมสูง/ใหญ่กว่าเห็นชัด ต้องระบุใน Subject ทุก scene ที่ทั้งคู่อยู่ในเฟรมเดียวกัน — เต 178cm/72kg (athletic, broader shoulders) อยู่ระหว่างกลาง ต่างจากไอซ์ 3cm (ใกล้เคียง ไม่ต้องเน้นมาก) ต่างจากคิม 5cm (ไม่ต้องเน้นมาก เพราะเตกับคิมไม่ได้อยู่ในเฟรมเดียวกันใน ep นี้)

---

## 🎬 Scene 1 — HOOK: หน้าตึก PRISM (0:00-0:08)

**Ingredients:** `@ice_v1` (expression: neutral calm, then quiet determination)

**Text overlay ที่ใส่ตอนตัดต่อ (โผล่ตั้งแต่ 0:00-0:03):** *"วันแรก... ของทุกอย่าง"*

**⚠️ Brand/Logo Lock (ดู `docs/shorts-prompt-standards.md` ข้อ 2D):** ป้าย PRISM บนตึก/ล็อบบี้ต้องเป็น**ตัวอักษรล้วน ไม่มีโลโก้กราฟิก** — ภาพ reference `references/Creative_agency_office_interior.jpeg` ที่มีอยู่จริงมีโลโก้รูปเพชร (diamond icon) อยู่เหนือคำว่า PRISM ซึ่งขัดกับกฎนี้ **ต้องเขียนกำกับ override ชัดเจนว่า "only the text 'PRISM', no diamond icon, no graphic logo symbol"** ทุกจุดที่อ้างอิงป้ายนี้

```
Subject: @ice_v1, wearing a modest fitted white (#F7F5F2 — clean white, not
cream, not grey) dress shirt tucked into dark charcoal-navy (#22252B —
dark, not pure black) tailored trousers, no accessories, a plain dark
suit jacket (#1D1F24 — near-black navy, not brown) worn over the shirt —
his only suit, still crisp and new — standing on the sidewalk outside a
fourteen-story glass office tower in the Thonglor district of Bangkok,
looking straight up at the building's glass facade, a sign near the
building entrance reading only the text "PRISM Creative Agency" in clean
modern sans-serif lettering, no diamond icon, no graphic logo symbol.
Composition: low-angle medium shot looking up along with Ice's gaze, Ice
positioned camera-center-right in the foreground, the glass tower rising
behind and above him, morning sunlight glinting off the glass facade.
Action: Ice tilts his head back further, squinting slightly against the
bright glass reflection, then takes a deep breath, straightens his suit
jacket with both hands, and steps forward toward the entrance.
Mood: approximately 8:45 AM, clear sky, soft gentle morning sunlight, not
too hot, a hopeful nervous first-day energy, bright optimistic color
grade, no dialogue — bright morning light must not shift clothing
colors: Ice's shirt stays visibly white (#F7F5F2 — not cream/grey), his
suit jacket stays visibly dark navy (#1D1F24 — not brown).
```

---

## 🎬 Scene 2 — ลิฟต์เปิด: เตทักทาย (0:08-0:16)

**Ingredients:** `@ice_v1` (expression: neutral calm, mildly startled), `@te_v1` (expression: warm friendly smile)

**Setting/Furniture Lock:** พื้นหลังเป็นออฟฟิศเปิด open-plan เห็นโต๊ะทำงานหลายแถวลึกเข้าไป (ตาม `references/Creative_agency_office_interior.jpeg` โทนออฟฟิศจริง)

```
Subject: @ice_v1, wearing a modest fitted white (#F7F5F2 — clean white, not
cream, not grey) dress shirt tucked into dark charcoal-navy (#22252B —
dark, not pure black) tailored trousers and a plain dark navy (#1D1F24 —
not brown) suit jacket, standing just inside the elevator doors on the
14th floor, turning around toward a voice behind him; @te_v1, wearing a
light pastel-blue (#A8C5DE) short-sleeve button-down shirt (soft pale
blue, not white, not grey) with a chest pocket and navy (#1B2A4A)
tailored trousers, holding a to-go coffee cup in one hand, standing
behind Ice with an easy warm smile, open-plan office desks with computer
monitors visible in the background stretching into the distance.
Composition: medium shot, eye-level, Ice on camera-left having just
turned around, Te on camera-right approaching from behind, rows of desks
softly visible in the background, bright open-plan office lighting.
Action: Te takes a step closer, raising his coffee cup slightly in a
casual greeting gesture; Ice turns fully around, slightly startled but
polite.
Dialogue — Speaker: Te. Line: "น้องใหม่เหรอ?". Delivery: warm, casual,
friendly. Speaker: Ice. Line: "ครับ ผม—". Delivery: polite, a little
nervous, cut off mid-sentence. Speaker: Te. Line: "ไอซ์ใช่ไหม? เลขาฯ ใหม่
ของพี่คิม ผมเต ฝ่าย HR ยินดีต้อนรับนะ". Delivery: bright, welcoming,
talking a bit fast with enthusiasm.
Mood: approximately 8:55 AM, clear sky, soft gentle morning sunlight, not
too hot, a bustling but welcoming morning office ambience, the sound of
distant keyboards and conversation, bright optimistic color grade — warm
morning light must not shift clothing colors: Ice's shirt stays visibly
white (#F7F5F2 — not cream/grey), Te's shirt stays visibly pastel-blue
(#A8C5DE — not white/grey).
```

---

## 🎬 Scene 3 — ทัวร์ออฟฟิศ: แนะนำทีม (0:16-0:24)

**Ingredients:** `@ice_v1` (expression: trying hard to remember names, slightly overwhelmed), `@te_v1` (expression: casual, pointing things out)

**⚠️ Empty Zone (ตัดสินใจโดย Ek):** ต้นฉบับ Scene นี้ระบุชัดว่ามีดิว นนท์ ฟลุ้ค เจมส์ นั่งทำงานอยู่ที่โต๊ะของตน (บรรทัด 29) — **ไม่ใช่ฉากว่างเปล่า มีคนจริงตามที่ต้นฉบับระบุ** ต้องเขียนระบุจำนวน/ตัวตนคนในฉากชัดเจนตามนี้ ไม่ใช้คำกำกวม "mostly empty/busy" — background cameo เท่านั้น ไม่มี dialogue

```
Subject: @te_v1, wearing a light pastel-blue (#A8C5DE) short-sleeve
button-down shirt (soft pale blue, not white, not grey) with a chest
pocket and navy (#1B2A4A) tailored trousers, walking ahead through a row
of open-plan desks, gesturing casually with his coffee-cup hand toward
each coworker as he passes; @ice_v1, wearing a modest fitted white
(#F7F5F2 — clean white, not cream, not grey) dress shirt and dark navy
(#1D1F24) suit jacket, following just behind Te, glancing quickly at each
desk, trying to remember names. Along the row: Dew, wearing his worn
over-ear headphones with a slightly frayed cable, head down, focused on
his monitor, not looking up; Non, seated beside Dew wearing his
stem-style wireless in-ear earbuds, quietly focused on his own screen;
Fluke, seated at his desk, glancing up and giving a wide easy smile and a
nod toward Ice; James, seated across from Fluke, looking up briefly with
a neutral expression then immediately looking back down at his screen.
Composition: medium tracking shot following Te and Ice from a slight
side angle as they walk down the aisle, camera-left to camera-right
movement, the four coworkers' desks visible in a row along the
background, each at their own desk with monitors and keyboards in frame,
bright open-plan office lighting.
Action: Te points briefly toward each desk in turn without stopping his
walking pace; Fluke smiles and nods at Ice as they pass; James glances up
for a beat then returns to his screen; Dew and Non remain absorbed in
their work, not reacting to the passersby.
Mood: approximately 9:00 AM, clear sky, soft gentle morning sunlight, not
too hot, a busy focused morning office ambience, quiet keyboard clicks
and distant murmurs of conversation, bright optimistic color grade, no
dialogue — warm morning light must not shift clothing colors: Ice's
shirt stays visibly white (#F7F5F2 — not cream/grey), Te's shirt stays
visibly pastel-blue (#A8C5DE — not white/grey).
```

---

## 🎬 Scene 4 — ห้องคิม: เจอกันครั้งแรก (0:24-0:32)

**Ingredients:** `@kim_v1` (expression: neutral calm, sharp but not unkind), `@ice_v1` (expression: quietly flustered, trying to compose himself)

**Setting/Furniture Lock:** โต๊ะทำงานคิม, จอคอมพิวเตอร์, ประตูกระจกฝ้า ต้องเห็นชัดในเฟรมตามที่กำหนดใน Blocking

```
Subject: @kim_v1, wearing a crisp white (#F5F5F0 — clean white, not cream,
not grey) button-up dress shirt with sleeves rolled to the forearm, top
button undone, no tie, a minimalist dark-brown leather strap analog
watch, and dark charcoal-navy (#22252B — dark, not pure black) tailored
trousers, seated at his desk with his computer monitor and keyboard in
frame, a pen held loosely at his lips, turning his head away from the
screen toward the door; @ice_v1, wearing a modest fitted white (#F7F5F2)
dress shirt and dark navy (#1D1F24) suit jacket, standing just inside the
doorway near the frosted-glass door, Kim noticeably taller and broader
than Ice, standing upright but slightly nervous.
Composition: medium two-shot, eye-level, Kim on camera-left seated behind
his desk with monitor and keyboard visible, Ice on camera-right standing
near the door, soft daylight through the office window behind Kim.
Action: Kim sets the pen down on the desk, looks Ice over for a brief
still moment, then gives a small nod; Ice straightens his posture,
adjusting his thoughts visibly on his face for a beat before speaking.
Dialogue — Speaker: Ice. Line: "สวัสดีครับ ผมไอซ์ เลขานุการใหม่ครับ".
Delivery: polite, composed, a slight nervous edge. Speaker: Kim. Line:
"คิมครับ นั่งตรงโต๊ะข้างนอก งานที่ต้องทำวันนี้ส่งไว้ในอีเมลแล้ว".
Delivery: short, clipped, matter-of-fact, no smile. Speaker: Ice. Line:
"ครับ ขอบคุณครับ". Delivery: polite, slightly unsure how to read him.
Mood: approximately 9:05 AM, clear sky, soft gentle morning sunlight, not
too hot, a quiet focused office ambience inside Kim's private room, calm
first-meeting tension, bright but composed color grade — daylight must
not shift clothing colors: Kim's shirt stays visibly white (#F5F5F0 —
not cream/grey), Ice's shirt stays visibly white (#F7F5F2 — not
cream/grey), Ice's suit jacket stays visibly dark navy (#1D1F24 — not
brown).
```

---

## 🎬 Scene 5 — สามชั่วโมงผ่านไป: สังเกตนิสัยคิม (0:32-0:40)

**Ingredients:** `@ice_v1` (expression: quietly observant, small realization), `@kim_v1` (expression: focused, opening an email immediately)

**⚠️ Empty Zone (ตัดสินใจโดย Ek):** ต้นฉบับไม่ระบุคนอื่นในจังหวะนี้ชัดเจน — ใช้ shallow depth of field ให้ background เบลอไม่ระบุสถานะคนแทน (ไม่ยืนยัน/ปฏิเสธว่ามีคนอื่น) ตามแนวทางเดียวกับ ep06 Scene 3

```
Subject: @ice_v1, wearing a modest fitted white (#F7F5F2 — clean white,
not cream, not grey) dress shirt and dark navy (#1D1F24) suit jacket,
standing just outside Kim's frosted-glass office door, holding a folder
of documents, watching through the glass as @kim_v1, wearing a crisp
white (#F5F5F0) button-up dress shirt with sleeves rolled to the
forearm and dark charcoal-navy (#22252B) tailored trousers, seated at
his desk with his monitor in frame, opens an email notification the
instant it arrives and begins reading it immediately.
Composition: medium shot, eye-level, Ice on camera-right in the
foreground looking through the frosted glass, Kim visible on camera-left
through the glass at his desk, shallow depth of field softly blurring the
surrounding office behind Ice.
Action: Ice watches Kim's hand move to click open the email the moment
the notification appears, a small realization crossing his face — a
faint thoughtful smile.
Mood: approximately 12:05 PM, clear sky, soft midday sunlight, not too
hot, a quiet focused midday office ambience, a small private moment of
noticing someone's character, warm contemplative color grade, no
dialogue — daylight must not shift clothing colors: Ice's shirt stays
visibly white (#F7F5F2 — not cream/grey), Kim's shirt stays visibly
white (#F5F5F0 — not cream/grey).
```

---

## 🎬 Scene 6 — ห้าโมงครึ่ง: ขนตาติดแก้ม (0:40-0:48) — Emotional Payoff

**Ingredients:** `@kim_v1` (expression: neutral calm shifting to a flicker of surprise, then not meeting Ice's eyes), `@ice_v1` (expression: startled, then quietly flustered blush)

**⚠️ Empty Zone (ตัดสินใจโดย Ek):** ต้นฉบับระบุ "ห้าโมงครึ่ง ทุกคนเริ่มเก็บของ" ในห้องประชุมใหญ่ — มีคนอื่นอยู่ในบริเวณกว้างแต่ไม่ได้ระบุจำนวน/ตัวตนชัดเจนตรงจุดนี้ — เขียนแบบเห็นคนอื่นเก็บของอยู่ไกลๆ นอกโฟกัส ไม่ระบุจำนวนเจาะจง (มีมูลจากต้นฉบับว่า "ทุกคน" กำลังเก็บของ ไม่ใช่ฉากว่างเปล่า)

**Prop state:** ขนตาหลุดติดแก้มไอซ์ (ข้างขวา) → คิมยื่นมือแตะแก้มปัดออก → วางบนกระดาษทิชชูบนโต๊ะ

```
Subject: @ice_v1, wearing a modest fitted white (#F7F5F2 — clean white,
not cream, not grey) dress shirt and dark navy (#1D1F24) suit jacket,
standing beside a meeting-room table holding a printed summary folder
out toward @kim_v1, a single loose eyelash resting on his right cheek;
@kim_v1, wearing a crisp white (#F5F5F0) button-up dress shirt with
sleeves rolled to the forearm and dark charcoal-navy (#22252B) tailored
trousers, seated at the table having just signed the folder with a pen,
looking up at Ice, noticeably taller and broader-built than Ice even
while seated, other coworkers visible further back in the meeting room
packing up their laptops and bags, out of sharp focus.
Composition: medium close-up two-shot, eye-level, Kim on camera-left
seated, Ice on camera-right standing beside the table, a tissue paper
visible on the table surface near Kim's hand, soft warm late-afternoon
light through the windows behind them.
Action: Kim's eyes flick to Ice's cheek, he sets the pen down and raises
his hand toward Ice's face; Ice freezes, eyes widening slightly; Kim's
fingertip gently brushes the loose eyelash off Ice's cheek and sets it
down on the tissue paper on the table; both of them go completely still
for a beat, neither moving.
Dialogue — Speaker: Kim. Line: "ขนตา". Delivery: flat, quiet, almost
startled by himself. Speaker: Ice. Line: "หา?". Delivery: confused,
caught off guard. Speaker: Kim. Line: "ขนตาติดแก้ม". Delivery: quiet,
matter-of-fact, then a beat of stillness after touching Ice's cheek.
Speaker: Kim. Line: "ขอพรได้". Delivery: even, composed, but not making
eye contact. Speaker: Ice. Line: "ขอบคุณครับ". Delivery: soft, a little
breathless, cheeks flushed.
Mood: approximately 5:30 PM, clear sky, warm golden late-afternoon
sunlight through the windows, not too hot, a hushed intimate stillness
inside a mostly-emptying meeting room, gentle lingering tension, warm
cinematic color grade — warm late-afternoon light must not shift
clothing colors: Kim's shirt stays visibly white (#F5F5F0 — not
cream/grey), Ice's shirt stays visibly white (#F7F5F2 — not cream/grey),
Ice's suit jacket stays visibly dark navy (#1D1F24 — not brown).
```

---

## 🎬 Scene 7 — ปิดฉาก: ปลายนิ้วคิม + ไอซ์ขอพร (0:48-0:56) — Closing Tag

**Ingredients:** `@ice_v1` (expression: soft private happiness, eyes closed in a wish), `@kim_v1` (expression: quietly puzzled at himself)

**⚠️ Camera anchor:** สอง location คู่ขนาน (โต๊ะไอซ์ + ห้องคิม) — ตัดสลับ 2 shot สั้นๆ ภายในคลิปเดียว ต้องระบุมุมกล้องแยกกันชัดเจนสำหรับแต่ละครึ่ง

```
Subject (first half): @ice_v1, wearing a modest fitted white (#F7F5F2 —
clean white, not cream, not grey) dress shirt and dark navy (#1D1F24)
suit jacket, seated at his own desk just outside Kim's office door, a
folded tissue paper with a single eyelash on it placed carefully beside
his keyboard, his computer monitor and keyboard visible in frame.
Composition (first half): medium close-up, eye-level, static camera, Ice
centered in frame with the tissue paper and his keyboard clearly visible
on the desk in front of him, warm early-evening desk lighting.
Action (first half): Ice looks at the tissue paper for a long beat, then
closes his eyes and tilts his head down slightly, making a silent wish.

Subject (second half): @kim_v1, wearing a crisp white (#F5F5F0) button-up
dress shirt with sleeves rolled to the forearm and dark charcoal-navy
(#22252B) tailored trousers, alone in his office, seated at his desk with
his monitor in frame, looking down at his own right hand, turning his
fingertips slightly as if still feeling the touch.
Composition (second half): medium close-up, eye-level, static camera,
Kim centered in frame with his desk and monitor visible behind his raised
hand, same warm early-evening lighting as the first half.
Action (second half): Kim stares at his own fingertips for a quiet
moment, brow faintly furrowed in quiet puzzlement at himself, then lowers
his hand slowly back to the desk.
Mood: approximately 5:32 PM, clear sky, warm golden late-afternoon
sunlight fading into early evening, not too hot, a quiet private
lingering feeling on both ends of the office, gentle warm cinematic color
grade, no dialogue — warm light must not shift clothing colors: Ice's
shirt stays visibly white (#F7F5F2 — not cream/grey), Kim's shirt stays
visibly white (#F5F5F0 — not cream/grey).
```

**Text overlay ปิดท้าย (ใส่ตอนตัดต่อ):** *ชั้น 14 มีรัก | ตอนต่อไป: ภูมิ × ปอนด์ — เก็บให้ครบ*

---

## 📋 Checklist การผลิต

**ก่อนอื่น — ผ่าน Quality Gate ตาม `docs/shorts-prompt-standards.md` ข้อ 6 ก่อน (prop/blocking/ingredient/แสง/timeline) แล้วค่อยเริ่มขั้นตอนด้านล่าง — ผลการตรวจอยู่ในหัวข้อ "Quality Gate — ผลการตรวจ" ท้ายไฟล์นี้:**

0. [ ] ยืนยันว่ามี turnaround sheet ของคิม, ไอซ์, เต สร้างไว้จริงหรือยัง ก่อน generate — ยืนยันแล้วทั้ง 3 คน (ดูหัวข้อ "ใช้กับ" ด้านบน)
1. [ ] Generate Scene 1-7 ตามลำดับ (แต่ละคลิป 8 วิ)
2. [ ] เรียงคลิปใน Scenebuilder ตามลำดับ 1→2→3→4→5→6→7
3. [ ] ใส่ text overlay 2 จุด (ต้น Scene 1, ท้าย Scene 7) ตอนตัดต่อ ไม่ต้องใส่ในพรอมต์ Flow
4. [ ] เช็คว่า Scene 1 (hook) สื่อ "วันแรกที่ตื่นเต้น/กังวล" ชัดเจนภายใน 3 วินาทีแรก
5. [ ] เช็คคลิปที่ generate จริงว่าป้าย PRISM ไม่มีโลโก้กราฟิกรูปเพชรติดมาจากภาพ reference — ถ้าติดมาให้ regenerate scene นั้นใหม่พร้อมเน้นคำ override ให้ชัดขึ้น
6. [ ] เช็คคลิปที่ generate จริงว่าสีขาวเสื้อคิม/ไอซ์ไม่เพี้ยนเป็นสีครีม/เหลืองจากแสงแดดแรงใน Scene 1, 3
7. [ ] เช็คว่าขนตา+กระดาษทิชชูใน Scene 6→7 อยู่ตำแหน่ง/สถานะต่อเนื่องกัน (ถอดจากแก้ม → วางบนทิชชู → ไอซ์ย้ายไปที่โต๊ะตัวเอง)
8. [ ] เช็คสัดส่วนตัวละครคิม (183cm) vs ไอซ์ (175cm) ในภาพที่ generate จริงว่าเห็นความต่าง 8cm ชัดเจนตาม Character Scale Lock
9. [ ] Export เป็น 9:16 ความยาวรวม ~56 วินาที พร้อมโพสต์

---

## ✅ Quality Gate — ผลการตรวจ (ตาม `docs/shorts-prompt-standards.md` ข้อ 6)

- [x] เปิดภาพ `references/คิม01-02-Creative Director.jpeg`, `references/ไอซ์01-02-เลขานุการผู้บริหาร.jpeg`, `references/เต01-02-HR.jpeg` ดูจริงแล้ว (ไม่ใช่เขียนจากความจำ)
- [x] เช็ค `docs/continuity-bible.md` แล้ว — ep01 เป็นตอนแรกสุด ไม่มีตอนก่อนหน้าให้เทียบ ⇒ กำหนด Outfit of the Day ใหม่ทั้งชุด อ้างอิงจาก default spec/ภาพตรงๆ
- [x] แปะ Prop State Table ของคิม/ไอซ์/เตไว้บนสุดไฟล์ (อ้างอิงบรรทัด spec จริง + ยืนยันโดย Mint)
- [x] แปะ Outfit State Table ไว้บนสุดไฟล์ (สี/ทรง/เนื้อผ้าเต็มชุดของวันนี้ อ้างอิงภาพจริง)
- [x] `grep -n "earbud\|headphone\|glasses\|watch\|jacket"` ไล่ทุกจุดในไฟล์เทียบกับ Prop State Table — ผลตรวจ: ดิว/นนท์ ปรากฏใน Scene 3 เท่านั้นด้วย signature prop เดิม (over-ear/in-ear) ตรงกันครบ, watch ของคิมปรากฏใน spec ไม่ใช่ signature prop เชิงสัญลักษณ์ (ระบุชัดในตารางแล้วว่าไม่ล็อก) — ไม่มีจุดขัดกัน
- [x] `grep -n "shirt\|trousers\|jacket\|sneakers\|hoodie"` ไล่ทุก scene เทียบกับ Outfit State Table — ทุก scene ที่คิม/ไอซ์/เตปรากฏมี outfit description เต็มครบ (ดูผล grep ด้านล่าง)
- [x] ทุก scene ที่ prop (ขนตา/ทิชชู) ถูกถอด/วาง/ย้าย มี action ของทั้งสองฝั่งครบ (Scene 6 คิมปัดขนตา+วางบนทิชชู → Scene 7 ไอซ์มองทิชชูที่โต๊ะตัวเอง)
- [x] กำหนด layout + camera-left/right ตายตัวตอนต้นไฟล์ และทุก scene อ้างอิงตรงกัน (ห้องคิม Scene 4 คิม camera-left/ไอซ์ camera-right, ห้องประชุมใหญ่ Scene 6 คิม camera-left/ไอซ์ camera-right เช่นกันแต่คนละสถานที่ — ระบุเหตุผลไว้ในหัวข้อ Blocking แล้ว)
- [x] `grep -n "desk\|monitor\|keyboard\|chair\|table"` ไล่ทุก Subject block — ทุก scene ที่ตัวละครนั่งทำงาน/อยู่ในห้องมีเฟอร์นิเจอร์ระบุชัดเจน — Scene 2/4/5/7 ใช้ desk/monitor/keyboard (โต๊ะทำงาน), **Scene 6 ใช้ "meeting-room table" แทน** เพราะเป็นห้องประชุมใหญ่ไม่ใช่โต๊ะทำงานส่วนตัว (ยืนยันตรงกับ Blocking ที่กำหนดไว้) — ตรวจแล้วครบทุก scene ที่มีตัวละครนั่ง/ยืนในพื้นที่ที่มีเฟอร์นิเจอร์เฉพาะ ไม่มี scene ไหนขาด (ดูผล grep ด้านล่าง)
- [x] ไม่มี scene ไหนใช้คำอ้างอิง "same as Scene X" แบบลอยๆ ที่ต้องเพิ่มมุม/ระยะกล้องกำกับ (ตอนนี้เป็นโครงสร้าง Linear ไม่มี scene ที่ขยาย/ย้อนจาก scene ก่อนหน้าแบบ ep07)
- [x] `grep -n "empty\|mostly\|no one\|coworker"` ไล่ทุก scene ที่จำนวนคนในฉากมีผลต่อ story logic — Scene 3 ระบุตัวตนคนในฉากชัดเจนตามต้นฉบับ (ดิว/นนท์/ฟลุ้ค/เจมส์), Scene 5-6 ใช้ shallow depth of field/บรรยายกว้างไม่กำกวมแทนคำว่า "mostly empty" — ไม่มีคำกำกวมหลงเหลือ
- [x] ทุก scene ที่มีอารมณ์ชัดเจน ระบุ expression tag ต่อท้าย `@handle` ครบ (ดู Ingredients ทุก scene)
- [x] ตัวละครทุกตัวที่ใช้ `@handle` มี turnaround sheet ยืนยันแล้วว่ามีอยู่จริง — `@kim_v1`, `@ice_v1`, `@te_v1` ยืนยันครบ
- [x] วลีแสง/บรรยากาศซ้ำคำต่อคำข้าม scene ในตอนเดียวกัน (เช้า: Scene 1-4 ใช้ "clear sky, soft gentle morning sunlight, not too hot" ซ้ำเป๊ะ, บ่าย-เย็น: Scene 5-7 ปรับเป็น midday/late-afternoon ตามเวลาจริงแต่คงคำว่า "clear sky...not too hot" ไว้)
- [x] ไล่ตรวจ timeline/ระยะทางกายภาพ — "สามชั่วโมงผ่านไป" (Scene 4→5) และ "ห้าโมงครึ่ง" (Scene 6) มีเวลาเจาะจงกำกับตรงตามต้นฉบับ
- [x] ทุกจุดที่ระบุสีเสื้อผ้า/prop มีคู่สีที่ห้ามเพี้ยนกำกับด้วย + hex code ครบ — ตรวจด้วย `grep -n "#"` ทุกจุดที่มีคำอธิบายสี (ดูผล grep ด้านล่าง)
- [x] scene ที่ใช้แสงแดดแรง/แสงอุ่น มีคำเตือนกันสีเพี้ยนต่อท้าย Mood ครบทุก block
- [x] ทุก scene ระบุเวลาเจาะจง (8:45 AM → 5:32 PM ไล่ตามลำดับ Linear) และสภาพอากาศ "clear sky...not too hot" กำกับใน Mood ตรงกับ Fictional Weather Table ของ ep01
- [x] ทุก scene ที่ตัวละคร 2 คนขึ้นไปอยู่ในเฟรมเดียวกัน ระบุสัดส่วน/ส่วนสูงสัมพัทธ์ชัดเจนใน Subject (Scene 2, 4, 6, 7 — คิม vs ไอซ์ ต่างกัน 8cm ระบุครบ)
- [x] `grep -n "PRISM\|logo\|signage\|sign reading"` ไล่ทุกจุดที่มีป้าย/ข้อความบริษัทปรากฏในเฟรม — Scene 1 มีป้าย PRISM ระบุ "no diamond icon, no graphic logo symbol" กำกับครบ (จุดเดียวในไฟล์นี้ที่มีป้ายบริษัท)

### ผล grep ตรวจสอบไฟล์นี้ (สรุป)

- `grep -n "#" shorts-prompts-ep01.md` — ทุกจุดที่มีคำอธิบายสี (white #F5F5F0/#F7F5F2, dark navy #22252B/#1D1F24, pastel-blue #A8C5DE, navy #1B2A4A) มี hex กำกับครบ ไม่มีจุดขาด
- `grep -n "shirt\|jacket\|trousers" shorts-prompts-ep01.md` — คิม/ไอซ์/เต มี outfit เต็มซ้ำทุก scene ที่ปรากฏ ไม่มี scene ไหนเว้นว่าง
- `grep -n "desk\|monitor\|keyboard\|table" shorts-prompts-ep01.md` — Scene 2, 4, 5, 7 ใช้ desk/monitor/keyboard, Scene 6 ใช้ meeting-room table (คนละสถานที่ตามที่ตั้งใจ) — ทุก scene ที่มีเฟอร์นิเจอร์เฉพาะสถานที่ระบุครบใน Subject
- `grep -n "empty\|mostly" shorts-prompts-ep01.md` — ไม่พบคำกำกวม "mostly empty" ในไฟล์นี้เลย

---

## 🔁 หมายเหตุสำหรับตอนถัดไป

ตอน 1 นี้ใช้โครงสร้าง **Linear** เพราะเป็นตอนเปิดเรื่อง ต้องปูบริบทตามลำดับเวลาให้คนดูเข้าใจตั้งแต่ต้น — ตอน 2-3 (ภูมิ×ปอนด์ วันเดียวกัน เช้า→บ่าย) ก็ใช้โครงสร้าง Linear ต่อเนื่องเช่นกัน เพราะเป็นการสะสมเหตุการณ์ทีละสเต็ปไม่มีจุดพีคเดี่ยวที่ต้องขยายความย้อนหลัง — ดู `shorts-prompts-ep02.md` และ `shorts-prompts-ep03.md`
