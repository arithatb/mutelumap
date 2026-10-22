# 🗺️ MUTELU MAP THAILAND — TRILINGUAL USER MANUAL & PRODUCTION DEPLOYMENT GUIDE
## คู่มือการใช้งาน 3 ภาษา (ไทย / English / 简体中文) และคู่มือการนำเว็บแอปไปเปิดให้คนนอกใช้งานจริง

---

## 📦 ไฟล์ในชุดส่งออกใช้งานจริง (`mutelu_map_deploy_package.zip`)
1. **`index.html` และ `Mutelu_Map_Thailand_Standalone.html`**
   - ไฟล์เว็บแอปพลิเคชันฉบับสมบูรณ์ (Standalone Production Build) ที่รวมโค้ด, ข้อมูลสถานที่มูเตลูทั่วไทย, ระบบสลับ 3 ภาษา (ไทย / อังกฤษ / จีน), คู่มือการใช้งาน 3 ภาษา, ระบบ AI จัดทริปสายมู และ QR Code พร้อมเพย์ 9 บาท ไว้ในไฟล์เดียว
   - **วิธีใช้งานแบบเร็วที่สุด:** ส่งไฟล์ `Mutelu_Map_Thailand_Standalone.html` ให้เพื่อนหรือผู้ใช้งานทาง LINE / Google Drive / Email ผู้รับสามารถดับเบิลคลิกเปิดใช้งานบนเบราว์เซอร์ได้ทันทีทั้งบน Windows, macOS, Android และ iOS!
2. **`manifest.json`**
   - ไฟล์ตั้งค่า Progressive Web App (PWA) สำหรับให้ผู้ใช้งานกด **Add to Home Screen (เพิ่มไปยังหน้าจอโฮม)** บน iPhone, iPad, Android และคอมพิวเตอร์
3. **`src/App.jsx`**
   - ซอร์สโค้ด React Component ฉบับเต็ม สำหรับนักพัฒนาที่ต้องการนำไปต่อยอดในโปรเจกต์ Vite / Next.js

---

