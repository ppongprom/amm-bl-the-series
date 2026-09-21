# ชั้น 14 มีรัก — Environment Reference Prompts (อ้างอิงตามเนื้อเรื่องจริงแต่ละ ep)

**วัตถุประสงค์:** ไฟล์นี้เสริมจาก environment-reference-prompts.md (ที่มี pantry / หน้าห้องประชุม / ในห้องประชุม / ลิฟต์ / หน้าลิฟต์ / สวนลุมพินี อยู่แล้ว) — เก็บ**สถานที่ใหม่ที่ยังไม่เคยทำ prompt** ซึ่งปรากฏจริงในตอนที่ 1-9 ที่เขียนไปแล้ว โดยดึงรายละเอียดจากเนื้อเรื่องจริงมาใส่ในพรอมต์ ไม่ใช่เดาเอาเอง เพื่อให้ภาพที่ generate ตรงกับสิ่งที่เขียนไว้แล้ว 100%

**ใช้กับ:** Google Flow (Ingredients to Video) — ไม่มีคนในเฟรมทุกภาพ เพื่อใช้เป็น Environment Ingredient คู่กับ Character Ingredient

## 🗺️ ตารางดัชนี: แต่ละ ep ใช้สถานที่ไหนบ้าง

| **ตอน** | **สถานที่ที่ปรากฏ** | **อยู่ในไฟล์ไหน** |
|----|----|----|
| ep01 | หน้าตึก PRISM (ภายนอก), ล็อบบี้ลิฟต์ชั้น 14, ห้องคิม, โต๊ะไอซ์, โซน Creative, ห้องประชุมใหญ่ | ไฟล์นี้ (ใหม่) + environment-reference-prompts.md (ห้องประชุมใหญ่) |
| ep02 | โต๊ะภูมิ-ปอนด์ (Strategy) | ไฟล์นี้ (ใหม่) |
| ep03 | Pantry ชั้น 14, ร้านข้าวแกงปากซอย, ร้านกาแฟข้างตึก | environment-reference-prompts.md (pantry) + ไฟล์นี้ (ร้านข้าวแกง/ร้านกาแฟ) |
| ep04 | โซน Creative, ห้องประชุมเล็ก | ไฟล์นี้ (ใหม่) |
| ep05 | ร้านอาหารญี่ปุ่นปากซอยทองหล่อ, ถนนทองหล่อตอนกลางคืน, สถานี BTS ทองหล่อ, ในตู้รถไฟ BTS | ไฟล์นี้ (ใหม่) |
| ep06 | โซน Creative, มุม HR (โต๊ะเต), โต๊ะแทน (IT) | ไฟล์นี้ (ใหม่) |
| ep07 | โซน Creative ตอนดึก, ห้องเซิร์ฟเวอร์, ห้องคิม (เย็น) | ไฟล์นี้ (ใหม่) |
| ep08 | ห้องประชุมใหญ่, โต๊ะไอซ์, ห้องคิม | environment-reference-prompts.md + ไฟล์นี้ |
| ep09 | ล็อบบี้ชั้นล่าง, ซอยทองหล่อตอนฝนตก, สถานี BTS ทองหล่อ (เย็น/ฝน) | ไฟล์นี้ (ใหม่) |

## ⚠️ อัปเดต v2 (20 ก.ย.) — ทำไมภาพที่ได้ไม่สมจริง/ไม่ตรง prompt

จากภาพทดสอบที่ได้ (server room ออกมาเป็นภาพตึกภายนอก, โต๊ะไอซ์ดูเล็ก/ไม่สมฐานะ) วิเคราะห์แล้วเจอ 2 ปัญหาหลัก ที่จริงๆ **กระทบทุก prompt ในไฟล์นี้ ไม่ใช่แค่ 2 อันที่ทดสอบ:**

1.  **Master Block เดิมขึ้นต้นด้วยคำอธิบาย "ตึกกระจก 14 ชั้น...สะท้อนท้องฟ้า" ทุกครั้ง** — แม้ prompt จะเป็นภาพภายในห้อง AI ก็มีโอกาสอ่านประโยคแรกที่พูดถึง "กระจกสะท้อนท้องฟ้า" แล้วตีความไปเป็นภาพภายนอกตึกแทน ยิ่งคำว่า **"establishing shot"** ที่ปะท้ายไว้ทุกอัน คำนี้ในภาษาถ่ายภาพ/ภาพยนตร์มักหมายถึง "ภาพมุมกว้างจากภายนอกเปิดฉาก" อยู่แล้ว — เป็นตัวดึงให้ AI สร้างภาพตึกจากข้างนอกซ้ำแล้วซ้ำอีก **นี่คือสาเหตุที่ห้องเซิร์ฟเวอร์ออกมาเป็นภาพตึก**

2.  **รายละเอียดเฟอร์นิเจอร์เดิมเป็นคำกว้างๆ** ("a clean modern desk", "a cramped desk") ไม่มีขนาด/วัสดุ/จำนวนที่ชัดเจน — AI เลยต้อง "จินตนาการ" เอาเอง และมักเลือกขนาดเล็กที่สุดที่เป็นไปได้ตามค่าเฉลี่ยที่เทรนมา **นี่คือสาเหตุที่โต๊ะเลขาดูเล็ก**

