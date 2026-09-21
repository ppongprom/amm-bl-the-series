# ชั้น 14 มีรัก — Environment Reference Prompts (Google Flow / Veo 3.1 Syntax)

**วัตถุประสงค์:** ภาพอ้างอิงบรรยากาศแต่ละมุมของตึก PRISM + สวนลุมพินี ใช้เป็น "Environment Ingredient" คู่กับ Character Ingredient ตอนสร้าง scene — ช่วยให้ฉากในสถานที่เดียวกัน (เช่น pantry ตอนเช้า vs pantry ตอนเย็น) มีโทนแสง/สี/decor คงที่ตลอดทั้ง 40 ตอน

**ใช้กับ:** Google Flow (Ingredients to Video) — สร้างเป็น Environment Ingredient แยกจาก Character Ingredient (จำไว้ว่า Flow ใส่ ingredient ได้สูงสุด 3 ต่อ scene — ปกติจะเป็น ตัวละคร 2 + environment 1)

**ทุกภาพในไฟล์นี้:** ไม่มีคนอยู่ในเฟรม (no people) เพื่อให้ใช้เป็น "ฉากเปล่า" อ้างอิงล้วนๆ แยกจากตัวละคร

## ⚠️ อัปเดต v3 (20 ก.ย.) — อ่านก่อนใช้ไฟล์นี้

**v2:** Master Block เดิมขึ้นต้นด้วยการบรรยายตึกภายนอก + คำว่า "establishing shot" ทำให้ AI มีโอกาสสร้างภาพตึกจากข้างนอกแทนที่จะเป็นภาพในห้อง — แก้แล้วด้วย Interior Consistency Block (รายละเอียดเต็มดูใน environment-reference-by-episode.md)

**v3:** จากฟีดแบ็กจริง PRISM เป็นตึกกระจกทั้งตึก ห้อง/พื้นที่ที่อยู่ริมอาคาร (pantry, ห้องประชุมใหญ่) **ควรเห็นวิวเมืองผ่านกระจกจริงๆ** ส่วนที่อยู่แกนกลางตึก (ทางเดิน, ลิฟต์, โถงลิฟต์) ไม่มีผนังกระจกจริง เลยแยก Interior Block เป็น **2 แบบ** ตามตำแหน่งห้องจริง — ทุก prompt ด้านล่างจัดเข้ากลุ่มที่ถูกต้องแล้ว

**เรื่องล็อกภาพให้เหมือนเดิมทุกครั้ง:** Google Flow/Nano Banana ไม่มี seed ให้ล็อกผลลัพธ์ — prompt ละเอียดช่วยให้ได้ภาพตั้งต้นที่ดีที่สุด แต่การจะได้ "ภาพเดิมเป๊ะ" ทุกครั้งต้อง **generate ครั้งเดียว แล้วเซฟเป็น Ingredient/asset เอากลับมาใช้ซ้ำ** ไม่ generate จาก prompt ข้อความใหม่อีก (รายละเอียดเต็มดูใน environment-reference-by-episode.md หัวข้อ v3)

## 🏢 Interior Block — มีวิว (ใช้กับ pantry, ในห้องประชุมใหญ่ — ห้องริมอาคาร มีกระจกเห็นวิวเมืองจริง)

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

## 🏢 Interior Block — ห้องปิด (ใช้กับ ทางเดินหน้าห้องประชุมใหญ่, ในลิฟต์, หน้าลิฟต์ — พื้นที่แกนกลางตึก ไม่มีหน้าต่าง)

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

## 🚫 Negative Prompt Block (แปะต่อท้ายทุก prompt ในไฟล์นี้ด้วยเสมอ — ยังไม่ได้ใส่ไว้ในตัวอย่างด้านล่าง ให้ต่อท้ายเองทุกครั้งก่อน generate)

Negative / avoid: no exterior building or sky visible in an interior

shot; no distorted, extra, or missing fingers on any hand-shaped object;

no warped, blurry, or illegible text on signage; no melted, asymmetric,

or physically-impossible furniture; no plastic-looking, waxy, or

over-smoothed surfaces; no oversaturated or neon-shifted colors; no

fisheye or barrel distortion; no floating or impossible architecture; no

inconsistent or multiple shadow directions; no lens flare, glow, or HDR

halo; no cartoonish or illustrated rendering; no visible AI artifacts or

repeating texture patterns.

**หมวดเวลาของวัน (เลือกใส่ต่อท้ายตามต้องการ):**

