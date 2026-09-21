# ชั้น 14 มีรัก — Character Reference Turnaround Sheets (Google Flow / Veo 3.1 Syntax)

**อัปเดต:** เปลี่ยนจาก "ภาพนิ่งท่าเดียว" เป็น **Character Reference Turnaround Sheet** — ภาพเดียวที่มีหลายมุมมองในตัว (ครึ่งตัว/เต็มตัว/หน้า/ข้าง/หลัง/ซูมหน้า) ใช้เป็นต้นแบบอ้างอิงตอนสร้าง video clip ที่ต้องเห็นตัวละครจากหลายมุม — มาตรฐานเดียวกับที่ทีมอนิเมชัน/เกมใช้ทำ "model sheet" ก่อนเริ่มโปรดักชันจริง

**ใช้กับ:** Google Flow (Ingredients to Video) — Nano Banana สร้างภาพนิ่ง Ingredient + Veo 3.1 สร้างวิดีโอ

## ⚠️ ข้อมูลพื้นฐาน (เหมือนเดิม)

- ต้องมี Google AI Plus/Pro ขึ้นไป, ไม่มี free tier ถาวร

- คุมหน้าตัวละครด้วย **Ingredients** (@ เรียกใช้), สูงสุด 3 ต่อ scene

- รองรับ 9:16 vertical เต็มระบบ, คลิป 8-10 วิ/ครั้ง ต่อกันด้วย Scenebuilder

- Native audio ภาษาไทยยังไม่ยืนยันคุณภาพ — ทดสอบก่อนใช้จริง (ดูรายละเอียดในไฟล์ shorts-prompts-ep09.md)

## 🧩 วิธีใช้ Reference Sheet ให้ได้ผลจริง

1.  **Generate ภาพ turnaround sheet ตาม prompt ด้านล่าง** — จะได้ภาพเดียวที่มี 5 panel ในตัว (เต็มตัวหน้า/เต็มตัวข้าง/เต็มตัวหลัง/ครึ่งตัว/ซูมหน้า)

2.  **เช็คความสม่ำเสมอก่อน** — โมเดล generate ภาพยังมีโอกาสทำหน้าแต่ละ panel เพี้ยนไม่ตรงกัน 100% (ข้อจำกัดของ AI image gen ทุกเจ้าในปัจจุบัน) ถ้า panel ไหนหน้าเพี้ยนไปจาก panel อื่นชัดเจน ให้ regenerate ใหม่ทั้งภาพ หรือ crop เฉพาะ panel ที่ดีที่สุดมาใช้

3.  **เลือก panel "เต็มตัวหน้าตรง" เป็น Ingredient หลัก** สำหรับเรียกใช้ @ชื่อ_v1 ทั่วไป

4.  **เก็บ panel อื่นไว้เป็น "Ingredient สำรอง"** — เวลามี scene ที่ต้องถ่ายมุมข้าง/มุมหลัง/close-up หน้าโดยเฉพาะ ให้ crop panel ที่ตรงกับมุมนั้นมาใช้เป็น ingredient ของ scene นั้นแทน จะช่วยให้ Flow คุมมุมกล้อง+หน้าตาได้แม่นกว่าใช้แค่ภาพหน้าตรงภาพเดียวทุกมุม

5.  **Generate Expression Reference Sheet เพิ่ม** (ต่อท้ายทุกคนในไฟล์นี้แล้ว) — เก็บไว้เป็น ingredient สำรองสำหรับ scene ที่มีอารมณ์ชัดเจน (ยิ้ม/เศร้า/เขิน) เพราะแค่หน้าซีเรียสจาก panel เดิมไม่พอบอก Flow ว่า "หน้ายิ้ม" หรือ "หน้าเศร้า" ของคนนั้นควรหน้าตายังไง — crop panel อารมณ์ที่ตรงกับ scene มาใช้แทนภาพหน้าตรงเฉยๆ จะได้ผลแม่นกว่ามาก

## 🎨 Master Style Guide — Universal Quality Baseline