**วิธีแก้ (ใช้ทั้งไฟล์นี้และ environment-reference-prompts.md ตั้งแต่นี้ไป):**

- แยก Master Block เป็น **2 แบบ**: Interior Block (ใช้กับทุกฉากในร่ม) กับ Exterior Block (ใช้เฉพาะฉากถ่ายจากนอกตึกจริงๆ) — Interior Block จะ**ไม่พูดถึงภายนอกตึกเลยแม้แต่คำเดียว** และมีประโยคกำกับชัดเจนว่า "ห้ามมีภายนอกตึก/ท้องฟ้าในเฟรม"

- ตัดคำว่า "establishing shot" ออกจากทุก interior prompt (ยังใช้ได้กับ exterior เท่านั้น)

- ทุกชิ้นเฟอร์นิเจอร์สำคัญ ระบุ **ขนาดเป็น cm + วัสดุ/สีที่เจาะจง + จำนวนชิ้นแน่นอน** เสมอ ไม่ใช้คำกว้างๆ

- เพิ่ม **Negative Prompt Block** ต่อท้ายทุก prompt เพื่อกันจุดที่ AI มักพลาด (สัดส่วนเพี้ยน, ตัวหนังสือเบี้ยว, แสง/เงาไม่สัมพันธ์กัน ฯลฯ)

- เพิ่มสเปกกล้อง/เลนส์/แสงแบบเทคนิคจริง แทนคำลอยๆ ว่า "photorealistic" เฉยๆ

ไฟล์นี้แก้ Master Block ในทุก prompt ให้แล้วโดยอัตโนมัติ (สลับเป็น Interior Block ให้หมด) — ส่วนโต๊ะไอซ์กับห้องเซิร์ฟเวอร์แก้ใหม่ทั้งพรอมต์ด้านล่าง เป็นตัวอย่างมาตรฐานใหม่

## ⚠️ อัปเดต v3 (20 ก.ย. รอบ 2) — วิวตึกกระจก + เรื่องล็อกภาพให้เหมือนเดิม

**1. Interior Block เดิมแก้เกินไป — บล็อกภาพวิวออกหมดทุกห้อง**

ตอนแก้ v2 ผมใส่คำสั่ง "ห้ามมีภายนอกตึก/ท้องฟ้าในเฟรมเด็ดขาด" ไว้ใน Interior Block เดียวที่ใช้กับ**ทุกห้อง**เหมือนกันหมด — นั่นแก้ปัญหา server room ได้จริง แต่ดันไปกระทบห้องที่ควรมีวิวด้วย เพราะ PRISM เป็นตึกกระจกทั้งตึก ห้องที่อยู่ริมอาคาร (ห้องคิม, ห้องประชุมใหญ่, pantry, ล็อบบี้) ควรเห็นวิวเมืองผ่านกระจกจริงๆ ตามที่คุณอั้มสังเกต ส่วนห้องที่เป็นแกนกลางตึกไม่มีผนังริม (ห้องเซิร์ฟเวอร์, ในลิฟต์, ทางเดิน/โถงลิฟต์) ถึงจะทึบไม่มีหน้าต่างจริงๆ

**แก้โดยแยก Interior Block เป็น 2 แบบ** ตามตำแหน่งห้องจริงในตึก แทนที่จะเป็นกฎเดียวปนกันหมด — ดูด้านล่าง ทุก prompt ในไฟล์นี้ถูกจัดเข้ากลุ่มที่ถูกต้องแล้ว

**2. เรื่อง "ล็อกภาพให้เหมือนเดิมทุกครั้งที่ gen"**

ตรวจสอบแล้ว (ข้อมูล ก.ย. 2026): **Google Flow / Nano Banana ในหน้าแอปที่ใช้งานทั่วไป ไม่มีปุ่มหรือค่า "seed" ให้ล็อกผลลัพธ์** ต่างจาก API บางตัวที่มี seed number กด generate ซ้ำด้วย prompt เดียวกันทุกตัวอักษร **ก็ยังได้ภาพที่ต่างกันทุกครั้ง** เป็นธรรมชาติของโมเดล — ไม่มีทางเขียน prompt ให้ "ล็อก" ผลลัพธ์จากข้อความอย่างเดียวได้ 100%

**วิธีที่ถูกต้องในการได้ "ภาพเดิม" ทุกครั้ง (นี่คือเหตุผลที่ระบบ Ingredients ของ Flow ถูกออกแบบมา):**

1.  Generate prompt นี้**ครั้งเดียว** จนกว่าจะได้ภาพที่พอใจ (ลองได้หลายรอบ เลือกภาพที่ดีที่สุด)

2.  บันทึกภาพนั้นเป็น **Ingredient / asset** ในไลบรารีของ Flow (หรือดาวน์โหลดเก็บไว้)

