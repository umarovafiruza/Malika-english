# 🎓 Speakline — English Speaking Practice & Teleprompter

**Speakline** — Ingliz tili nutqini oshirish, teleprompter orqali matnlarni ravon o'qish, diktofon orqali o'z ovozini yozib olib tahlil qilish hamda har bir mavzu bo'yicha 10 tadan qiyin so'zlarni diktor yordamida tinglab o'rganish uchun mo'ljallangan zamonaviy EdTech veb-ilovasi.

Ilova dizayni zamonaviy **Chegg / Duolingo / iOS** mobil ilovalari estetikasida (pastel ranglar, yorqin to'q sariq aksentlar, suzuvchi navigatsiya paneli) yaratilgan.

---

## ✨ Asosiy Imkoniyatlar

1. **CEFR Darajalari (A1, A2, B1):**
   - Ilovaga kirish bilanoq yuqorida `A1 • Beginner`, `A2 • Elementary`, `B1 • Intermediate` darajalari ko'rinadi.
   - Tanlangan darajaga mos mavzular avtomatik filtrlanadi va saqlanib qoladi.

2. **Teleprompter (Matnni 4 so'zlik qatorda o'qish):**
   - Matn har bir qatorda aniq 4 ta so'zdan iborat qilib formatlangan.
   - O'qish tezligi 60 dan 250 WPM gacha silliq boshqariladi (Slider va 80, 140, 190, 250 tezlik tugmalari).
   - O'qilayotgan faol qator yuqori kontrastda yorishadi, boshqa qatorlar esa xiralashtiriladi.

3. **Ovoz Yozish (Diktofon & LocalStorage):**
   - Foydalanuvchi matnni o'qiyotganida ovozi brauzerning `MediaRecorder` orqali yozib olinadi.
   - Yozib olingan ovozlar qurilmaning `localStorage` xotirasida saqlanadi.
   - Maksimal 3 ta audio saqlanadi, yangi yozuv qo'shilganda eng eskisi avtomatik o'chiriladi (FIFO navbati).
   - Saqlangan yozuvlarni pleyer orqali istalgan payt eshitish yoki o'chirish mumkin.

4. **Lug'at (Vocabulary) & 2-Siklli Ovozli Diktant:**
   - Har bir mavzuda matndan olingan 10 tadan qiyin so'z va ularning aniq o'zbekcha tarjimasi (Jami 100 ta so'z).
   - Diktor har bir so'zni **2 martadan** aytib beradi:
     - **1-sikl:** `[Inglizcha so'z]` $\rightarrow$ 400ms $\rightarrow$ `[O'zbekcha tarjimasi]`
     - *(800ms oraliq pauza)*
     - **2-sikl:** `[Inglizcha so'z]` $\rightarrow$ 400ms $\rightarrow$ `[O'zbekcha tarjimasi]`
     - *(1.2s oraliqdan so'ng keyingi so'zga o'tish)*
   - "Barchasini tinglash" (Autoplay) yoki istalgan so'zni bittalab bosib eshitish imkoniyati.

5. **Ikki Tilli Interfeys (EN / UZ):**
   - Inglizcha va O'zbekcha tillarga birgina tugma orqali lahzada almashish.

---

## 🚀 Ishga Tushirish

### 1-usul: Node.js server orqali
```bash
npm start
# yoki
node server.js
```
Brauzerda oching: `http://localhost:3000`

### 2-usul: To'g'ridan-to'g'ri brauzerda (Static)
Hech qanday qo'shimcha o'rnatishlarsiz `index.html` yoki `speakline_english_speaking_practice.html` faylini istalgan brauzerda ochish kifoya.

---

## 📁 Loyiha Strukturasi

```
Malika-English/
├── index.html                               # Asosiy ilova fayli (GitHub Pages uchun)
├── speakline_english_speaking_practice.html # To'liq ilova kodi (HTML/CSS/JS modullar)
├── server.js                                # Node.js local HTTP server
├── package.json                             # Loyiha konfiguratsiyasi
└── README.md                                # Loyiha qo'llanmasi
```

---

## 🛠 Texnologiyalar

- **HTML5 & CSS3** (CSS Custom Properties, Flexbox, Grid, Glassmorphism)
- **JavaScript (ES6+)** (Web Speech API / SpeechSynthesis, MediaStream Recording API, Web Audio API, LocalStorage)
- **Node.js** (Oddiy zero-dependency HTTP server)
- **Google Fonts** (Plus Jakarta Sans, Inter, Source Serif 4)