**หลักการ:** บล็อกนี้คือ "มาตรฐานความหล่อ/ความเนี้ยบ" ที่ต้อง**แปะต่อท้ายทุก prompt ตัวละคร** โดยไม่มีข้อยกเว้น — เพื่อให้ทั้ง 10 คนมีคุณภาพภาพเท่ากันหมด (ผิวใส สุขภาพดี ดูแลตัวเองดี) แม้บุคลิกในเรื่องจะต่างกัน:

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail — not plastic or over-smoothed, soft even studio lighting,

consistent lighting and color grade across all panels

**Turnaround Sheet Layout ที่ใช้ในทุก prompt (แปะหัว prompt เสมอ):**

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

neutral expression, sharp focus showing skin texture, eye detail, and

hairstyle clearly.

**หลักการออกแบบ 10 คนให้ต่างกันชัด:** แบ่งเป็น 3 กลุ่มความสูง (175 ซม.ลงมา / 176-180 / 181 ขึ้นไป) และแต่ละคนมีรูปร่าง+ทรงหน้า+ทรงผมที่ไม่ซ้ำกันเลย — ดูตารางสรุปท้ายไฟล์

## 🌇 World Ingredient — บรรยากาศออฟฟิศ PRISM (เหมือนเดิม)

A modern minimalist creative agency office interior in Bangkok, Thailand, on the

14th floor of a glass tower in the Thonglor district, floor-to-ceiling glass windows

letting in soft warm natural daylight, open-plan desks mixed with frosted-glass

meeting rooms, muted beige and glass-blue color palette, contemporary 2026 office

design, photorealistic, editorial photography style, shallow depth of field,

no people in frame, establishing shot

## 👤 Character Reference Turnaround Sheet Prompts (10 คน)

### 1. คิม — Creative Director (คิม × ไอซ์)

**จุดขาย:** หล่อเข้ม สุขุม สายพี่ใหญ่/ซีอีโอ

| **รายละเอียด** | **ค่า** |
|----|----|
| ส่วนสูง / น้ำหนัก | 183 ซม. / 76 กก. |
| รูปร่าง | นักกีฬา-กำยำแบบฟิต ไหล่กว้าง หน้าอกหนา ไม่ใหญ่เทอะทะ |
| หน้า | กรามคมชัดเป็นเหลี่ยม จมูกโด่งได้รูป ตาลึกคมนิ่ง คิ้วเข้มหนาเป็นเส้นตรง ผิวสีแทนอมเหลืองเนียนใส |
| ทรงผม | ผมสั้นทรงเท็กซ์เจอร์ แสกข้างเรียบร้อย ปลายผมยุ่งนิดๆ ให้ดูมีมิติ สีดำสนิท |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

neutral expression, sharp focus showing skin texture, eye detail, and

hairstyle clearly.

Character: a 33-year-old Thai man, Creative Director at an advertising

agency, 183cm tall, 76kg, athletic muscular build with broad shoulders and

a fit toned physique. Sharp angular jawline, high defined nose bridge,

deep-set intense calm eyes, thick straight dark eyebrows, clear olive-tan

skin. Short textured cropped hair with a clean side part, slightly tousled

on top for dimension, jet black hair. Clean-shaven. Wearing a crisp white

button-up dress shirt with sleeves rolled to the forearm, top button undone,

no tie, minimalist analog watch, dark tailored trousers.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral calm resting expression, front-facing.

Panel 2 (top-right): genuine restrained half-smile, subtle warmth in the

eyes.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): quietly concerned expression, brow slightly

furrowed, eyes softer than usual — as close as he gets to looking worried.

Character: a 33-year-old Thai man, Creative Director at an advertising

agency, 183cm tall, 76kg, athletic muscular build with broad shoulders and

a fit toned physique. Sharp angular jawline, high defined nose bridge,

deep-set intense calm eyes, thick straight dark eyebrows, clear olive-tan

skin. Short textured cropped hair with a clean side part, slightly tousled

on top for dimension, jet black hair. Clean-shaven.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

### 2. ไอซ์ — เลขานุการผู้บริหาร (คิม × ไอซ์)

**จุดขาย:** หล่อใสเรียบร้อย สายน้องรัก