3.  ตั้งแต่นั้นไป **ห้าม generate จาก prompt ข้อความซ้ำอีก** — ให้ดึงภาพที่บันทึกไว้ (@server_room_v2, @kim_office_day_v1 ฯลฯ) มาใช้เป็น Environment Ingredient ในทุก scene ที่ต้องการห้องนั้นแทน วิธีนี้จะได้ห้องเดิมเป๊ะๆ ทุกครั้ง เพราะเป็นภาพไฟล์เดียวกันจริงๆ ไม่ใช่การ generate ใหม่

พูดง่ายๆ: **prompt ที่ละเอียดคือเครื่องมือให้ได้ภาพ "ตั้งต้น" ที่ดีที่สุดในรอบแรก ไม่ใช่เครื่องมือให้ล็อกผลลัพธ์** — ตัวล็อกจริงคือขั้นตอนเซฟเป็น asset แล้วเอากลับมาใช้ซ้ำ ต้องทำควบคู่กันเสมอ (ไฟล์ character-seeds.md ที่มีอยู่แล้วออกแบบมาเพื่อเก็บ asset เหล่านี้พอดี)

## 🏢 Interior Block — มีวิว (ห้องริมอาคาร มีกระจกเห็นวิวเมือง/ถนนจริง)

**ใช้กับ:** ห้องคิม, ห้องประชุมใหญ่, ห้องประชุมเล็ก, pantry, ล็อบบี้ลิฟต์ชั้น 14, ล็อบบี้ชั้นล่าง, โซน Creative, โต๊ะภูมิ-ปอนด์, มุม HR, โต๊ะไอซ์ — ห้อง/พื้นที่เหล่านี้อยู่ริมอาคารกระจก ต้องเห็นวิวเมืองหรือถนนผ่านกระจกจริงๆ

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

## 🏢 Interior Block — ห้องปิด (ไม่มีหน้าต่าง อยู่แกนกลางตึก)

**ใช้กับ:** ห้องเซิร์ฟเวอร์, ในลิฟต์, หน้าลิฟต์ (โถงลิฟต์), ทางเดินหน้าห้องประชุมใหญ่, โต๊ะแทน (IT) — พื้นที่เหล่านี้อยู่แกนกลางอาคาร ไม่ติดผนังกระจกภายนอก จึงไม่มีหน้าต่าง/วิวจริงๆ

INTERIOR SHOT, FULLY ENCLOSED -- camera is standing inside the building,

inside a windowless interior space with no exterior-facing glass at all

(it sits toward the core of the floor plan, away from the building's

glass perimeter walls); absolutely no exterior of the tower, no sky, and

no city view visible anywhere in the frame. Interior of PRISM Creative

Agency, a contemporary 2026 Bangkok creative-agency office on the 14th

floor of a Thonglor glass tower. Consistent interior design language:

matte warm-beige ("Almond Cream"-tone) painted walls, engineered

light-oak wood flooring transitioning to honed light-grey limestone tile

in corridors, black powder-coated aluminum door/partition frames,

recessed 3000K warm-white LED downlights on a dark-grey painted

exposed-concrete ceiling with black exposed ductwork.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural white balance (4000K, artificial

lighting only, no daylight source), tripod-mounted for a level,

non-distorted perspective, tack-sharp focus front to back, natural

realistic material texture and reflections. No people in frame.

## 🏙️ Exterior Consistency Block (ใช้เฉพาะฉากถ่ายจากนอกตึกจริงๆ)

EXTERIOR SHOT -- camera is outdoors, positioned at street level or

nearby, looking up/across at the building. Exterior of PRISM Creative

Agency, a 14-story glass curtain-wall office tower in the Thonglor

district of Bangkok, Thailand: blue-tinted glass facade in a uniform

grid of floor-to-ceiling window panels divided by thin silver-anodized

aluminum mullions, a double-height glass ground-floor entrance lobby

visible at street level.

Camera: photorealistic architectural exterior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm tilt-shift lens to

keep vertical building lines straight (no converging verticals), f/8

aperture, ISO 100, sharp focus front to back. No people in frame.

## 🚫 Negative Prompt Block (แปะต่อท้ายทุก prompt ในไฟล์นี้เสมอ — ทั้ง interior และ exterior)

Negative / avoid: no exterior building or sky visible in an interior

shot; no distorted, extra, or missing fingers on any hand-shaped object;

no warped, blurry, or illegible text on signage; no melted, asymmetric,

or physically-impossible furniture; no plastic-looking, waxy, or

over-smoothed surfaces; no oversaturated or neon-shifted colors; no

fisheye or barrel distortion; no floating or impossible architecture; no

inconsistent or multiple shadow directions; no lens flare, glow, or HDR

halo; no cartoonish or illustrated rendering; no visible AI artifacts or

repeating texture patterns.

## 📏 มาตรฐานเขียนรายละเอียดเฟอร์นิเจอร์ (ใช้ทุกครั้งที่เพิ่มสถานที่ใหม่)

ทุกชิ้นที่สำคัญในเฟรม ต้องระบุครบ 4 อย่างนี้ ไม่ปล่อยให้ AI เดา:

1.  **ขนาด** เป็น cm (กว้าง x ลึก x สูง)