| **ช่วงเวลา** | **Lighting descriptor ที่ใช้** |
|----|----|
| เช้า (~8:00-9:00) | soft cool morning daylight, low-angle sun, quiet and empty, gentle blue-white tone |
| กลางวัน (~12:00-13:00) | bright even midday daylight, high sun angle, crisp clear light, neutral white balance |
| เย็น (~17:00-18:00) | warm golden-hour light, orange and pink sky visible through windows, long soft shadows |
| ค่ำ (~20:00-21:00) | dark night sky outside, warm interior artificial lighting, city skyline lights twinkling through windows, quiet emptied space |

## 1. Pantry (ครัวส่วนกลาง)

**รายละเอียดที่ต้องคงที่:** เคาน์เตอร์หินขัดสีอ่อน, เครื่องชงกาแฟสแตนเลส, ตู้เย็นกระจกฝ้า, บาร์สตูลไม้ 3-4 ตัว, ผนังกระจกมองเห็นวิวเมือง, ตู้เก็บแก้ว/จานสีขาว

### เช้า

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

A modern office pantry area: pale polished stone countertop, stainless

steel espresso machine, frosted-glass mini fridge, three wooden bar stools,

white ceramic cup and plate storage, floor-to-ceiling window showing the

city skyline. Soft cool morning daylight, low-angle sun, quiet and empty,

gentle blue-white tone.

### กลางวัน

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

A modern office pantry area: pale polished stone countertop, stainless

steel espresso machine, frosted-glass mini fridge, three wooden bar stools,

white ceramic cup and plate storage, floor-to-ceiling window showing the

city skyline. Bright even midday daylight, high sun angle, crisp clear

light, neutral white balance.

### เย็น

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

A modern office pantry area: pale polished stone countertop, stainless

steel espresso machine, frosted-glass mini fridge, three wooden bar stools,

white ceramic cup and plate storage, floor-to-ceiling window showing the

city skyline. Warm golden-hour light, orange and pink sky visible through

the window, long soft shadows across the countertop.

### ค่ำ

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

A modern office pantry area: pale polished stone countertop, stainless

steel espresso machine, frosted-glass mini fridge, three wooden bar stools,

white ceramic cup and plate storage, floor-to-ceiling window showing the

city skyline. Dark night sky outside, warm interior pendant lighting above

the counter, city skyline lights twinkling through the window, quiet

emptied space.

## 2. หน้าห้องประชุมใหญ่ (ทางเดินหน้าห้องประชุม)

**รายละเอียดที่ต้องคงที่:** ทางเดินพื้นหินขัดสีเทาอ่อน, ผนังกระจกฝ้าของห้องประชุมด้านหนึ่ง, ป้ายชื่อห้องประชุมติดผนังกระจก, ไฟดาวน์ไลท์เพดาน, ต้นไม้กระถางเล็กมุมทางเดิน

### เช้า

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

A hallway just outside the main glass-walled meeting room: light grey

polished stone floor, frosted glass wall on one side with a meeting room

name sign, recessed ceiling downlights, a small potted plant in the corner.

Soft cool morning daylight, low-angle sun, quiet and empty, gentle

blue-white tone.

### กลางวัน

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

A hallway just outside the main glass-walled meeting room: light grey

polished stone floor, frosted glass wall on one side with a meeting room

name sign, recessed ceiling downlights, a small potted plant in the corner.

Bright even midday daylight, high sun angle, crisp clear light, neutral

white balance.

### เย็น

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

A hallway just outside the main glass-walled meeting room: light grey

polished stone floor, frosted glass wall on one side with a meeting room

name sign, recessed ceiling downlights, a small potted plant in the corner.

Warm golden-hour light spilling in from a distant window, long soft

shadows along the floor.

### ค่ำ

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

A hallway just outside the main glass-walled meeting room: light grey

polished stone floor, frosted glass wall on one side with a meeting room

name sign, recessed ceiling downlights, a small potted plant in the corner.

Dark outside, warm recessed ceiling lighting illuminating the corridor,

quiet and empty at night.

## 3. ในห้องประชุมใหญ่

**รายละเอียดที่ต้องคงที่:** โต๊ะประชุมยาวสีไม้อ่อน เก้าอี้หนังสีเทาเข้ม 10-12 ตัว จอโปรเจคเตอร์ผนังฝั่งหัวโต๊ะ ผนังกระจกมองเห็นวิวเมืองอีกด้าน ไวท์บอร์ดกระจกมุมห้อง