| **รายละเอียด** | **ค่า** |
|----|----|
| ส่วนสูง / น้ำหนัก | 175 ซม. / 63 กก. |
| รูปร่าง | สลิมฟิต ไม่ผอมแห้ง มีมัดกล้ามบางๆ พอดูออก |
| หน้า | ตาหวานทรงอัลมอนด์ ชั้นตาสองชั้นชัด จมูกโด่งพอดี ริมฝีปากอิ่มได้รูป ผิวขาวอมชมพูใสมีออร่า |
| ทรงผม | ผมดำนุ่มปัดข้างเบาๆ ปลายผมหยักเล็กน้อย ทรงเรียบร้อยหวีเซ็ตดี |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

neutral expression, sharp focus showing skin texture, eye detail, and

hairstyle clearly.

Character: a 23-year-old Thai man, executive secretary and recent literature

graduate, 175cm tall, 63kg, slim toned build with subtle healthy muscle

definition. Soft almond-shaped eyes with clearly visible double eyelids,

well-proportioned high nose bridge, soft full well-shaped lips, smooth clear

fair skin with a natural warm glow and light blush, gentle defined jawline.

Soft black hair with a light side-swept fringe, slightly wavy ends, neatly

combed and styled. Clean-shaven youthful face. Wearing a modest fitted white

dress shirt tucked into dark tailored trousers, no accessories.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral calm resting expression, front-facing.

Panel 2 (top-right): genuine warm smile, eyes bright and soft.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): shy embarrassed expression with a visible warm

blush across the cheeks, eyes looking slightly away, a bit flustered.

Character: a 23-year-old Thai man, executive secretary and recent literature

graduate, 175cm tall, 63kg, slim toned build with subtle healthy muscle

definition. Soft almond-shaped eyes with clearly visible double eyelids,

well-proportioned high nose bridge, soft full well-shaped lips, smooth clear

fair skin with a natural warm glow and light blush, gentle defined jawline.

Soft black hair with a light side-swept fringe, slightly wavy ends, neatly

combed and styled. Clean-shaven youthful face.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

### 3. เต — ฝ่าย HR (เต × แทน)

**จุดขาย:** หล่ออบอุ่น ยิ้มมีเสน่ห์

| **รายละเอียด** | **ค่า**                                                      |
|---------------|-------------------------------------------------------------|
| ส่วนสูง / น้ำหนัก | 178 ซม. / 72 กก.                                            |
| รูปร่าง         | ฟิตแบบนักกีฬา ไหล่กว้างหนา ดูแข็งแรงอบอุ่น                           |
| หน้า           | ตากลมโตอบอุ่น มีลักยิ้มเวลายิ้ม แก้มมนนิดๆ จมูกโด่งตรง ผิวสีแทนทองสุขภาพดี  |
| ทรงผม         | ผมดำอมน้ำตาลหยักฟูเป็นธรรมชาติ ปลายผมม้วนเล็กน้อย ทรงลุคสบายๆ แต่ดูแลดี |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

smiling naturally with visible dimples, sharp focus showing skin texture,

eye detail, and hairstyle clearly.

Character: a 29-year-old Thai man, HR staff at a creative agency, 178cm

tall, 72kg, athletic build with broader shoulders, strong and warm-looking

physique. Warm round almond eyes, dimples visible when smiling, slightly

rounded cheeks, straight well-shaped nose, tan golden healthy-looking skin.

Short wavy tousled dark brown-black hair with natural texture, slightly

curled at the ends. Light stubble. Wearing a short-sleeve button-down shirt

in a soft pastel color, casual smart-casual trousers.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral calm resting expression, front-facing.

Panel 2 (top-right): big genuine smile with visible dimples, eyes crinkled

with warmth.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): gentle comforting expression, soft caring eyes, head

tilted slightly — the look he gives when checking on someone.

Character: a 29-year-old Thai man, HR staff at a creative agency, 178cm

tall, 72kg, athletic build with broader shoulders, strong and warm-looking

physique. Warm round almond eyes, dimples visible when smiling, slightly

rounded cheeks, straight well-shaped nose, tan golden healthy-looking skin.

Short wavy tousled dark brown-black hair with natural texture, slightly

curled at the ends. Light stubble.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

### 4. แทน — ฝ่าย IT (เต × แทน)

**จุดขาย:** หล่อเย็นชา เนิร์ดหล่อ

