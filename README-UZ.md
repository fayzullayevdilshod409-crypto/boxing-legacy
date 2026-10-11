# BOXING LEGACY — PWA paket

Bu papkada o‘yinning PWA (Progressive Web App) versiyasi bor. U birinchi marta internet bilan muvaffaqiyatli ochilgach, Service Worker orqali asosiy o‘yin faylini keshlaydi va keyingi ochilishlarda internet bo‘lmasa ham ishlashi uchun sozlangan.

## Telefon orqali GitHub Pages’ga joylash
1. GitHub’da yangi repository yarating.
2. Shu papkadagi fayllarni repository’ning asosiy (root) qismiga yuklang: `index.html`, `manifest.json`, `sw.js`, `icons/`. `README.md` ixtiyoriy.
3. Repository → Settings → Pages → Deploy from a branch → `main` va `/(root)` ni tanlang → Save.
4. HTTPS sayt manzili tayyor bo‘lishini kuting va Chrome’da oching.
5. O‘yinni bir marta to‘liq yuklang, so‘ng Chrome menyusidan “Install app” yoki “Add to Home screen”ni tanlang.
6. Internetni o‘chirib, o‘yinni tekshiring. Offline keshlash faqat birinchi muvaffaqiyatli tashrifdan keyin ishlaydi.

## Google Play uchun muhim
Bu PWA fayllarining o‘zi AAB emas. Google Play’ga chiqarish uchun PWA’ni Android paketiga (masalan, Trusted Web Activity/Bubblewrap yoki mos build xizmati bilan) o‘rash, release signing va Play Console talablarini bajarish kerak. Service Worker va manifest HTTPS domenida ishlashi kerak. O‘yinning offline ishlashini va saqlangan karyerani telefonda sinab ko‘ring.

## Fayllar
- `index.html` — BOXING LEGACY o‘yini, PWA ulanishlari qo‘shilgan.
- `manifest.json` — ilova nomi, ranglar va ikonka sozlamalari.
- `sw.js` — offline cache.
- `icons/` — 192×192 va 512×512 PNG ikonkalari.
