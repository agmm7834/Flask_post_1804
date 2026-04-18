
### 1. Masala: Kontakt formasi
**Shartlar:**  
- Formada 3 ta maydon bo‘lishi kerak.  
- Validatsiya:  
  - `ism` uzunligi > 2 bo‘lishi shart  
  - `email` da `@` belgisi bo‘lishi shart  
  - `xabar` uzunligi >= 15 bo‘lishi shart  
- Agar barcha shartlar bajarilsa → `res = [ism, email, xabar]`  
- Aks holda → `res = ["Ma'lumotlar noto'g'ri kiritildi"]`  

**index.html (to‘liq form):**
```html
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kontakt</title>
</head>
<body>
    <h2>Kontakt ma'lumotlarini kiriting</h2>
    <form method="POST">
        <input type="text" name="ism" placeholder="Ismingiz" required><br><br>
        <input type="email" name="email" placeholder="Email manzilingiz" required><br><br>
        <textarea name="xabar" placeholder="Xabaringiz" rows="5" required></textarea><br><br>
        <button type="submit">Yuborish</button>
    </form>
</body>
</html>
```

### 2. Masala: Ro‘yxatdan o‘tish (telefon bilan)
**Shartlar:**  
- Formada 3 ta maydon bo‘lishi kerak.  
- Validatsiya:  
  - `foydalanuvchi_nomi` uzunligi > 4 bo‘lishi shart  
  - `telefon` da “+” belgisi bo‘lishi va uzunligi >= 11 bo‘lishi shart  
  - `yosh` raqam bo‘lishi va 18 ≤ yosh ≤ 99 bo‘lishi shart  
- Agar barcha shartlar bajarilsa → `res = [foydalanuvchi_nomi, telefon, yosh]`  
- Aks holda → `res = ["Ma'lumotlar noto'g'ri kiritildi"]`  

**index.html (to‘liq form):**
```html
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ro'yxatdan o'tish</title>
</head>
<body>
    <h2>Ro'yxatdan o'tish</h2>
    <form method="POST">
        <input type="text" name="foydalanuvchi_nomi" placeholder="Foydalanuvchi nomi" required><br><br>
        <input type="text" name="telefon" placeholder="+998 XX XXX XX XX" required><br><br>
        <input type="text" name="yosh" placeholder="Yoshingiz" required><br><br>
        <button type="submit">Ro'yxatdan o'tish</button>
    </form>
</body>
</html>
```

### 3. Masala: Kitob ma'lumotlarini qo'shish
**Shartlar:**  
- Formada 3 ta maydon bo‘lishi kerak.  
- Validatsiya:  
  - `kitob_nomi` uzunligi > 3 bo‘lishi shart  
  - `muallif` uzunligi > 3 bo‘lishi shart  
  - `sahifalar` raqam bo‘lishi va ≥ 50 bo‘lishi shart  
- Agar barcha shartlar bajarilsa → `res = [kitob_nomi, muallif, sahifalar]`  
- Aks holda → `res = ["Ma'lumotlar noto'g'ri kiritildi"]`  

**index.html (to‘liq form):**
```html
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kitob qo'shish</title>
</head>
<body>
    <h2>Yangi kitob ma'lumotlarini kiriting</h2>
    <form method="POST">
        <input type="text" name="kitob_nomi" placeholder="Kitob nomi" required><br><br>
        <input type="text" name="muallif" placeholder="Muallif" required><br><br>
        <input type="text" name="sahifalar" placeholder="Sahifalar soni" required><br><br>
        <button type="submit">Qo'shish</button>
    </form>
</body>
</html>
```

### 4. Masala: Fikr-mulohaza (baholash) formasi
**Shartlar:**  
- Formada 3 ta maydon bo‘lishi kerak.  
- Validatsiya:  
  - `ism` uzunligi > 2 bo‘lishi shart  
  - `baho` faqat “1”, “2”, “3”, “4” yoki “5” bo‘lishi shart  
  - `sharh` uzunligi >= 10 bo‘lishi shart  
- Agar barcha shartlar bajarilsa → `res = [ism, baho, sharh]`  
- Aks holda → `res = ["Ma'lumotlar noto'g'ri kiritildi"]`  

**index.html (to‘liq form):**
```html
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fikr-mulohaza</title>
</head>
<body>
    <h2>Fikr-mulohazangizni qoldiring</h2>
    <form method="POST">
        <input type="text" name="ism" placeholder="Ismingiz" required><br><br>
        <input type="text" name="baho" placeholder="Baho (1-5)" required><br><br>
        <textarea name="sharh" placeholder="Sharhingiz" rows="4" required></textarea><br><br>
        <button type="submit">Yuborish</button>
    </form>
</body>
</html>
```