2.  **วัสดุ/สี/ผิวสัมผัส** ที่เจาะจง (เช่น "white gloss lacquer with brushed-aluminum edge" ไม่ใช่แค่ "modern desk")

3.  **จำนวนชิ้นแน่นอน** (เช่น "4 racks", "two 27-inch monitors" ไม่ใช่ "a few")

4.  **ตำแหน่งเทียบกับจุดอ้างอิงคงที่** (เช่น "against the wall to the left of the door")

## ภายนอกตึก + ล็อบบี้

### หน้าตึก PRISM (ภายนอก, เช้า)

**อ้างอิง ep01:** *"PRISM Creative Agency — ตึกกระจกสิบสี่ชั้นกลางทองหล่อ แสงแดดเช้าสะท้อนจนต้องหรี่ตา"*

EXTERIOR SHOT -- camera is outdoors, positioned at street level or

nearby, looking up/across at the building. Exterior of PRISM Creative

Agency, a 14-story glass curtain-wall office tower in the Thonglor

district of Bangkok, Thailand: blue-tinted glass facade in a uniform

grid of floor-to-ceiling window panels divided by thin silver-anodized

aluminum mullions, a double-height glass ground-floor entrance lobby

visible at street level.

Camera: photorealistic architectural exterior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm tilt-shift lens to

keep vertical building lines straight (no converging verticals), f/8

aperture, ISO 100, sharp focus front to back. No people in frame.

Glass facade reflecting the bright morning sky, glaring morning sunlight

bouncing off the glass surface directly into the lens (soft realistic

lens glare only on the glass itself, not a rendering artifact), busy

Thonglor street level below with two motorcycle taxis in orange vests

waiting at the curb, tropical rain trees lining the sidewalk, a row of

5-6 parked motorcycles along the curb. Bright glaring morning light,

long morning shadows cast across the pavement.

Negative / avoid: no distorted or warped reflections in the glass grid,

no melted or bent window mullions, no oversaturated sky, no impossible

perspective, no lens-flare artifacts beyond a realistic sun-glint, no

people in frame.

### ล็อบบี้ลิฟต์ชั้น 14 (จุดที่ลิฟต์เปิดเข้าสู่ออฟฟิศ)

**อ้างอิง ep01:** *"ลิฟต์เปิดที่ชั้น 14... ออฟฟิศเต็มรูปแบบ"*

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

The view immediately as elevator doors open onto the 14th floor: a wide

open-plan office beyond, reception-style waiting area with low modern

sofas just past the elevator lobby, the PRISM Creative Agency logo mounted

on the wall, polished stone floor transitioning to carpet. Bright neutral

daylight from windows further inside.

### ล็อบบี้ชั้นล่างตึก PRISM

**อ้างอิง ep09:** *"หกโมงเย็น ฝนตกหนัก... ล็อบบี้ชั้นล่างมีคนยืนรอทีละคนสองคน"*

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

Ground floor lobby: wide glass entrance with automatic sliding doors,

polished stone floor, a reception desk visible in the background, tall

glass walls looking out onto the street where heavy rain is falling

outside, water streaking down the glass. Warm interior lighting contrasting

with the grey rainy evening light outside.

## พื้นที่ทำงานภายในออฟฟิศ

### ห้องคิม (ห้องผู้บริหาร)

**อ้างอิง ep01:** *"ประตูห้องทำงานที่มีกระจกบังตาฝ้า... คิมหันมาจากจอคอมพิวเตอร์"* + ไบเบิล: *"มีห้องทำงานส่วนตัว กระจกบังตาฝ้า"*

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

Interior of a private executive office: one frosted-glass wall and door

facing the open office outside, a sleek dark wood desk with a computer

monitor and a pen holder, a black ergonomic office chair, a floor-to-ceiling

clear glass window on the opposite side showing the Bangkok skyline,

minimalist decor with no clutter. Bright daytime working light.

**เวอร์ชันเย็น (สำหรับ ep07 ที่คิมยังทำงานอยู่ดึก):**

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

Interior of a private executive office: one frosted-glass wall and door

facing the open office outside, a sleek dark wood desk with a computer

monitor and a pen holder, a black ergonomic office chair, a floor-to-ceiling

clear glass window on the opposite side showing the city skyline lit up at

night. Warm desk lamp light, most of the outer office beyond the frosted

glass dark and empty, a lone lit office at night.

### โต๊ะไอซ์ (นอกห้องคิม)

**อ้างอิง ไบเบิล:** *"โต๊ะอยู่ข้างนอกห้องคิม"* — ปรากฏ ep01/06/07/08

**🔧 v2 — แก้ปัญหา "โต๊ะดูเล็ก ไม่สมฐานะ":** เพิ่มขนาดจริงเป็น cm ทำให้เป็นโต๊ะทรง L ขนาดใหญ่กว่าปกติ วัสดุเกรดสูง (ลามิเนตเงา + สแตนเลส) มีจอคู่/โทรศัพท์สำนักงาน/ตู้เก็บเอกสารเข้าชุด และมุมรอรับแขกเล็กๆ ข้างโต๊ะ — สื่อสถานะว่าเป็นเลขาของผู้บริหารระดับสูง ไม่ใช่โต๊ะพนักงานทั่วไป

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