| **รายละเอียด** | **ค่า** |
|----|----|
| ส่วนสูง / น้ำหนัก | 181 ซม. / 68 กก. |
| รูปร่าง | สูงเพรียวแบบมีมัดกล้ามซ่อนอยู่ ดูบางแต่แน่น ไม่ใช่ผอมโทรม |
| หน้า | ตาคมทรงจิ้งจอกนิดๆ โหนกแก้มชัด จมูกโด่งตรง ริมฝีปากบางได้รูป ผิวขาวอมเหลืองซีดนิดๆ จากอยู่แต่ในห้อง แต่ยังดูสุขภาพดี |
| ทรงผม | ผมดำทรงยุ่งๆ แบบจัดแต่งให้ดูเท่ (bed-head chic ไม่ใช่ไม่หวี) ใส่แว่นกรอบบางสีเข้ม |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

neutral expression, sharp focus showing skin texture, eye detail, hairstyle,

and glasses clearly.

Character: a 27-year-old Thai man, IT support staff, 181cm tall, 68kg, lean

and lanky build with subtle hidden muscle definition — looks slim but fit,

not frail. Sharp fox-like eyes, high defined cheekbones, straight nose, thin

sculpted lips, healthy fair-tan skin with a slightly pale undertone. Slightly

messy tousled black hair deliberately styled to look effortlessly cool, a

stylish bed-head look. Thin dark-frame rectangular glasses. Clean-shaven.

Wearing a plain fitted dark-colored polo shirt, simple trousers.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral calm resting expression, front-facing.

Panel 2 (top-right): rare small genuine smile, understated but warm.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): quietly worried expression, eyes slightly tired,

looking away as if lost in thought late at night.

Character: a 27-year-old Thai man, IT support staff, 181cm tall, 68kg, lean

and lanky build with subtle hidden muscle definition — looks slim but fit,

not frail. Sharp fox-like eyes, high defined cheekbones, straight nose, thin

sculpted lips, healthy fair-tan skin with a slightly pale undertone. Slightly

messy tousled black hair deliberately styled to look effortlessly cool, a

stylish bed-head look. Thin dark-frame rectangular glasses. Clean-shaven.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

### 5. ภูมิ — หัวหน้าทีม / Project Manager (ภูมิ × ปอนด์)

**จุดขาย:** หล่อบึกบึน สายพี่ใหญ่ผู้นำทีม

| **รายละเอียด** | **ค่า** |
|----|----|
| ส่วนสูง / น้ำหนัก | 180 ซม. / 80 กก. |
| รูปร่าง | ล่ำบึกบึนแบบนักกีฬา ไหล่กว้างหนาที่สุดในกลุ่ม อกหนาแขนใหญ่ |
| หน้า | กรามเหลี่ยมแข็งแรง ตาลึกดุดันแต่มีเมตตา คิ้วหนาเข้ม โหนกแก้มชัด ผิวสีแทนเข้มสุขภาพดี |
| ทรงผม | ผมสั้นเกรียนข้างแบบเฟดสะอาดตา ด้านบนปล่อยยาวนิดหน่อยจัดทรงเนี้ยบ |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

neutral expression, sharp focus showing skin texture, eye detail, and

hairstyle clearly.

Character: a 31-year-old Thai man, project manager at a creative agency,

180cm tall, 80kg, muscular broad-shouldered athletic build — the most

solidly built of the group, thick arms and a strong chest. Strong square

jawline, deep-set steady gaze with a hint of warmth beneath a serious

exterior, thick dark eyebrows, well-defined cheekbones, deep tan healthy

skin. Short hair with clean faded sides and a slightly longer neatly styled

top. Well-groomed light stubble. Wearing a well-fitted simple solid-color

dress shirt, plain leather strap watch, dark trousers.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral calm resting expression, front-facing.

Panel 2 (top-right): confident warm smile, protective and reassuring.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): softened protective expression, gaze gentler than

usual, the look he gives when quietly caring for someone.

Character: a 31-year-old Thai man, project manager at a creative agency,

180cm tall, 80kg, muscular broad-shouldered athletic build — the most

solidly built of the group, thick arms and a strong chest. Strong square

