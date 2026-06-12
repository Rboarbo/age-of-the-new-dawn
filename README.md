# ⚜ Age of the New Dawn

Een volledig speelbare Age of Empires-stijl real-time strategy game in de browser,
gebouwd in 3D met Three.js. Eén HTML-bestand, volledig offline speelbaar
(Three.js is inline embedded — geen CDN of internet nodig).

## 🎮 Spelen

Open `index.html` in een moderne browser, of speel de gehoste versie via GitHub Pages.

**Features:** resource gathering (hout/voedsel/goud) · boerderijen · huizen · kazerne
met soldaten, boogschutters en upgrades (wapens/pantser) · muren met lijnplaatsing ·
poorten die openen voor eigen units · wachttorens · fog of war · vijandelijk krijgskamp
als winconditie · golvenverdediging · control groups · pauzemenu · procedurele
painterly textures & WebAudio-geluid.

## 🚀 Eenmalige setup (daarna deployt elke wijziging automatisch)

1. Maak op GitHub een nieuwe repository, bijv. `age-of-the-new-dawn`
2. In deze map:
   ```bash
   git init
   git add .
   git commit -m "v5: Age of the New Dawn"
   git branch -M main
   git remote add origin https://github.com/Rboarbo/age-of-the-new-dawn.git
   git push -u origin main
   ```
3. Op GitHub: **Settings → Pages → Source: "GitHub Actions"**

Klaar. Vanaf nu geldt: **elke `git push` naar `main` deployt automatisch**
naar `https://rboarbo.github.io/age-of-the-new-dawn/` via de meegeleverde
workflow (`.github/workflows/deploy.yml`). Nieuwe spelversie = bestand
vervangen, committen, pushen — binnen ~1 minuut staat hij live.

## 🔄 Workflow voor nieuwe versies

```bash
# vervang index.html door de nieuwe versie, dan:
git add index.html
git commit -m "v6: <wat er nieuw is>"
git push
```

De Actions-tab toont de deploy-status.