An executive secretary's workstation positioned directly in front of a

private office's frosted acid-etched glass wall and door (a dark

walnut-veneer door with a brushed-steel lever handle visible directly

behind the desk, an empty brushed-silver nameplate holder mounted on the

wall beside the door frame). The desk is a substantial L-shaped

executive-support desk, 180cm along the long side and 140cm along the

return, white gloss lacquer worktop with a brushed-aluminum waterfall

edge, resting on a brushed stainless-steel frame -- noticeably larger

and higher-spec than the standard desks in the open-plan area behind it,

visually signaling the seniority of the executive it serves. On the

desk: two identical 27-inch monitors side by side mounted on a

dual-monitor aluminum arm, a slim wireless keyboard and mouse, a black

desk telephone with a row of extension buttons, one closed white leather

portfolio folder, a single white orchid in a round white ceramic pot in

the corner, and a slim brushed-metal gooseneck desk lamp switched off.

A tall white gloss lacquer storage credenza, 120cm wide x 45cm deep x

75cm tall, matching the desk finish, stands against the wall to the

right, topped with two neatly stacked grey document trays. A high-back

ergonomic mesh office chair (black frame, dark grey mesh backrest,

adjustable armrests) is tucked under the desk. To the left of the desk,

a small visitor waiting nook: two low-back cream fabric armchairs

flanking a round glass-top side table (60cm diameter) with two design

magazines stacked neatly on it. Honed light-grey limestone floor beneath

the desk area, rows of open-plan desks visible further back beyond the

secretary's station. Bright, even, neutral daylight from windows out of

frame to the side.

Negative / avoid: no exterior building or sky visible; no distorted or

extra fingers on any object; no warped or illegible text on the

nameplate or documents; no melted or asymmetric furniture; no

plastic-looking or waxy surfaces; no oversaturated colors; no

inconsistent shadow directions; no cartoonish rendering; the desk must

read as noticeably larger and more premium than a standard open-plan

desk, not smaller.

### โซนเปิด ทีม Creative (เจมส์-ฟลุ้ค ตรงข้ามกัน, ดิว-นนท์ ข้างกัน)

**อ้างอิง ep01/04/06/07:** โต๊ะเรียงเป็นแถว จอคู่ สมุดจดโน้ตติดขอบจอ

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

An open-plan creative team work area: rows of modern desks arranged in

facing pairs, each with dual-monitor setups, drawing tablets, a few sticky

notes on monitor edges, ergonomic mesh office chairs, large windows along

one side letting in natural daylight. Bright neutral daytime lighting,

lived-in but tidy workspace.

**เวอร์ชันดึก (สำหรับ ep07 OT night):**

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

An open-plan creative team work area at night: rows of modern desks

arranged in facing pairs, most desks empty and dark, a couple of desks

still lit by monitor glow and a single desk lamp, dual-monitor setups,

drawing tablets, sticky notes on monitor edges. Dark outside the windows,

quiet dim atmosphere, most overhead lights off except a few work lamps.

### โต๊ะภูมิ + โต๊ะปอนด์ (ทีม Strategy)

**อ้างอิง ep02:** *"นั่งอยู่ที่โต๊ะแล้ว หน้าจอเปิดอยู่สามหน้าต่าง กาแฟดำวางข้างคีย์บอร์ดไม่ใส่น้ำตาล"*

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

A project manager's desk in the strategy team area: a triple-monitor

computer setup, a plain black cup of coffee with no sugar or milk beside

the keyboard, an organized clutter-free desk. A smaller intern's desk

positioned nearby with a thick paper notebook resting on it, open-plan

office setting around. Bright neutral morning daylight, quiet early-office

mood.

### มุม HR (โต๊ะเต)

**อ้างอิง ep06:** *"เตนั่งที่โต๊ะ มุม HR"*

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

An HR staff desk in a quieter corner of the office: a warm approachable

desk setup with a small potted plant, a small bowl of wrapped candy,

a corkboard with colorful sticky notes and a small photo, personal warm

touches distinguishing it from the other more minimal desks. Bright neutral

daytime lighting.

### โต๊ะแทน (IT)

**อ้างอิง ep06:** *"จอบนโต๊ะเปิดทิ้งไว้... มุมจอด้านบนมีรอยเทปใสแปะ จอเก่ากว่าเครื่องอื่นในออฟฟิศ"*

INTERIOR SHOT, FULLY ENCLOSED -- camera is standing inside the building,

inside a windowless interior space with no exterior-facing glass at all

(it sits toward the core of the floor plan, away from the building's

glass perimeter walls); absolutely no exterior of the tower, no sky, and

no city view visible anywhere in the frame. Interior of PRISM Creative

Agency, a contemporary 2026 Bangkok creative-agency office on the 14th

floor of a Thonglor glass tower. Consistent interior design language:

matte warm-beige ("Almond Cream"-tone) painted walls, engineered

