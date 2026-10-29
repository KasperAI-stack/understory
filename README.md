# Kasper til Understory

En personlig landingpage til ansøgningen som Marketing Operations Lead hos Understory i Aarhus. Siden er bygget på koden fra Cozze-siden (repoet cozze, som bygger på Maki og hey-kasper.dk) med ny tekst, Understorys farver og Understorys logo.

## Mappen

- site/: selve hjemmesiden. Det er kun denne mappe, der kommer online.
  - index.html: forsiden med al teksten
  - cv.html og ansoegning.html: CV'et og ansøgningen bygget op som PDF'erne i assets/pdf/. PDF'erne er på engelsk, så de engelske sider er ordret fra dem, og de danske er en oversættelse. Ret teksten begge steder.
  - css/dokument.css: designet til CV og ansøgning (Inter, farverne fra PDF'erne)
  - en/: de engelske udgaver (index.html, cv.html og application.html). Sprogvælgeren DA/EN i toppen skifter mellem dem.
  - 404.html: siden, der vises, hvis adressen er forkert
  - css/styles.css: farver og design. Understorys farver (mørkegrøn #022C12 og lysegul #F1F97E) står øverst under `:root`.
  - js/main.js: små forbedringer, fx agentvælgeren i toppen og temaknappen
  - assets/understory-logo.svg: Understorys logo i mørkegrøn (#022C12)
  - assets/og-image.jpg og og-image-en.jpg: billedet, der vises, når linket deles på LinkedIn eller i en mail
- netlify.toml: fortæller Netlify, at site/ skal publiceres.

## Linket

Siden ligger på GitHub Pages: https://kasperai-stack.github.io/understory/ (engelsk: https://kasperai-stack.github.io/understory/en/)

Den bliver opdateret automatisk, hver gang der pushes (se .github/workflows/pages.yml). Første gang skal GitHub Pages slås til én gang: Settings → Pages → Source: "GitHub Actions".

## Se siden på din egen computer

1. Åbn en terminal i mappen.
2. Skriv `npx serve site` og åbn adressen, der vises i terminalen.

## Godt at vide

- Siden skal ikke kunne findes på Google. Den har `noindex` i HTML'en, i netlify.toml og i robots.txt.
- Der er ingen Google Tag Manager, cookies eller formular på siden. Kontakt sker via "Kald til samtale" (mail til kasmussen80@gmail.com) og telefon.
- Teksten følger Kaspers stemme: "I" og "jer" til Understory, ingen tankestreger og ingen opdigtede tal. Fakta kommer fra jobopslaget, understory.io og Kaspers CV og ansøgning.
