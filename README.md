# Train2Win — Prezentacja sponsorska (Brillux)

Statyczna prezentacja HTML/CSS/JS (React + Babel z CDN, custom web components `<deck-stage>` i `<image-slot>`). Slajdy 1920x1080 z auto-skalowaniem do dowolnego viewportu.

## Struktura

```
brilux/
├── public/                 # root deployu na Vercelu
│   ├── index.html
│   ├── deck-stage.js
│   ├── image-slot.js
│   ├── tweaks-panel.jsx
│   └── uploads/
│       ├── mural_image-...png
│       └── wall_image-...png
├── vercel.json
├── .gitignore
└── README.md
```

## Lokalny podgląd

```powershell
cd public
python -m http.server 8080
# albo: npx serve .
```

Nawigacja: lewo/prawo, PageUp/PageDown, Spacja, Home/End, R = reset.

## Deploy na Vercelu

1. Repo jest podłączone do https://github.com/armitiel/brilux.git
2. Na vercel.com/new zaimportuj repo `armitiel/brilux`
3. Ustawienia: **Framework Preset = Other**, **Root Directory = `public`**, build/install commands puste
4. Deploy

## Aktualizacja

```powershell
cd C:\Users\DELL\Documents\brilux
git add .
git commit -m "..."
git push
```
