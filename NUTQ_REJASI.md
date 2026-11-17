# C# Class Library (Sinflar Kutubxonasi) — Taqdimotchi Nutq Rejasi

Ertaga doskaga chiqqaningizda ushbu qo'llanmadan foydalanishingiz mumkin. Har bir slayd uchun nima deyish kerakligi va ekranda qanday harakat qilish lozimligi qadamba-qadam yozilgan.

---

## 🚀 Taqdimotni Qanday Ishga Tushirasiz?
1. Desktopdagi `CSharp_Class_Library_Taqdimot` papkasiga kiring.
2. `index.html` faylini istalgan brauzerda (Google Chrome, Microsoft Edge) ikki marta bosib oching.
3. Klaviaturadan **F11** yoki yuqori o'ng burchakdagi **"⛶ Ekranga yoyish"** tugmasini bosing (to'liq ekranga o'tadi).
4. Slaydlarni o'tkazish uchun: **O'ng strelka (→)** yoki **Probel (Space)** tugmasidan foydalaning.

---

## 🎙️ Slaydma-Slayd Gapiriladigan So'zlar:

### 1-Slayd: Kirish (Sarlavha)
> **Siz aytasiz:**
> *"Assalomu alaykum, hurmatli ustoz va qadrli talabalar. Bugun men sizlarga C# dasturlash tilida eng muhim va professional dasturchilar har kuni ishlatadigan mavzulardan biri — **'Sinflar kutubxonasini (Class Library) yaratish va loyihalar bilan ishlash'** mavzusini tushuntirib beraman. Oddiy slaydlardan ko'ra qiziqarliroq bo'lishi uchun men bu mavzuni interaktiv veb-platforma orqali va jonli kodlar bilan ko'rsatib bermoqchiman."*

---

### 2-Slayd: Class Library nima?
> **Siz aytasiz:**
> *"Keling, avvalo 'Class Library o'zi nima?' degan savolga javob beraylik. 
> Biz odatda C# da konsol ilovasi yoki Windows Forms yaratganimizda, u `Main()` metodiga ega bo'ladi va uni F5 bosib to'g'ridan-to'g'ri ishga tushiramiz. Natijada **.exe** fayl hosil bo'ladi.
> 
> **Class Library (Sinflar Kutubxonasi)** esa — mustaqil ishlamaydigan, o'zida `Main()` metodi bo'lmagan sinflar to'plamidir. Uni kompilyatsiya qilganimizda **.dll (Dynamic Link Library)** fayl hosil bo'ladi. Uning asosiy vazifasi — boshqa dasturlar uchun tayyor xizmat va funksiyalarni taqdim etishdir."*

---