jawline, deep-set steady gaze with a hint of warmth beneath a serious

exterior, thick dark eyebrows, well-defined cheekbones, deep tan healthy

skin. Short hair with clean faded sides and a slightly longer neatly styled

top. Well-groomed light stubble.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

### 6. ปอนด์ — เด็กฝึกงาน / Intern (ภูมิ × ปอนด์)

**จุดขาย:** น่ารักใสซื่อ สายน้องเล็กในกลุ่ม

| **รายละเอียด** | **ค่า** |
|----|----|
| ส่วนสูง / น้ำหนัก | 172 ซม. / 58 กก. |
| รูปร่าง | เพรียวบางแบบวัยรุ่น ตัวเล็กที่สุดในกลุ่มพี่ๆ ยังดูฟิตสุขภาพดี ไม่ผอมแห้ง |
| หน้า | ตากลมโตแบบตาหมา แก้มมนนิดๆ จมูกเล็กได้รูป ริมฝีปากบางน่ารัก ผิวขาวใสไร้สิว |
| ทรงผม | ผมดำทรงมัชรูม หน้าม้าปรกตาเล็กน้อยแบบเด็กมหาลัย |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

neutral expression, sharp focus showing skin texture, eye detail, and

hairstyle clearly.

Character: a 22-year-old Thai man, a university intern studying

communication arts, 172cm tall, 58kg, slender youthful build — the smallest

frame in the group of colleagues, but still looking healthy and lightly

toned, not underweight. Big round puppy-like eyes, softly rounded cheeks,

small well-shaped nose, soft cute thin lips, smooth clear fair skin with no

blemishes. Soft black mushroom-style haircut with a light fringe slightly

covering his forehead. Clean-shaven. Wearing a simple collared polo shirt

slightly oversized, plain casual trousers.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral calm resting expression, front-facing.

Panel 2 (top-right): bright genuine laughing smile, eyes crinkled with joy.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): shy embarrassed expression with a visible blush,

eyes looking slightly away, nervously flustered.

Character: a 22-year-old Thai man, a university intern studying

communication arts, 172cm tall, 58kg, slender youthful build — the smallest

frame in the group of colleagues, but still looking healthy and lightly

toned, not underweight. Big round puppy-like eyes, softly rounded cheeks,

small well-shaped nose, soft cute thin lips, smooth clear fair skin with no

blemishes. Soft black mushroom-style haircut with a light fringe slightly

covering his forehead. Clean-shaven.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

### 7. ฟลุ้ค — Copywriter (เจมส์ × ฟลุ้ค)

**จุดขาย:** หล่อสดใส ตัวสูงยิ้มกว้าง

| **รายละเอียด** | **ค่า** |
|----|----|
| ส่วนสูง / น้ำหนัก | 185 ซม. / 72 กก. (สูงที่สุดในกลุ่ม ตามที่กำหนดไว้ว่าสูงกว่าเจมส์เกือบครึ่งหัว) |
| รูปร่าง | สลิมแอธเลติก ตัวยาวสมส่วน ไหล่กว้างพอดี |
| หน้า | ตายิ้มโค้งสวยมีตีนกามีเสน่ห์ตอนยิ้ม จมูกโด่งสูง ยิ้มกว้างฟันเรียงสวย ผิวสีแทนสุขภาพดี |
| ทรงผม | ผมดำยาวปานกลางหยักฟูเป็นธรรมชาติ ดูมีวอลลุ่ม |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

smiling with visible smile-lines, sharp focus showing skin texture, eye

detail, and hairstyle clearly.

Character: a 26-year-old Thai man, a copywriter at an advertising agency,

185cm tall, 72kg — the tallest in his friend group, slim athletic build

with long well-proportioned limbs and nicely fitting shoulders. Bright

almond-shaped eyes with charming smile-lines, high nose bridge, a wide

genuine smile showing straight white teeth, healthy tan skin. Medium-length

tousled wavy black hair with soft natural volume. Clean-shaven. Wearing a

relaxed oversized button-down shirt, casual trousers.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral calm resting expression, front-facing.

Panel 2 (top-right): wide genuine laughing smile, eyes crinkled with joy,