light-oak wood flooring transitioning to honed light-grey limestone tile

in corridors, black powder-coated aluminum door/partition frames,

recessed 3000K warm-white LED downlights on a dark-grey painted

exposed-concrete ceiling with black exposed ductwork.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural white balance (4000K, artificial

lighting only, no daylight source), tripod-mounted for a level,

non-distorted perspective, tack-sharp focus front to back, natural

realistic material texture and reflections. No people in frame.

An IT support desk positioned near the server room: a noticeably older

monitor than the rest of the office with a strip of clear tape on one

corner and a faint screen flicker, tangled cables underneath the desk, a

worn keyboard, a small toolkit box on the side. Neutral daytime lighting,

slightly less tidy than other desks.

### ห้องเซิร์ฟเวอร์

**อ้างอิง ep07:** *"แทนเดินออกจากห้องเซิร์ฟเวอร์ ถือโน้ตบุ๊คเครื่องเก่า"*

**🔧 v2 — แก้ปัญหา "ออกมาเป็นภาพตึกภายนอก":** ระบุขนาดห้องจริง ตำแหน่งกล้อง (ถ่ายจากในห้อง มองจากใกล้ประตู) และคำสั่งห้ามชัดเจนซ้ำสองครั้งว่าห้ามมีภายนอกตึกในเฟรม เพิ่มรายละเอียดเชิงเทคนิค (จำนวน rack, สายไฟ, เครื่องปรับอากาศ) ให้ AI ไม่ต้องเดา

INTERIOR SHOT -- camera is standing inside a small windowless room deep

inside the building; absolutely no exterior of the tower, no sky, and no

building facade visible anywhere in the frame; this is NOT an exterior

architectural shot. Interior of PRISM Creative Agency, a contemporary

2026 Bangkok creative-agency office on the 14th floor of a Thonglor

glass tower. Consistent interior design language: matte warm-beige

("Almond Cream"-tone) painted walls, recessed 3000K warm-white LED

downlights, dark-grey painted exposed-concrete ceiling with black

exposed ductwork.

Camera: photorealistic architectural interior photography, shot from

just inside the doorway looking into the room, full-frame mirrorless

camera (Sony A7R V) with a 24mm wide-angle lens, f/5.6 aperture, ISO 400

(dim-room exposure), tripod-mounted, tack-sharp focus front to back,

natural realistic material texture and reflections. No people in frame.

A dedicated IT server room, approximately 3 meters wide by 2.5 meters

deep, windowless on all sides, entered through a plain grey solid-core

door with a keycard reader mounted beside the frame (door held open,

shot from just inside it -- never a view from outside the building).

Pale-grey anti-static perforated raised-floor tiles cover the entire

floor. Two rows of black powder-coated steel 42U server racks (4 racks

total) line the back wall, each rack populated with 8-10 rack-mounted

servers and network switches showing small green and amber status LEDs;

thick bundles of blue and black Cat6 ethernet cables run vertically

through black plastic cable-management arms on the side of each rack

and disappear into gaps between the raised floor tiles. A wall-mounted

white-plastic precision in-row air-conditioning unit is fixed to the

left wall, its small digital display reading "18 C". Along the right

wall, a plain grey laminate workbench, 120cm wide x 60cm deep, holds one

aging beige-grey laptop with a strip of clear tape visible on one corner

of its lid, a small external USB hard drive, and a coiled spare ethernet

cable. A red cylindrical fire extinguisher is mounted on a wall bracket

beside the door. Lighting comes from a single bare fluorescent tube

fixture on the ceiling giving flat, cool-white light (5000K), with the

server racks' status LEDs adding a faint cold blue-white glow reflected

on the raised floor tiles. No windows anywhere, no view of the outside

world. Slightly cluttered but functional technical space, quiet and dim

compared to the rest of the office.

Negative / avoid: absolutely no exterior building, skyline, or sky

visible anywhere in the frame -- this must read unmistakably as a small

enclosed interior room, not an establishing shot of the tower; no

distorted or extra fingers on any object; no warped or illegible text on

equipment labels; no melted or physically-impossible rack shapes; no

oversaturated colors; no inconsistent shadow directions; no lens flare;

no cartoonish rendering.

### ห้องประชุมเล็ก

**อ้างอิง ep04:** *"บ่ายสอง ห้องประชุมเล็ก"* — ต่างจากห้องประชุมใหญ่

INTERIOR SHOT WITH EXTERIOR VIEW THROUGH GLASS -- camera is standing

inside the building. The room itself -- its walls, floor, ceiling, and

furniture -- must read unmistakably as an interior space, but this room

sits along the building's glass curtain wall, so a real exterior view

(Bangkok skyline or street below) is visible through the floor-to-ceiling

window exactly as it would be in a real glass office tower. Interior of

PRISM Creative Agency, a contemporary 2026 Bangkok creative-agency

office on the 14th floor of a Thonglor glass tower. Consistent interior