### 3-Slayd: Nega Class Library yaratamiz? (Afzalliklari va Hayotiy misol)
> **Siz aytasiz:**
> *"Nega biz hamma kodni bitta dastur ichiga yozavermaymiz? Bunga 3 ta asosiy sabab bor:
> 1. **DRY (Don't Repeat Yourself):** Bir xil matematik formula yoki ma'lumotlar bilan ishlash kodini qayta-qayta yozmasdan, bitta DLL qilib qo'yib, yuzlab dasturlarda foydalanish mumkin.
> 2. **Modullilik:** Katta jamoada ishlaganda har kim o'z kutubxonasini alohida yozadi.
> 3. **Xavfsizlik:** Kodingizni boshqalarga bermoqchi bo'lsangiz, manba kodni (source code) emas, tayyor `.dll` ni berasiz.
> 
> **Hayotiy misol:** Avtomobil zavodi (bu bizning asosiy dastur). Dvigatel ishlab chiqaruvchi zavod esa — Class Library. Dvigatel ko'chada mashinasiz o'zi yura olmaydi. Lekin xuddi shu dvigatelni turli rusumdagi avtomobillarga o'rnatib ishlatsa bo'ladi."*

---

### 4-Slayd: Loyihalar Arxitekturasi (.sln, .csproj, .dll)
> **Siz aytasiz:**
> *"Endi .NET da bu qanday tuzilganini ko'ramiz. Bitta yechim — **Solution (.sln)** ochiladi. Uning ichida ikkita loyiha bo'ladi:
> Biri — **Class Library**, ikkinchisi — uni ishlatuvchi **Console App**.
> Konsol ilovamiz kutubxonani tushunishi uchun biz **Project Reference (Loyiha havolasi)** ulaymiz. Shundan so'ng, xuddi tizimning `System` kutubxonasini ishlatgandek, tepada `using MeningKutubxonam;` deb bemalol chaqira olamiz."*

---

### 5-Slayd: Qadamba-qadam yaratish (CLI / Terminal)
*(Bu slaydda yuqoridagi 1, 2, 3, 4 tugmalarni bosib, ketma-ket ko'rsatasiz!)*

> **1-Qadam tugmasini bosing:** 
> *"Birinchi qadamda `dotnet new classlib -o MatematikaLib` buyrug'i orqali toza kutubxona ochamiz."*
> 
> **2-Qadam tugmasini bosing:**
> *"Ikkinchi qadamda sinf yozamiz. Bu yerda eng muhim qoida: Sinf va metodlar oldiga **public** kalit so'zi qo'yilishi shart! Agar qo'ymasdan qoldirsak, u sukut bo'yicha `internal` bo'lib qoladi va boshqa dasturlarga ko'rinmaydi."*
> 
> **3-Qadam va 4-Qadam tugmalarini bosing:**
> *"So'ngra konsol ilova yaratib, `dotnet add reference` buyrug'i orqali kutubxonamizni unga ulaymiz va `new` qilib obyekt olamiz."*

---

### 6-Slayd: Kirish Cheklovchilari (Access Modifiers)
> **Siz aytasiz:**
> *"Class Library loyihalarida eng ko'p e'tibor qaratiladigan narsa — bu **kirish huquqlari (Access Modifiers)**.
> - **public:** Bu kutubxonaning ochiq yuzi. Tashqi loyihalar foydalanishi uchun.
> - **internal:** Faqat shu DLL ichidagi sinflar bir-biri bilan gaplashishi uchun. Tashqaridan qaragan odam buni umuman ko'ra olmaydi. Bu tizimning xavfsizligi va arxitektura tozaligini ta'minlaydi."*

---

### 7-Slayd: JONLI INTERAKTIV PLAYGROUND (Eng asosiy qism! 🔥)
*(Bu yerda doskada amaliy tomosha ko'rsatasiz!)*

> **Siz aytasiz:**
> *"Hurmatli ustoz, endi esa buni amalda ko'ramiz. Ushbu interaktiv muhitda chap tomonda kutubxonamiz kodi, o'ng tomonda esa uni ishlatuvchi konsol dasturimiz joylashgan."*
> 
> 1. Yuqoridagi **"▶ Ishga tushirish (Run)"** tugmasini bosing.
>    - Terminalda `dotnet build`, `.dll` fayl hosil bo'lishi va natijalar chiqqanini ko'rsating.
> 2. `Program.cs` tabiga o'ting va sonlarni o'zgartiring:
>    - Masalan, `son1 = 25` ni `100` qiling.
> 3. Yana **"▶ Ishga tushirish (Run)"** tugmasini bosing.
>    - Terminalda natijalar yangilangani darhol ko'rinadi!
> 4. Dropdown menyudan **"2-Misol: Talaba Baholash Kutubxonasi"** ni tanlab, yana bitta OOP misolini ko'rsating.

---

### 8-Slayd: Muhim Savol-Javoblar va Nozik Nuqtalar (FAQ)
*(Har bir kartani bosib, auditoriyaga savol-javob tariqasida tushuntirasiz)*

> **Siz aytasiz:**
> *"Mavzuni to'liq mustahkamlash uchun, amaliyotda dasturchilar eng ko'p adashadigan yoki e'tibor qaratishi lozim bo'lgan bir nechta muhim nozik texnik jihatlarni ko'rib chiqamiz:*
> 
> 1. **1-savolni ochasiz:**
>    *'Birinchi muhim masala: Class Library loyihasini to'g'ridan-to'g'ri F5 bosib ishga tushirsa bo'ladimi?'*
>    *— 'Yo'q, chunki unda dasturga kirish nuqtasi bo'lgan `Main()` metodi mavjud emas. U faqat boshqa dasturlarga (Console, Web yoki Mobil) xizmat ko'rsatish uchun mo'ljallangan.'*
> 
> 2. **2-savolni ochasiz:**
>    *'Ikkinchi masala: DLL nima va u qayerga tushadi?'*
>    *— 'DLL — bu Dynamic Link Library, ya'ni dinamik kutubxona bo'lib, loyihani build qilganimizda `bin/Debug` papkasida hosil bo'ladi.'*
> 
> 3. **3-savolni ochasiz:**
>    *'Uchinchi masala: Biz yaratgan kutubxonani butun dunyo dasturchilari ishlatishi uchun nima qilish kerak?'*
>    *— 'Uni NuGet paketi (`.nupkg`) holatida paketlab, ochiq omborga joylashtirish mumkin. Masalan, barchamiz biladigan Newtonsoft.Json ham xuddi shunday Class Library asosida yaratilgan.'*
> 
> 4. **4-savolni ochasiz:**
>    *'To'rtinchi masala: Project Reference bilan Package Reference ning farqi nima?'*
>    *— 'Project Reference bu bitta Solution ichidagi o'zimiz yozayotgan qo'shni loyihaga ulanish. Package Reference esa internetdan tayyor yig'ilgan paketni yuklab olib ulanishdir.'*

---

### 9-Slayd: Xulosa
> **Siz aytasiz:**
> *"Xulosa qilib aytganda, Class Library — bu C# va .NET ekotizimida kodni toza saqlash, xavfsizlik va bir yozilgan kodni qayta-qayta ishlatish (reusability) ning eng asosiy poydevoridir. E'tiboringiz uchun rahmat, agar savollar bo'lsa javob berishga tayyorman!"*

---

## 🎯 Maslahat:
Ertaga darsga borishdan oldin faylni ochib, slaydlarni 1-2 marta o'zingiz bosib, nutqni mashq qilib ko'ring. Barcha kerakli narsalar to'liq avtonom ishlaydi (internet bo'lishi ham shart emas!).
Omad! Siz albatta eng yuqori ballni olasiz!
