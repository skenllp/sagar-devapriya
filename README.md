# Sagar T V & Devapriya V — Wedding Invitation

Mobile-first cinematic invitation. Plain HTML5, CSS3, and vanilla JavaScript.
Grand Reception (15 December 2026, Oasis Grand) is the primary feature.

```
sagar-devapriya/
├── assets/
│   ├── images/
│   │   ├── cover/          cover.webp, cover.jpg (landing background)
│   │   ├── hero/           hero.jpg, hero.webp
│   │   ├── couple/         couple-1.jpg/webp, couple-2.jpg/webp (the two supplied photographs)
│   │   ├── reception/      qr-oasis-grand.png (functional Google Maps QR)
│   │   ├── share/          sagar-devapriya-og.jpg (1200×630 social preview)
│   │   ├── decorations/    section wash SVGs
│   │   └── icons/
│   ├── video/              invitation-reveal.mp4
│   └── audio/
├── css/
├── js/
├── index.html
└── README.md
```

## Run

Serve the project root over HTTP (needed for video):

```powershell
python -m http.server 8080
```

Open <http://localhost:8080>.

## Production assets

| Role | Path |
|------|------|
| Landing cover | `assets/images/cover/cover.webp` (fallback `cover.jpg`) |
| Intro video | `assets/video/invitation-reveal.mp4` |
| Hero background | `assets/images/hero/hero.webp` (fallback `hero.jpg`) |
| Section washes | `assets/images/decorations/wash-*.svg` |
| Couple photographs | `assets/images/couple/couple-1.*`, `couple-2.*` |
| Reception QR | `assets/images/reception/qr-oasis-grand.png` — points to the Oasis Grand Google Maps listing |
| Social share image | `assets/images/share/sagar-devapriya-og.jpg` |

## Content notes

- English only — no Malayalam text or fonts are loaded anywhere in this build.
- Wedding ceremony: 12 December 2026, 11:50 AM – 12:20 PM, Valayanattu Auditorium, Ranni.
- Grand Reception: 15 December 2026, 6:00 PM onwards, Oasis Grand, Trichambaram, Taliparamba.
- Update `og:url` / `og:image` (and the matching Twitter tags) in `index.html` to the real deployed domain before going live — social previews will not render correctly until those absolute URLs match production.