design language throughout the office: matte warm-beige ("Almond

Cream"-tone) painted walls, engineered light-oak wood flooring in work

areas transitioning to honed light-grey limestone tile in corridors and

lobbies, floor-to-ceiling glass partitions in black powder-coated

aluminum frames, acid-etched frosted glass for private offices and

meeting rooms, recessed 3000K warm-white LED downlights evenly spaced on

a dark-grey painted exposed-concrete ceiling with black-painted exposed

ductwork as an industrial-loft accent.

Camera: photorealistic architectural interior photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 24mm wide-angle lens,

f/5.6 aperture, ISO 200, natural daylight-balanced white balance (5200K),

tripod-mounted for a level, non-distorted perspective, tack-sharp focus

front to back, natural realistic material texture and reflections,

correctly balanced exposure so both the interior and the exterior view

through the window are clearly visible together (not a blown-out white

window, not a silhouetted dark interior). No people in frame.

A small meeting room, more intimate than the main conference room: a

compact rectangular table seating about 4-6 people, a wall-mounted display

screen, comfortable upholstered chairs, a glass wall with blinds partially

closed for privacy. Bright neutral afternoon daylight.

### ดาดฟ้าตึก PRISM (เตรียมไว้ล่วงหน้า — ยังไม่ปรากฏใน ep1-9 แต่มีในไบเบิล)

**อ้างอิง ไบเบิล:** *"มีดาดฟ้า (ชั้น 14 เป็นชั้นบนสุด)"* — จะใช้ในตอนหลัง (ฉากพระอาทิตย์ตกคิม×ไอซ์)

ROOFTOP SHOT -- camera is standing on an open-air rooftop terrace on top

of the building, looking out toward the city skyline; the building's own

facade is not the subject (only the terrace floor/railing and the

skyline beyond). Rooftop terrace atop PRISM Creative Agency, a 14-story

tower in Thonglor, Bangkok.

Camera: photorealistic outdoor architectural photography, shot on a

full-frame mirrorless camera (Sony A7R V) with a 35mm lens, f/4 aperture,

ISO 200, sharp focus front to back, natural golden-hour color rendering.

No people in frame.

A compact rooftop terrace, roughly 6 meters by 4 meters: light-grey

composite decking underfoot, a waist-high glass safety railing (clear

tempered glass in a thin black aluminum frame) running along the open

edge, four large terracotta planter pots with small potted frangipani

trees spaced along the railing, one low rattan-weave two-seat bench with

cream cushions positioned facing the view, a small round concrete-top

side table beside it. Beyond the railing, a clear unobstructed view of

the Bangkok skyline at sunset: warm orange-and-pink dusk sky, silhouettes

of distant high-rises, city lights just beginning to switch on. Warm

golden-hour to dusk lighting, long soft shadows across the decking,

quiet romantic atmosphere.

Negative / avoid: no distorted railing lines, no floating or

physically-impossible furniture, no oversaturated sky, no melted plant

shapes, no lens flare artifacts beyond a soft realistic sun-glow, no

people in frame.

## นอกตึก / ย่านทองหล่อ

### ร้านข้าวแกงปากซอย

**อ้างอิง ep03:** *"ข้าวกล่องที่ซื้อมาจากร้านข้าวแกงปากซอย สี่สิบห้าบาท"*

A small Thai curry rice street food stall at the mouth of a soi in the

Thonglor area of Bangkok: a simple metal cart with glass display trays of

Thai curries and stir-fried dishes, styrofoam takeout boxes stacked

nearby, a hand-written menu sign, a small plastic stool for the vendor,

motorcycles parked alongside, busy Bangkok street backdrop. Photorealistic

street photography, bright midday daylight, no people in frame.

### ร้านกาแฟข้างตึก

**อ้างอิง ep03:** *"แก้วกาแฟเย็น... ยี่ห้อร้านข้างตึก... แค่ยี่สิบห้าบาท"*

A small local iced coffee stand next to a modern office building in

Thonglor, Bangkok: a simple kiosk cart with a hand-painted coffee menu

board, bags of coffee beans, stacks of plastic cups with lids and straws

on the counter, a striped awning for shade, ice bucket visible on the

counter. Photorealistic street photography, bright midday daylight, no

people in frame.

### ร้านอาหารญี่ปุ่นเล็กๆ ปากซอยทองหล่อ

**อ้างอิง ep05:** *"ร้านอาหารญี่ปุ่นเล็กๆ ปากซอยทองหล่อ แปดคนนั่งโต๊ะยาว"* + ไบเบิล: *"มีชั้นลอย 251-500 บาท/คน"*

A small izakaya-style Japanese restaurant at the mouth of a soi in

Thonglor, Bangkok: a long wooden dining table seating eight, a low

mezzanine level visible above the main floor, warm wood interior, hanging

paper lanterns, a small open kitchen counter visible in the back, cozy

intimate atmosphere. Photorealistic restaurant interior photography, warm

evening lighting, no people in frame.

### ถนนทองหล่อ/สุขุมวิท ตอนกลางคืนคึกคัก (คืนวันศุกร์)

**อ้างอิง ep05:** *"ถนนสุขุมวิทวันศุกร์คึกคัก เสียงเพลงจากร้านเหล้า เสียงรถ เสียงคนหัวเราะ"*

Thonglor street in Bangkok at night on a lively Friday evening: neon signs

from bars and restaurants lining the street, warm string lights strung

between buildings, motorcycle taxis waiting at the roadside, glowing

shopfronts, a busy energetic nightlife atmosphere. Photorealistic street

photography, no people in frame.

### ซอยทองหล่อตอนฝนตกหนัก

**อ้างอิง ep09:** *"ฝนตกหนัก... ถนนกลายเป็นลำธาร น้ำสาดจากรถที่แล่นผ่าน"*

A narrow soi street in the Thonglor area of Bangkok during heavy rain at

dusk: flooded pavement reflecting neon shop signs, visible rain streaking

through the air, warm streetlights glowing through the downpour, glistening

wet asphalt, moody atmospheric evening light. Photorealistic street

photography, no people in frame.

## BTS สายสุขุมวิท

### สถานี BTS ทองหล่อ (ชานชาลา) — ปกติ

**อ้างอิง ep05:** *"เดินไม่กี่นาทีก็ถึงสถานี BTS ทองหล่อ"*

BTS Thong Lo skytrain station platform in Bangkok, Thailand: elevated

outdoor platform with a curved roof canopy, yellow tactile paving strips

along the platform edge, digital train arrival information screens, city

traffic visible below on Sukhumvit Road. Photorealistic transit photography,

clear evening light, no people in frame.

### สถานี BTS ทองหล่อ — เย็นฝนตก

**อ้างอิง ep09:** สถานีที่เจมส์กับฟลุ้คไปหลบฝน

BTS Thong Lo skytrain station platform in Bangkok, Thailand, sheltered

under the platform roof during heavy rain: rain visible falling just

beyond the covered area, wet reflective platform floor, digital train

arrival screens, city lights beginning to glow in the wet evening dusk.

Photorealistic transit photography, no people in frame.

### ในตู้รถไฟ BTS

**อ้างอิง ep05/09:** ยืนเกาะราว มองผ่านกระจก

Interior of a BTS Skytrain train car in Bangkok: rows of blue upholstered

seats along the sides, stainless steel grab poles and overhead handles, a

route map displayed above the windows, large windows showing the city

passing by outside. Clean modern transit interior, photorealistic

photography, no people in frame.

## 📌 Checklist

- ทุกครั้งก่อนกด generate — แปะ **Negative Prompt Block** ต่อท้าย prompt เสมอ (อยู่ด้านบนของไฟล์นี้)

  เช็คว่า prompt เป็นภาพนอกอาคาร / ในร่มมีวิว / ในร่มไม่มีหน้าต่าง แล้วใช้ **Exterior Block** / **Interior Block — มีวิว** / **Interior Block — ห้องปิด** ให้ถูกประเภท — ห้ามผสมกัน

  Generate ทั้งหมด 18 environment ในไฟล์นี้ (ดูตารางดัชนีด้านบนว่าตอนไหนต้องใช้อันไหน) — ห้องเซิร์ฟเวอร์กับโต๊ะไอซ์เป็นเวอร์ชัน v2 ที่แก้ปัญหาแล้ว ใช้เวอร์ชันนี้เท่านั้น

  เทียบกับ environment-reference-prompts.md — 2 ไฟล์นี้ต้องใช้ Interior Block ชุดเดียวกัน เพื่อให้ทุกมุมของตึกดู "เป็นตึกเดียวกัน"

  **สำคัญที่สุด — เรื่องภาพเหมือนเดิมทุกครั้ง:** Flow ไม่มี seed ให้ล็อก ดังนั้น generate ทุก prompt แค่**ครั้งเดียว**จนพอใจ แล้วเซฟเป็น Ingredient/asset ทันที ห้าม generate จาก prompt เดิมซ้ำอีกในภายหลัง (จะได้ห้องคนละภาพ) — ให้ดึง asset ที่เซฟไว้มาใช้แทนเสมอ

  ถ้าภาพที่ได้ยังไม่ตรง (เช่น ยังมีภายนอกตึกโผล่มาในห้องปิด หรือของบางชิ้นดูผิดสัดส่วน) — ลอง generate ใหม่อีก 1-2 รอบก่อน (Nano Banana มีความสุ่มในตัว) แล้วค่อยแจ้งผมถ้ายังไม่ตรงซ้ำๆ จะช่วยเพิ่มรายละเอียดกำกับให้แน่นขึ้นอีก

  ตั้งชื่อ asset ให้สื่อถึง ep ที่ใช้ครั้งแรก เช่น kim_office_ep01_v1, soi_rain_ep09_v1, ice_desk_v2, server_room_v2

  เก็บ URL/asset name ลงใน character-seeds.md (หมวด Environment Ingredients)

  เมื่อเขียนตอนใหม่ (ep10 เป็นต้นไป) ถ้ามีสถานที่ใหม่ที่ยังไม่เคยทำ — แจ้งผมได้ ผมช่วยดึงรายละเอียดจากเนื้อเรื่องมาทำ prompt ตามมาตรฐาน hyper-detail นี้ให้ทุกครั้ง