### เช้า

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

Interior of the main meeting room: a long light-wood conference table with

10-12 dark grey leather chairs, a large projector screen mounted on the

wall at the head of the table, a floor-to-ceiling glass wall on the

opposite side showing the city skyline, a glass whiteboard in the corner.

Soft cool morning daylight, low-angle sun, quiet and empty, gentle

blue-white tone.

### กลางวัน

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

Interior of the main meeting room: a long light-wood conference table with

10-12 dark grey leather chairs, a large projector screen mounted on the

wall at the head of the table, a floor-to-ceiling glass wall on the

opposite side showing the city skyline, a glass whiteboard in the corner.

Bright even midday daylight, high sun angle, crisp clear light, neutral

white balance.

### เย็น

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

Interior of the main meeting room: a long light-wood conference table with

10-12 dark grey leather chairs, a large projector screen mounted on the

wall at the head of the table, a floor-to-ceiling glass wall on the

opposite side showing the city skyline, a glass whiteboard in the corner.

Warm golden-hour light streaming through the glass wall, orange and pink

sky over the skyline, long soft shadows across the table.

### ค่ำ

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

Interior of the main meeting room: a long light-wood conference table with

10-12 dark grey leather chairs, a large projector screen mounted on the

wall at the head of the table, a floor-to-ceiling glass wall on the

opposite side showing the city skyline, a glass whiteboard in the corner.

Dark night sky outside, city lights visible through the glass wall, warm

interior downlighting over the table, quiet emptied room.

## 4. ในลิฟต์

**รายละเอียดที่ต้องคงที่:** ลิฟต์กระจกสมัยใหม่ ผนังสแตนเลสขัดเงาด้านหนึ่ง กระจกเงาอีกด้าน แผงปุ่มกดชั้น 1-14 ไฟ LED สีขาวนวล ราวจับสแตนเลส

### เช้า

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

Interior of a modern glass elevator: brushed stainless steel wall on one

side, mirrored glass wall on the other, a floor-button panel showing

numbers 1 through 14, soft white LED lighting, a stainless steel handrail.

Soft cool light suggesting early morning, doors closed, empty car.

### กลางวัน

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

Interior of a modern glass elevator: brushed stainless steel wall on one

side, mirrored glass wall on the other, a floor-button panel showing

numbers 1 through 14, soft white LED lighting, a stainless steel handrail.

Bright neutral lighting, crisp and clean, doors closed, empty car.

### เย็น

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

Interior of a modern glass elevator: brushed stainless steel wall on one

side, mirrored glass wall on the other, a floor-button panel showing

numbers 1 through 14, soft white LED lighting with a warm golden tint,

a stainless steel handrail. Doors closed, empty car, warm evening mood.

### ค่ำ

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

Interior of a modern glass elevator: brushed stainless steel wall on one

side, mirrored glass wall on the other, a floor-button panel showing

numbers 1 through 14, dim warm LED lighting, a stainless steel handrail.

Doors closed, empty car, quiet late-night mood.

## 5. หน้าลิฟต์ (โถงลิฟต์แต่ละชั้น)

**รายละเอียดที่ต้องคงที่:** โถงลิฟต์พื้นหินขัด ผนังไม้อ่อนกรุรอบประตูลิฟต์สแตนเลส ป้ายตัวเลขชั้น LED เหนือประตู ไฟดาวน์ไลท์เพดาน กระถางต้นไม้ประดับ

### เช้า

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

An elevator lobby on one of the office floors: polished stone floor, warm

light-wood paneling surrounding the brushed steel elevator doors, an LED

floor-number display above the doors, recessed ceiling downlights, a

decorative potted plant to the side. Soft cool morning daylight from a

nearby window, quiet and empty.

### กลางวัน

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

An elevator lobby on one of the office floors: polished stone floor, warm

light-wood paneling surrounding the brushed steel elevator doors, an LED

floor-number display above the doors, recessed ceiling downlights, a

decorative potted plant to the side. Bright even midday daylight, crisp

clear light, neutral white balance.

### เย็น

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

An elevator lobby on one of the office floors: polished stone floor, warm

light-wood paneling surrounding the brushed steel elevator doors, an LED

floor-number display above the doors, recessed ceiling downlights, a

decorative potted plant to the side. Warm golden-hour light from a nearby

window, long soft shadows across the floor.

### ค่ำ

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

An elevator lobby on one of the office floors: polished stone floor, warm

