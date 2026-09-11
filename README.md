# Dars jadvali

Haftalik dars jadvalini ko'rsatuvchi, qo'l bilan chapga/o'ngga surib kunlar orasida o'tiladigan, zamonaviy va och-qora/kulrang (monoxrom) dizaynli veb-ilova. Hech qanday tashqi kutubxona yoki server talab qilmaydi — bitta `index.html` fayl.

## Xususiyatlari

- Ilova ochilganda avtomatik ravishda **bugungi kun** va o'sha kunlik dars jadvali ko'rsatiladi
- Kunlar orasida **qo'l bilan surib** (swipe) o'tish, yoki yuqoridagi sirg'anuvchi (segmented) kun tanlagichdan bosib tanlash
- Hozirgi vaqtga to'g'ri kelgan dars **"Hozir"** belgisi bilan ajratiladi (soat ko'rsatilmaydi, faqat ichki hisoblash uchun ishlatiladi)
- To'liq monoxrom — och-qora fon va kulrang tonlar, ortiqcha ranglarsiz
- Bitta HTML fayl — internetsiz ham ishlaydi (shrift yuklanishidan tashqari)

## Mahalliy ishga tushirish

`index.html` faylini istalgan brauzerda oching, yoki telefonda Acode kabi muharrirlardan **Open with Browser** funksiyasi orqali ochsangiz bo'ladi.

## GitHub'ga joylash

1. GitHub'da yangi repozitoriya yarating (masalan `dars-jadvali`), README qo'shmasdan.
2. Shu papkadagi fayllarni kompyuteringizga yoki telefoningizga tushiring.
3. Terminalda (yoki Termux/Acode terminalida) quyidagilarni bajaring:

   ```bash
   cd dars-jadvali
   git init
   git add .
   git commit -m "Dars jadvali - zamonaviy versiya"
   git branch -M main
   git remote add origin https://github.com/FOYDALANUVCHI_NOMI/dars-jadvali.git
   git push -u origin main
   ```

   `FOYDALANUVCHI_NOMI` o'rniga o'z GitHub login nomingizni yozing.

## GitHub Pages orqali onlayn qilish (bepul havola olish)

1. Repozitoriyada **Settings → Pages** bo'limiga o'ting.
2. **Branch** qismida `main` va papka sifatida `/ (root)` ni tanlang, so'ng **Save** bosing.
3. Bir necha daqiqadan so'ng ilova quyidagi manzilda ochiladi:

   ```
   https://FOYDALANUVCHI_NOMI.github.io/dars-jadvali/
   ```

Shu havolani telefon ekraniga qo'shib qo'ysangiz, oddiy ilova kabi ochilaveradi.

## iPhone'da ilova sifatida ishlatish

Bu oddiy veb-sahifa, lekin uni iPhone'da xuddi haqiqiy ilova kabi bosh ekranga qo'yib olishingiz mumkin — App Store kerak emas:

1. Avval loyihani GitHub Pages orqali onlayn qiling (yuqoridagi bo'limga qarang) — sizga bir havola kerak bo'ladi, masalan `https://foydalanuvchi.github.io/dars-jadvali/`.
2. iPhone'da **Safari** brauzerini oching (Chrome emas — bu funksiya faqat Safari'da ishlaydi) va o'sha havolani oching.
3. Pastdagi **Ulashish** tugmasini bosing (kvadrat ichidan strelka chiqib turgan belgi).
4. Ro'yxatdan **"Add to Home Screen" / "Bosh ekranga qo'shish"** ni tanlang.
5. Nom kiritishni so'raydi — xohlasangiz "Dars jadvali" deb qoldiring va **Qo'shish**ni bosing.

Shundan so'ng bosh ekraningizda o'z ikonkasi bilan alohida ilova paydo bo'ladi — uni bosganda Safari manzil satrisiz, to'liq ekranli, haqiqiy ilova kabi ochiladi. Loyihada shu holat uchun kerakli sozlamalar (`manifest.json`, `icons/` papkasi) allaqachon tayyorlangan — shunchaki GitHub'ga fayllarni **o'zaro papka tuzilishini saqlagan holda** yuklashingiz kifoya.

## Jadvalni yangilash

Barcha darslar `index.html` faylining ichidagi `WEEK` massivida saqlanadi. Yangi hafta yoki o'zgargan dars bo'lsa, shu massivdagi tegishli kunning `lessons` ro'yxatini tahrirlang — har bir dars `subj` (fan nomi) va `teacher` (o'qituvchi) maydonlaridan iborat, `t1`/`t2` esa faqat "Hozir" belgisini hisoblash uchun ichki foydalaniladi va ekranda ko'rinmaydi.
