# Speakline — Minimalist English Speaking Practice & Teleprompter

**Speakline** — Ingliz tili nutqini (speaking fluency) rivojlantirish uchun mo'ljallangan minimalist va estetik veb-ilova.

Saytga kirgan foydalanuvchiga 10 ta hissiy va motivatsion mavzu tanlash imkoniyati beriladi. Mavzu tanlanganda ayol diktor **"Speak fast and clear"** jumlasini o'qiydi va matn ko'z fokus chizig'i bo'ylab to'xtovsiz, silliq (smooth) yuqoriga harakatlanishni boshlaydi.

---

## ✨ Asosiy Imkoniyatlar

1. **Sof Oq va Minimalist Dizayn:**
   - Hech qanday keraksiz emojilar yoki axmoqona piktogrammalarsiz, toza Apple/Substack editorial tipografiyasi.
   - Yuqori kontrastli matnlar, qulay bo'shliqlar va to'liq Responsive dizayn (mobil, planshet, kompyuter).

2. **10 Ta Hissiy & Motivatsion Mavzular (A1, A2, B1):**
   - Matnlar insonga dalda beradigan, siqilganda kirib o'qiydigan va to'g'ridan-to'g'ri kitobxonga ("You") murojaat qiladigan qilib yozilgan.
   - Har bir qator aniq **4 ta so'zdan** iborat bo'lib, ko'z va nutq ritmi uchun qulay kadansni ta'minlaydi.

3. **To'xtovsiz va Silliq Teleprompter (Continuous Linear Scroll):**
   - Qatorma-qator yoki so'zma-so'z sakrashlar butunlay olib tashlangan.
   - Hardware-accelerated GPU rendering (`translate3d` va `requestAnimationFrame`) orqali 60 FPS silliqlikda bir maromda yuqoriga oqib boradi.
   - Ko'z qaratilishi kerak bo'lgan joyda nozik **gorizontal fokus chizig'i** mavjud.

4. **Kengaytirilgan Tezlik Sozlamasi (Maksimal 260 WPM):**
   - 60 dan 260 WPM gacha bo'lgan tezlik slayderi (presets: 80, 140, 200, 260 WPM).
   - O'qish jarayonining o'zida ham pastki suzuvchi paneldan tezlikni o'zgartirish yoki bir harakatda to'xtatish (pause) mumkin.

5. **"Speak fast and clear" Ovozli Start & Diktofon:**
   - Boshlash tugmasi bosilganda yoqimli ayol ovozi "Speak fast and clear" deydi.
   - O'qish paytida ovozni yozib olib, yakunda o'z nutqini eshitib tekshirish imkoniyati (MediaRecorder).

6. **Har Bir Mavzu Bo'yicha Lug'at (Key Words):**
   - 10 tadan eng muhim so'zlar va ularning o'zbekcha tarjimasi, bosilganda to'g'ri inglizcha talaffuz eshittiriladi.

---

## 🚀 Ishga Tushirish

### Node.js server orqali:
```bash
node server.js
```
Brauzerda oching: `http://localhost:3000`

### To'g'ridan-to'g'ri brauzerda:
`index.html` faylini istalgan brauzerda ikki marta bosib ochish kifoya.

---

## 📁 Loyiha Strukturasi

```
Malika-English/
├── index.html                               # Asosiy toza minimalist veb-ilova
├── speakline_english_speaking_practice.html # Sinxron nusxa
├── server.js                                # Node.js local server (Port 3000)
├── package.json                             # Loyiha ma'lumotlari
└── README.md                                # Qo'llanma
```