light-wood paneling surrounding the brushed steel elevator doors, an LED

floor-number display above the doors, recessed ceiling downlights, a

decorative potted plant to the side. Dark outside, warm interior downlights

illuminating the lobby, quiet and empty at night.

## 🌳 สวนลุมพินี (Lumpini Park)

**หมายเหตุ:** ใช้สำหรับฉากนอกออฟฟิศ — รวมถึงฉากสำคัญช่วงท้ายเรื่อง (ภูมิ×ปอนด์ กลับไปที่สวนที่เคยนั่งคุยกันครั้งแรก) ไม่ต้องแปะ Master Building Consistency Block เพราะเป็นสถานที่ธรรมชาติคนละสไตล์กับตึก

**รายละเอียดที่ต้องคงที่:** ทะเลสาบกลางสวน ทางเดินปูอิฐรอบทะเลสาบ ต้นไม้ใหญ่ร่มรื่น ม้านั่งไม้สีเขียวเข้มริมทาง ฉากหลังเป็นตึกระฟ้าย่านสีลม/สาทรลิบๆ ไกลๆ

### กลางวัน (สำหรับฉากทั่วไป/เดินเล่น)

Lumpini Park, Bangkok, Thailand: a large public park with a central lake,

a brick-paved walking path circling the water, tall shady rain trees lining

the path, dark green wooden benches along the walkway, joggers' path

visible, the distant Bangkok skyline of Silom/Sathorn skyscrapers faintly

visible beyond the treeline. Bright clear midday daylight, dappled sunlight

through the tree canopy, photorealistic outdoor photography, wide-angle

lens, no people in frame, establishing shot.

### เย็น/พระอาทิตย์ตก (สำหรับฉากอารมณ์สำคัญ เช่น ฉากขอแต่งงาน)

Lumpini Park, Bangkok, Thailand: a large public park with a central lake

reflecting the sunset sky, a brick-paved walking path circling the water,

tall shady rain trees lining the path, a dark green wooden bench along the

walkway, the distant Bangkok skyline of Silom/Sathorn skyscrapers silhouetted

against a warm orange-pink dusk sky, city lights just beginning to turn on

in the distance. Warm golden-hour to dusk lighting, soft romantic

atmosphere, photorealistic outdoor photography, wide-angle lens, no people

in frame, establishing shot.

### เช้า (สำหรับฉากออกกำลังกาย/เดินเช้า)

Lumpini Park, Bangkok, Thailand: a large public park with a central lake,

a brick-paved walking path circling the water, tall shady rain trees lining

the path, dark green wooden benches along the walkway, morning mist

lightly hovering over the lake surface, the distant Bangkok skyline faintly

visible through soft morning haze. Soft cool early-morning light, gentle

blue-white tone, quiet and peaceful, photorealistic outdoor photography,

wide-angle lens, no people in frame, establishing shot.

## 📌 Checklist

- ทุกครั้งก่อนกด generate — แปะ **Negative Prompt Block** ต่อท้าย prompt เสมอ (อยู่ด้านบนของไฟล์นี้ — ตัวอย่างด้านล่างยังไม่ได้ใส่ไว้)

  Generate ทั้ง 20 prompt ของตึก PRISM (5 สถานที่ × 4 ช่วงเวลา) — ทุกอันใช้ Interior Consistency Block เวอร์ชัน v2 แล้ว

  Generate 3 เวอร์ชันของสวนลุมพินี (กลางวัน/เย็น/เช้า)

  เช็คว่าโทนสี/สไตล์ของแต่ละสถานที่ในตึกดูเป็น "ตึกเดียวกัน" สม่ำเสมอ (สี beige/glass-blue เหมือนกันหมด)

  ถ้าภาพยังไม่ตรง prompt ลอง generate ใหม่อีก 1-2 รอบก่อน (Nano Banana มีความสุ่มในตัว) แล้วแจ้งผมถ้ายังไม่ตรงซ้ำๆ

  ตั้งชื่อ asset ให้จำง่าย เช่น pantry_morning_v1, elevator_night_v1, lumpini_sunset_v1

  เก็บ URL/asset name ลงใน character-seeds.md (เพิ่มหมวด "Environment Ingredients" แยกจากตัวละคร) — หรือแจ้งผมได้ ผมช่วยเพิ่ม section ให้

  ใช้ environment ingredient คู่กับ character ingredient ตอนเขียน scene prompt ตามโครงสร้าง SCAM ในไฟล์ shorts-prompts-ep09.md
