# 🌟 สะสมดาว — ดาวของหนู (Starlight Leai)

> **แอปรางวัลดาวสำหรับครอบครัว 100% ฟรีตลอดชีพ**
>
> เปลี่ยนการทำงานบ้านและการฝึกเขียนเป็นดาวสะสม พร้อมมาสคอต "น้องดาว" ที่พูดได้ สำหรับเด็กอายุ 3-10 ปี

🌐 **เว็บไซต์**: <https://lexcorpseo.github.io/Starlight-Leai/>

---

## 💯 Free Forever Pledge (สัญญาว่าฟรีจริง)

| ✅ สัญญา | ❌ ไม่ทำ |
|---|---|
| ฟรี 100% ตลอดชีพ | ไม่มีค่าใช้จ่ายรายเดือน/รายปี |
| ไม่มีโฆษณาในแอป | ไม่มีการล็อกฟีเจอร์ไว้ให้จ่ายปลดล็อก |
| ข้อมูลเก็บใน Firebase ของคุณ | ไม่เก็บข้อมูลเด็กไปขาย |
| ส่งออกข้อมูล JSON ได้ตลอดเวลา | ไม่มี lock-in |
| เปิดโค้ด (เป็นไปได้ในอนาคต) | — |

อ่านเพิ่ม: [docs/FREE_FOREVER_PLEDGE.md](docs/FREE_FOREVER_PLEDGE.md)

---

## ✨ ฟีเจอร์เด่น

### 🎯 สำหรับเด็ก
- **📋 งานประจำวัน** — แปรงฟัน, เก็บของเล่น, ทำการบ้าน ฯลฯ (ปรับแต่งได้)
- **✍️ ฝึกเขียน** — ชื่อภาษาไทย, ชื่อภาษาอังกฤษ, ตัวเลข 0-20 พร้อมเส้นลากตาม
- **🤝 ภารกิจคู่** — กิจกรรมพ่อแม่-ลูก ที่ทำด้วยกัน
- **🎡 วงล้อกิจกรรม** — หมุนวันละ 3 ครั้ง รับกิจกรรมเซอร์ไพรส์
- **🎁 รางวัล** — สะสมดาวแลกรางวัลที่ผู้ปกครอกตั้งไว้
- **💌 ส่งข้อความถึงพ่อแม่** — ส่งอีโมจิ "หอมแก้ม" "รักพ่อแม่" ได้

### 👨‍👩‍👧 สำหรับผู้ปกครอก
- **🔒 โหมดผู้ปกครอกล็อกด้วย PIN** — ป้องกันเด็กแก้ตั้งค่า
- **📊 สรุปดาว 14 วัน** — กราฟแท่งแสดงความก้าวหน้า
- **🔥 Streak** — ติดตามการทำงานต่อเนื่อง
- **🎯 เป้าหมายสัปดาห์** — 10/15/20/30 ดาว
- **📤 ส่งออก/นำเข้า JSON** — สำรองข้อมูลได้

### 🆕 ฟีเจอร์ใหม่ (ในรุ่นนี้)
- **🎤 ให้ดาวด้วยเสียง** — พูด "ให้ดาว มานี 2 ดาว" แล้วระบบให้ให้อัตโนมัติ (Web Speech API)
- **☁️ สถานะการเชื่อมต่อ** — Pill แสดงสถานะออนไลน์/ออฟไลน์/กำลังซิงค์
- **📤 การ์ดดาวแชร์ได้** — สร้างภาพสรุปดาวประจำสัปดาห์แชร์ Facebook/LINE ได้
- **🌙 มาสคอต Lottie 5 สถานะ** — Idle/Cheer/Confused/Sad/Sleepy (พร้อมโหลด)
- **🔍 SEO ครบชุด** — JSON-LD Schema, OG tags, semantic HTML

---

## 🚀 เริ่มต้นใช้งาน