## 🌐 วิธีนำเว็บแอปขึ้นออนไลน์ให้คนทั้งประเทศใช้งานฟรี (ใช้เวลาเพียง 30 วินาที!)
### วิธีที่ 1: อัปโหลดผ่าน Netlify Drop (แนะนำ — เร็วและฟรี)
1. แตกไฟล์ `mutelu_map_deploy_package.zip` ออกมาเป็นโฟลเดอร์บนคอมพิวเตอร์
2. เปิดเว็บไซต์ **[https://app.netlify.com/drop](https://app.netlify.com/drop)**
3. ลากโฟลเดอร์ที่แตกไฟล์แล้วไปวางในกรอบบนหน้าเว็บ Netlify Drop
4. ระบบจะสร้างลิงก์เว็บไซต์สาธารณะ (`https://...netlify.app`) ให้ทันที สามารถเปลี่ยนชื่อลิงก์และแชร์ลง Facebook, TikTok, LINE ให้คนนอกเข้าใช้งานได้ทั่วโลก!

### วิธีที่ 2: อัปโหลดผ่าน Vercel หรือ GitHub Pages
- นำไฟล์ `index.html` และ `manifest.json` ขึ้น GitHub Repository แล้วเปิดใช้งาน **GitHub Pages** หรือเชื่อมต่อกับ **Vercel** ได้ฟรี

---

## 🇹🇭 1. คู่มือการใช้งานภาษาไทย (Thai User Manual)
1. **การเปลี่ยนภาษา (ไทย / EN / 中文):** กดปุ่มเลือกภาษา `🇹🇭 ไทย` | `🇬🇧 EN` | `🇨🇳 中文` ที่แถบด้านบนขวาของจอ หรือในหน้าคู่มือการใช้งาน เพื่อสลับภาษาของทั้งเว็บไซต์และคู่มือได้ทันที
2. **การสำรวจแผนที่ประเทศไทย:** คลิกเลือกจังหวัดบนแผนที่ประเทศไทยทางซ้ายมือ หรือกรองตามสายพร (โชคลาภ, การงาน, ความรัก, สุขภาพ) และสลับโหมด `เช็คคนแน่น` เพื่อดูระดับความหนาแน่นของผู้คน
3. **การดูคาถาบูชา & นำทาง Google Maps:** ในการ์ดสถานที่แต่ละแห่ง กดปุ่ม `คัดลอกคาถา` เพื่อก๊อปปี้บทสวด กดปุ่ม `ขั้นตอนการมู` เพื่อดูจำนวนธูป/ของไหว้ และกดปุ่มสีเขียว `นำทาง Google Maps` เพื่อเปิดแผนที่นำทางไปถึงหน้าวัด
4. **ชุมชนมูกระซิบ (อัปเดตคิว/ที่จอดรถพร้อมรูปถ่าย):** เข้าแท็บ `มูกระซิบ` เพื่ออ่านรีวิวสถานการณ์จริงจากเพื่อนสายมู หรือกดโพสต์ข้อความพร้อมแนบรูปถ่ายจากมือถือของคุณ
5. **AI วางแผนทริปสายมู (One Day Trip / หลายวัน):** เข้าแท็บ `ทริปมูของฉัน` (เริ่มต้นเป็นหน้าว่าง) เลือกจังหวัด อำเภอ สายพร และจำนวนวัน แล้วกดให้ AI สร้างตารางทริปรายชั่วโมงพร้อม Dashboard รูปสถานที่จริง
6. **ร่วมบุญสนับสนุนพัฒนาแอป 9 บาท:** กดปุ่ม `🙏 ร่วมสนับสนุนพัฒนาแอป 9 บาท` เพื่อสแกน QR Code พร้อมเพย์ และรับคำอวยพรเซียมซีเลขมงคล 9

---

## 🇬🇧 2. English User Manual
1. **Language Switching (TH / EN / ZH):** Click the `🇹🇭 ไทย` | `🇬🇧 EN` | `🇨🇳 中文` toggle in the top header bar (or inside the User Manual tab) to switch the entire interface and user manual language instantaneously.
2. **Interactive Thailand Map Explorer:** Click or tap any province on the Thailand SVG map, filter by blessing category (Wealth, Career, Love, Health), or switch to `Crowd Radar` mode to inspect real-time visitor density.
3. **Sacred Chants, Ritual Guide & Google Maps Navigation:** On any temple card, click `Copy Sacred Chant` to copy prayers, `Ritual & Offerings Guide` for step-by-step worship instructions, or the green `Google Maps Nav` button for turn-by-turn GPS navigation.
4. **Mu-Krasib Live Community:** Visit the `Mu-Krasib Reviews` tab to check live queue times and parking tips, or upload your own live photos from your smartphone.
5. **AI Smart Trip Planner:** Open the `AI Trip Planner` tab, select your desired Province, District, Blessing Focus, and Trip Duration (`One Day Trip`, `2 Days 1 Night`, or `3 Days 2 Nights`), and let AI generate a visual itinerary dashboard.
6. **Cross-Platform Install & 9 THB Merit Support:** Click `Install on Win / Mac / Android / iOS` for home-screen installation instructions, or click `Support Dev 9 THB` to support server maintenance via PromptPay QR and draw an auspicious fortune stick.

---

## 🇨🇳 3. 中文使用手册 (Simplified Chinese User Manual)
1. **多语言一键切换（泰语 / 英语 / 简体中文）：** 点击顶部导航栏或使用手册页面中的 `🇹🇭 ไทย` | `🇬🇧 EN` | `🇨🇳 中文` 按钮，即可实时切换全站界面与使用手册语言。
2. **泰国祈福互动地图：** 点击左侧泰国地图上的任意府份板块，或按祈福类别（💰招财、💼事业、❤️姻缘、🛡️健康平安）筛选灵验圣地；还可切换“实时人流热力”查看各府寺庙拥挤程度。
3. **参拜经文、供品指南与 Google 地图导航：** 在寺庙卡片上点击“复制参拜经文”可复制礼佛咒语，点击“参拜步骤与供品指南”查看上香支数与供品要求，点击绿色“Google 地图导航”按钮即可一键开启导航直达寺庙。
4. **“信众耳语”实况社区：** 出发前查看善信发布的排队时长与隐藏停车场位置，也可直接上传手机拍摄的现场照片分享实况。
5. **AI 智能祈福行程规划：** 进入“AI 智能祈福行程”页面，选择目的地府份、县区、祈福方向与行程天数（一日游 / 2天1夜 / 3天2夜），AI 将自动生成顺路的时间表与实景照片看板。
6. **全平台安装与 9 泰铢随喜功德赞助：** 点击顶部安装按钮查看 iOS、安卓、Windows 及 macOS 的桌面安装步骤；点击“随喜赞助开发者 9 泰铢”可扫描泰国 PromptPay 二维码支持应用维护并抽取吉祥九号灵签。