teeth showing.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): shy embarrassed expression with a visible blush,

caught off guard, eyes looking slightly away.

Character: a 26-year-old Thai man, a copywriter at an advertising agency,

185cm tall, 72kg — the tallest in his friend group, slim athletic build

with long well-proportioned limbs and nicely fitting shoulders. Bright

almond-shaped eyes with charming smile-lines, high nose bridge, a wide

genuine smile showing straight white teeth, healthy tan skin. Medium-length

tousled wavy black hair with soft natural volume. Clean-shaven.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

### 8. เจมส์ — Art Director (Junior-Mid) (เจมส์ × ฟลุ้ค)

**จุดขาย:** หล่อเท่นิ่งขรึม มินิมอล

| **รายละเอียด** | **ค่า** |
|----|----|
| ส่วนสูง / น้ำหนัก | 175 ซม. / 67 กก. (เตี้ยกว่าฟลุ้คพอสังเกตได้ ตามที่กำหนดในเรื่อง) |
| รูปร่าง | สลิมฟิตแน่น กระชับ ไม่ใหญ่โต แต่ดูมีมัดกล้าม |
| หน้า | ตาคมเข้มดูจริงจังตลอดเวลา จมูกโด่งตรง กรามชัดแต่ไม่บึกบึน ริมฝีปากบางมักเม้มปากนิ่งๆ ผิวสีแทนอ่อนเนียนใส |
| ทรงผม | ผมดำสั้นตรงทรงโมเดิร์นเรียบร้อย ไม่มีหน้าม้า |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

neutral serious expression, sharp focus showing skin texture, eye detail,

and hairstyle clearly.

Character: a 28-year-old Thai man, a junior-to-mid level art director, 175cm

tall, 67kg — noticeably shorter than his tall colleague but still

well-proportioned, lean toned compact build with visible but understated

muscle definition. Sharp intense narrow eyes that always look focused,

straight defined nose, a sharp but not overly broad jawline, thin lips

usually held in a neutral serious expression, clear fair-tan skin. Short

straight black hair in a clean modern crop with no fringe. Clean-shaven.

Wearing a fitted plain black or charcoal grey t-shirt, simple trousers.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral serious resting expression, front-facing.

Panel 2 (top-right): rare small restrained smile, subtle and understated,

just a slight lift at the corner of the mouth.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): quietly restrained caring expression, eyes softer

than usual, a faint hint of concern he tries not to show.

Character: a 28-year-old Thai man, a junior-to-mid level art director, 175cm

tall, 67kg — noticeably shorter than his tall colleague but still

well-proportioned, lean toned compact build with visible but understated

muscle definition. Sharp intense narrow eyes, straight defined nose, a sharp

but not overly broad jawline, thin lips, clear fair-tan skin. Short straight

black hair in a clean modern crop with no fringe. Clean-shaven.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

### 9. ดิว — Graphic Designer (ดิว × นนท์)

**จุดขาย:** หล่อศิลปิน สายตาคม

| **รายละเอียด** | **ค่า**                                                      |
|---------------|-------------------------------------------------------------|
| ส่วนสูง / น้ำหนัก | 174 ซม. / 61 กก.                                            |
| รูปร่าง         | สลิมบางแบบศิลปิน ไม่มีกล้ามชัดแต่ดูสุขภาพดี ท่าทางผ่อนคลาย               |
| หน้า           | ตาคมทรงแมวโฟกัสจริงจัง จมูกโด่งตรง กรามได้รูปแต่ไม่แข็งกร้าว ผิวขาวเนียน |
| ทรงผม         | ผมดำตรงยาวปรกลงมาปิดตาข้างนึงเล็กน้อย ทรงลุคศิลปิน                  |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

focused neutral expression, sharp focus showing skin texture, eye detail,

and hairstyle clearly.

Character: a 27-year-old Thai man, a graphic designer, 174cm tall, 61kg,

slim artistic build with a relaxed unhurried posture — no heavy muscle

definition but still looking healthy and well cared for. Sharp focused

cat-like eyes, straight nose, a defined yet soft jawline, smooth fair skin.

Straight black hair falling slightly over one eye, casually styled in an

artistic look. Clean-shaven. Wearing an old pair of worn over-ear