### สำหรับผู้ใช้ทั่วไป
1. เปิด <https://lexcorpseo.github.io/Starlight-Leai/> บนเบราว์เซอร์ (แนะนำ Chrome)
2. ล็อกอินด้วย Google หรือ Email
3. ยืนยันอีเมล (ถ้าล็อกอินด้วย Email)
4. สร้างโปรไฟล์เด็ก — เลือกอวตาร + ใส่ชื่อ
5. เริ่มเล่นได้เลย! 🎉

**ติดตั้งเป็นแอป** (PWA):
- Android Chrome: เมนู ⋮ → "ติดตั้งแอป"
- iOS Safari: ปุ่มแชร์ → "เพิ่มไปยังหน้าจอโฮม"

### สำหรับนักพัฒนา (Developer)

```bash
# Clone
git clone https://github.com/lexcorpseo/Starlight-Leai.git
cd Starlight-Leai

# ไม่ต้อง install — เป็น static HTML
# เปิดด้วย local server ใดก็ได้
python3 -m http.server 8000
# หรือ
npx serve .

# เปิด http://localhost:8000 ในเบราว์เซอร์
```

**Firebase Setup**:
- แอปใช้ Firebase ของเจ้าของ repo อยู่แล้ว
- ถ้าจะรัน fork ของตัวเอง ต้องสร้าง Firebase project ใหม่และแก้ config ใน `index.html` (บรรทัดที่มี `firebaseConfig`)

---

## 🛠️ เทคโนโลยี

| Layer | เทคโนโลยี |
|---|---|
| Frontend | HTML, CSS, Vanilla JavaScript (เป็น Single-file PWA) |
| Backend | Firebase Authentication |
| Database | Cloud Firestore |
| Hosting | GitHub Pages (ฟรี) |
| PWA | Web App Manifest + Service Worker |
| Animation | CSS Keyframes + Lottie (สำหรับ mascot) |
| TTS | Web Speech API |
| Voice Input | Web Speech Recognition API (Chrome only) |
| Image Gen | Canvas API (สำหรับ Share Card) |

---

## 📁 โครงสร้างไฟล์

```
Starlight-Leai/
├── index.html                  ← ไฟล์หลัก (Single-file PWA)
├── manifest.json               ← PWA manifest
├── icon-192.png                ← PWA icon
├── apple-touch-icon-180.png    ← iOS icon
├── assets/
│   ├── img/
│   │   ├── og-image.png        ← Open Graph image
│   │   ├── mascot-preview.png  ← Mascot ในท่า idle
│   │   ├── mascot-cheer.png    ← Mascot ในท่า cheer
│   │   └── mascot-sleepy.png   ← Mascot ในท่า sleepy
│   └── lottie/
│       ├── mascot-idle.json    ← Lottie IDLE state
│       ├── mascot-cheer.json   ← Lottie CHEER state
│       ├── mascot-confused.json
│       ├── mascot-sad.json
│       ├── mascot-sleepy.json
│       └── README.md           ← วิธีแทนที่ด้วย Lottie จริง
├── .github/
│   ├── workflows/
│   │   └── deploy.yml          ← GitHub Pages auto-deploy
│   └── ISSUE_TEMPLATE/
│       ├── bug-report.yml
│       ├── feature-request.yml
│       └── parent-feedback.yml
├── docs/
│   ├── FREE_FOREVER_PLEDGE.md
│   ├── MASCOT_PROMPT.md        ← Prompt สำหรับ AI image gen
│   ├── PRIVACY_POLICY.md
│   └── CHANGELOG.md
├── robots.txt
├── sitemap.xml
├── README.md                   ← (ไฟล์นี้)
├── CONTRIBUTING.md
├── LICENSE
└── .gitignore
```

---

## 🤝 ร่วมพัฒนา

อ่าน [CONTRIBUTING.md](CONTRIBUTING.md) ก่อนส่ง PR

