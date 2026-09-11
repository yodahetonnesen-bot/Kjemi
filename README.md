# Kjemi 1 — interaktive kapittelsider

Samme oppsett som fysikksidene: én selvstendig HTML-fil per kapittel, med HTML, CSS og
JavaScript i samme fil. Ingen byggesteg, ingen avhengigheter. Åpne fila i en nettleser,
eller publiser mappa.

| Fil | Kapittel |
| --- | --- |
| `index.html` | Kapittel 1 (stillas — venter på fagstoff) |

## Hva som allerede virker

- Designsystemet fra fysikksidene: lyst og mørkt tema, typografi, kort, bokser, formelblokker,
  tabeller, tidslinje, figurer og oppgaver med skjult løsning.
- Sidemeny med faner for oversikt, fem delkapitler, øving og referanse. Hver fane har sin egen
  adresse (`#del-a`), og tilbakeknappen virker.
- Søk fra topplinja, med `/` eller Ctrl/Cmd+K. Indeksen bygges fra sida selv.
- Sjekkliste med framdrift, flashcards med statistikk, og quiz med forklaring på hvert svar.
  Alt lagres lokalt i `localStorage`.
- Skiplenke, synlig fokusmarkering, tastaturstyrt flashcard, trykkmål på 44 px og ingen
  vannrett rulling ned til 360 px.

## Hva som mangler

Fagstoffet. Alle tekstfeltene er plassholdere. Animasjonsmotoren fra fysikksida (canvas-scener,
grafmotor og «Endre oppsettet») er ikke med ennå — den hentes inn når vi vet hvilke kjemiscener
kapitlet trenger (titrering, partikkelmodell, likevekt og så videre).

## Slik fyller du inn innhold

| Det du vil endre | Hvor i `index.html` |
| --- | --- |
| Kapitteltittel og delkapittelnavn | sidemenyen, `<button class="tab" …>` |
| Forsida | `<section id="panel-oversikt">` |
| Fagstoff | `<section id="panel-a">` til `panel-e` |
| Oppgaver | `<details class="task-item">` — spørsmål i `<summary>`, løsning i `.task-sol` |
| Sjekkliste | `const CHECKS` i det første `<script>` |
| Flashcards | `const CARDS` — `[kategori, begrep, forklaring, eksempel]` |
| Quiz | `const QUIZ` — `[del, spørsmål, [alternativer], riktig indeks, forklaring]` |
| Formelark | `<section id="panel-formler">` |
| Kompetansemål | `<section id="panel-mal">` |

Nyttige klasser i innholdet: `.card`, `.box box--key`, `.formula`, `.data` (tabell),
`.timeline`, `.fig` med `<figcaption>`, `.chip`, `.math`, `.u` (enhet), `.small`, `.dim`.