headphones with a slightly frayed cable, casual oversized graphic t-shirt

or hoodie.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral focused resting expression, front-facing.

Panel 2 (top-right): soft genuine smile, gentle and understated.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): sleepy exhausted expression, eyes half-closed,

peaceful and relaxed as if about to drift off.

Character: a 27-year-old Thai man, a graphic designer, 174cm tall, 61kg,

slim artistic build with a relaxed unhurried posture — no heavy muscle

definition but still looking healthy and well cared for. Sharp focused

cat-like eyes, straight nose, a defined yet soft jawline, smooth fair skin.

Straight black hair falling slightly over one eye, casually styled in an

artistic look. Clean-shaven.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

### 10. นนท์ — Motion Graphic Designer (ดิว × นนท์)

**จุดขาย:** น่ารักเด็กกว่า อบอุ่นละมุน

| **รายละเอียด** | **ค่า**                                                    |
|---------------|-----------------------------------------------------------|
| ส่วนสูง / น้ำหนัก | 170 ซม. / 56 กก. (เตี้ยที่สุดในกลุ่ม เด็กสุดในกลุ่ม)                 |
| รูปร่าง         | เพรียวบางละมุน ตัวเล็กพอดี ดูสุขภาพดีไม่ผอมโทรม                    |
| หน้า           | ตากลมอ่อนโยน คางมนนุ่มนวล จมูกเล็กพอดี แก้มนุ่มดูละมุน ผิวสีแทนอ่อนเนียน |
| ทรงผม         | ผมดำสั้นฟูเป็นธรรมชาติแบบทรงเด็กหนุ่ม                             |

A character reference turnaround sheet for a video production, arranged as

5 clearly separated panels on a plain neutral light-grey studio background,

consistent soft even studio lighting across all panels, same character in

every panel:

Panel 1 (top-left): full body front view, standing relaxed neutral pose,

arms at sides.

Panel 2 (top-right): full body side profile view, same standing pose.

Panel 3 (middle-left): full body back view, same standing pose.

Panel 4 (middle-right): half-body waist-up three-quarter view.

Panel 5 (bottom, larger): close-up detail shot of the face only, front-facing,

gentle calm expression, sharp focus showing skin texture, eye detail, and

hairstyle clearly.

Character: a 24-year-old Thai man, a motion graphic designer, 170cm tall,

56kg — the shortest and youngest-looking in the group, slender gentle build

that still looks healthy and well cared for, not frail. Soft round gentle

eyes, a soft rounded jawline, small well-proportioned nose, soft cheeks

giving a gentle warm impression, smooth light-tan skin. Short naturally

fluffy black hair with a boyish youthful texture. Clean-shaven. Wearing

simple affordable in-ear headphones, casual plain t-shirt with a light

jacket.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, fit and healthy toned physique with good upright posture,

bright alert expressive eyes, polished K-drama/Thai-BL leading-man aesthetic,

the kind of striking handsome first impression that immediately draws

attention, photorealistic rendering, natural skin texture with fine

realistic detail, soft even studio lighting, consistent lighting and color

grade across all panels

**🎭 Expression Reference Sheet (เสริม):**

A character facial expression reference sheet for a video production,

arranged as 4 clearly separated close-up panels on a plain neutral

light-grey studio background, consistent soft even studio lighting across

all panels, same character in every panel, face and shoulders only:

Panel 1 (top-left): neutral calm resting expression, front-facing.

Panel 2 (top-right): gentle warm smile, soft and shy.

Panel 3 (bottom-left): sad emotional expression, eyes slightly downcast and

misty, subdued mood.

Panel 4 (bottom-right): quietly caring expression, gaze directed slightly

sideways as if watching over someone, tender and attentive.

Character: a 24-year-old Thai man, a motion graphic designer, 170cm tall,

56kg — the shortest and youngest-looking in the group, slender gentle build

that still looks healthy and well cared for, not frail. Soft round gentle

eyes, a soft rounded jawline, small well-proportioned nose, soft cheeks

giving a gentle warm impression, smooth light-tan skin. Short naturally

fluffy black hair with a boyish youthful texture. Clean-shaven.