### รายการที่ยินดีรับความช่วยเหลือ
- 🐛 แจ้งบั๊ก: ใช้ template [Bug Report](.github/ISSUE_TEMPLATE/bug-report.yml)
- 💡 เสนอฟีเจอร์: [Feature Request](.github/ISSUE_TEMPLATE/feature-request.yml)
- 💌 ผู้ปกครอก feedback: [Parent Feedback](.github/ISSUE_TEMPLATE/parent-feedback.yml)
- 🔧 ส่ง PR: ใช้ [PR Template](.github/PULL_REQUEST_TEMPLATE.md)

### กฎการทำงานร่วมกัน
1. **เคารพเด็กและครอบครัว** — ทุกฟีเจอร์ต้องปลอดภัยสำหรับเด็ก
2. **ไม่มีโฆษณา ไม่มี tracking** — ไม่เพิ่ม Google Analytics หรือ ads
3. **Privacy first** — ไม่เก็บข้อมูลที่ไม่จำเป็น
4. **Free Forever** — ห้ามเพิ่มฟีเจอร์ที่ต้องจ่ายเงิน
5. **Accessibility** — รองรับ screen reader, มี ARIA labels

---

## 📊 แผนพัฒนา (Roadmap)

### ✅ รุ่นปัจจุบัน (v2.0)
- [x] SEO enhancement + JSON-LD
- [x] Voice Star Giving
- [x] Cloud Status Pill
- [x] Share Card Generator
- [x] Free Forever Pledge section
- [x] Lottie mascot placeholder (5 states)

### 🚧 รุ่นถัดไป (v2.1)
- [ ] Lottie mascot จริง (ส่งออกจาก After Effects)
- [ ] Bedtime Story Mode (LLM สร้างนิทานจากดาวประจำวัน)
- [ ] PWA Push Notification (เตือนทำงานบ้าน)
- [ ] LINE Notify (ส่งสรุปดาวรายสัปดาห์)
- [ ] Smart Task Suggestion

### 🔮 อนาคต (v3.0)
- [ ] Migration ไป Next.js 14
- [ ] Firestore subcollections
- [ ] AR Star Projection
- [ ] Constellation Map
- [ ] Referral Loop + Sticker Trading

อ่านเพิ่ม: [docs/ROADMAP.md](docs/ROADMAP.md)

---

## 🔒 ความเป็นส่วนตัว

อ่าน [docs/PRIVACY_POLICY.md](docs/PRIVACY_POLICY.md)

**สรุปสั้นๆ**:
- ไม่เก็บข้อมูลที่ไม่จำเป็น
- ไม่ใช้ Google Analytics (อาจใช้ Plausible แบบ privacy-first ในอนาคต)
- ข้อมูลเก็บใน Firebase ของเจ้าของบัญชี
- ส่งออก/ลบข้อมูลได้ตลอดเวลา
- ไม่ฝากข้อมูลเด็กไปยังบุคคลที่สาม

---

## 📄 License

MIT License — ดูรายละเอียดใน [LICENSE](LICENSE)

---

## 💖 สนับสนุน

ถ้าแอปนี้มีประโยชน์กับครอบครัวคุณ สามารถ:
- ⭐ กด Star repo นี้
- 💌 ส่ง feedback ที่ [Issues](https://github.com/lexcorpseo/Starlight-Leai/issues)
- 📢 แชร์ให้ครอบครัวอื่นรู้จัก
- ☕ สนับสนุนผ่าน Ko-fi (link มาเร็วๆ นี้)

**ไม่บังคับ ไม่กัด** — แอปนี้ฟรีตลอดชีพ ไม่ว่าจะสนับสนุนหรือไม่ก็ตาม 💛

---

## 🙏 ขอบคุณ

- ครอบครัวทุกครอบครัวที่ใช้แอปนี้
- ทีม Firebase ที่ให้ BaaS ฟรี
- GitHub ที่ให้ Pages ฟรี
- Google Fonts ที่ให้ Baloo Thai 2 + Mali ฟรี
- LottieFiles ที่ให้ Lottie player ฟรี

---

Made with 💛 for Thai families
