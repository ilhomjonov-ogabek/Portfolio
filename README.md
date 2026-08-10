# Og'abek Ilhomjonov — Portfolio

Java Backend Developer uchun shaxsiy portfolio sayti. Toza HTML/CSS/JS — build qadamisiz to'g'ridan-to'g'ri statik hosting (Netlify) orqali deploy qilinadi.

**Live:** https://ogabek-ilhomjonov.netlify.app

## Tarkib

- Bosh sahifa (hero)
- Ko'nikmalar (animatsion progress-bar'li skill kartalar)
- Ish tajribasi
- Ta'lim (timeline)
- Loyihalar
- Kontakt (kartochkalar + Netlify Forms orqali xabar yuborish formasi)

## Xususiyatlar

- Toza HTML/CSS/JS — hech qanday framework yoki build tool talab qilinmaydi
- Dark theme, animatsiyali Java-kod fon (canvas)
- Scroll-snap sahifalar + yon tomondagi dot-navigatsiya, scroll progress-bar
- Scroll-reveal animatsiyalar va animatsion skill barlar
- Mobil hamburger-menyu
- **UZ / RU / EN** til almashtirish (nav'dagi til tugmasi, tanlov `localStorage`da saqlanadi)
- **⌘K / Ctrl+K command palette** — bo'limlarga tez o'tish, email nusxalash, GitHub/Telegram ochish
- Jonli GitHub statistikasi (public repo va follower soni, GitHub API orqali)
- Netlify Forms orqali kontakt-forma (spam-himoya bilan)
- SEO: meta description, Open Graph/Twitter card, JSON-LD (Person schema), `robots.txt`, `sitemap.xml`
- PWA: `site.webmanifest` + ikonka — telefon ekraniga o'rnatish mumkin
- Maxsus 404 sahifa
- `@media print` — chop etishga mos ko'rinish
- `prefers-reduced-motion` ni hurmat qiladi
- Kichik easter egg (Konami code 🙂)

## Lokal ishga tushirish

Har qanday statik server yetarli, masalan:

```bash
npx serve .
```

yoki oddiygina `index.html` faylini brauzerda oching.

## HTML validatsiyasi

```bash
npx html-validate index.html 404.html
```

Bu tekshiruv har bir push'da GitHub Actions (`.github/workflows/ci.yml`) orqali avtomatik ishga tushadi.

## Deploy

Netlify'da publish directory sifatida repo ildizini (`/`) ko'rsating — build command shart emas. `netlify.toml` xavfsizlik headerlarini avtomatik qo'shadi.
