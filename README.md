# HTTP Metodlari: POST, GET, PUT, DELETE

HTTP metodlari vebda ma'lumotlarni almashish va API-lar bilan muloqot qilishning asosiy usuli hisoblanadi. Eng ko'p ishlatiladigan HTTP metodlari quyidagilardir:

- **POST** — Yangi resurs yaratish.
- **GET** — Ma'lumotni olish.
- **PUT** — Mavjud resursni yangilash yoki o'zgartirish.
- **DELETE** — Resursni o'chirish.

Bu metodlar odatda CRUD operatsiyalari bilan bog'liq bo'lib, ular RESTful API-larda keng qo'llaniladi.

## 1. POST Metodi

**POST** — bu serverga yangi resursni yaratish uchun so'rov yuboruvchi HTTP metodidir. POST so'rovi bilan birgalikda odatda ma'lumotlar (yangi yozuv) yuboriladi, va server bu ma'lumotlar asosida yangi resurs yaratadi.

### POST ning asosiy xususiyatlari:
- Serverda yangi ma'lumotlar yozuvini yaratish uchun ishlatiladi.
- Xavfsiz emas, chunki u server holatini o'zgartiradi.
- Idempotent emas — bir xil POST so'rovini bir necha marta yuborish bir nechta resurs yaratishga olib keladi.

### 2. GET Metodi

#### GET — serverdan ma'lumot olish uchun ishlatiladigan HTTP metodidir. GET so'rovi bilan hech qanday ma'lumot yuborilmaydi, balki serverdan mavjud ma'lumotlarni olish so'raladi.
##### GET ning asosiy xususiyatlari:
-Ma'lumotlarni olish uchun ishlatiladi.
-Xavfsiz, chunki u serverdagi ma'lumotlarni o'zgartirmaydi.
-Idempotent — bir xil GET so'rovini bir necha marta yuborish bir xil natija beradi.

### 3. PUT Metodi

#### PUT — mavjud resursni yangilash yoki uni o'zgartirish uchun ishlatiladigan HTTP metodidir. Agar resurs mavjud bo'lmasa, PUT uni yaratishi mumkin.
##### PUT ning asosiy xususiyatlari:
-Mavjud resursni yangilash yoki yangisini yaratish uchun ishlatiladi.
-Idempotent — bir xil PUT so'rovini bir necha marta yuborish bir xil natija beradi.
-Ma'lumotlar serverga to'liq ko'rinishda yuboriladi.

### 4. DELETE Metodi

#### DELETE — serverdagi resursni o'chirish uchun ishlatiladigan HTTP metodidir. DELETE so'rovi resursni butunlay yo'q qiladi.
#### DELETE ning asosiy xususiyatlari:
-Resursni o'chirish uchun ishlatiladi.
-Idempotent — bir xil DELETE so'rovini bir necha marta yuborish bir xil natija beradi (resurs yo'q bo'lsa, boshqa hech narsa bo'lmaydi).

### HTTP Metodlarining Qo'llanilishi
#### HTTP metodlari RESTful API-lar va veb ilovalar bilan ishlashda muhim rol o'ynaydi. Har bir metodning o'ziga xos maqsadi va qo'llanilish sohasi mavjud, bu esa tizimlar o'rtasida samarali va xavfsiz muloqotni ta'minlashga yordam beradi.

POST — Yangi ma'lumot yaratish.
GET — Ma'lumotni o'qish.
PUT — Ma'lumotni yangilash.
DELETE — Ma'lumotni o'chirish.
Bu metodlar tizimning barcha asosiy CRUD operatsiyalarini qamrab oladi va API-larning asosini tashkil qiladi.