flawless clear radiant skin with healthy natural glow, no blemishes or dark

circles, camera-ready photogenic bone structure, impeccably groomed and neat

overall styling, bright alert expressive eyes, polished K-drama/Thai-BL

leading-man aesthetic, photorealistic rendering, natural skin texture with

fine realistic detail, soft even studio lighting, consistent lighting and

color grade across all panels

## 📊 ตารางสรุป — เช็คความแตกต่างในแว้บเดียว

| **\#** | **ชื่อ** | **ส่วนสูง** | **น้ำหนัก** | **รูปร่างเด่น** | **จุดเด่นหน้า** | **ทรงผม** |
|----|----|----|----|----|----|----|
| 1 | คิม | 183 ซม. | 76 กก. | อกหนาไหล่กว้าง | กรามเหลี่ยม ตาลึกนิ่ง | สั้นเท็กซ์เจอร์แสกข้าง |
| 2 | ไอซ์ | 175 ซม. | 63 กก. | สลิมฟิต | ตาหวานสองชั้น | นุ่มปัดข้าง |
| 3 | เต | 178 ซม. | 72 กก. | ฟิตอบอุ่น | ตากลมมีลักยิ้ม | หยักฟูธรรมชาติ |
| 4 | แทน | 181 ซม. | 68 กก. | เพรียวสูง | ตาคมทรงจิ้งจอก+แว่น | ยุ่งจัดทรงเท่ |
| 5 | ภูมิ | 180 ซม. | 80 กก. | ล่ำบึกบึนสุด | กรามเหลี่ยมแข็งแรง | เกรียนข้างเฟด |
| 6 | ปอนด์ | 172 ซม. | 58 กก. | เพรียวเล็กสุดในพี่ๆ | ตากลมแบบตาหมา | มัชรูมหน้าม้า |
| 7 | ฟลุ้ค | 185 ซม. | 72 กก. | สูงสุดในกลุ่ม | ยิ้มกว้างตีนกา | ยาวปานกลางหยักฟู |
| 8 | เจมส์ | 175 ซม. | 67 กก. | กระชับแน่น | ตาคมจริงจัง | สั้นตรงไม่มีหน้าม้า |
| 9 | ดิว | 174 ซม. | 61 กก. | สลิมศิลปิน | ตาคมทรงแมว | ยาวปรกตาข้างนึง |
| 10 | นนท์ | 170 ซม. | 56 กก. | เล็ก-เด็กสุด | ตากลมอ่อนโยน | สั้นฟูธรรมชาติ |

## 🎥 Scene / Video Prompt Template

โครงสร้าง SCAM (Subject, Composition, Action, Mood) และตัวอย่าง scene พร้อมใช้ อยู่ในไฟล์ shorts-prompts-ep09.md — เมื่อ generate reference turnaround sheet ครบ 10 คนแล้ว crop panel ที่เหมาะกับแต่ละ scene มาทำ ingredient ได้เลย (ดูหัวข้อ "วิธีใช้ Reference Sheet" ด้านบน)

## 📌 Checklist

- Generate Reference Turnaround Sheet ทั้ง 10 คนตาม prompt ชุดนี้

  Generate Expression Reference Sheet ทั้ง 10 คน (นิ่ง/ยิ้ม/เศร้า/อารมณ์เฉพาะตัว) ต่อจากข้อ 1

  เช็คความสม่ำเสมอของหน้าในแต่ละ panel ทั้งสองชุด — ถ้าเพี้ยน regenerate ใหม่

  Crop panel "เต็มตัวหน้าตรง" เก็บเป็น Ingredient หลักของแต่ละคน

  Crop panel มุมข้าง/มุมหลัง/ซูมหน้า/อารมณ์ต่างๆ เก็บแยกไว้เป็น ingredient สำรองสำหรับ scene ที่ต้องใช้มุม/อารมณ์นั้นโดยเฉพาะ

  เทียบภาพทั้ง 10 คนกับตารางสรุปด้านบน เช็คว่าไม่มีใครหน้าคล้ายกันเกินไป

  อัปเดต URL/asset name ใหม่ (ภาพหลัก + มุมสำรอง + อารมณ์สำรอง) ลงใน character-seeds.md
