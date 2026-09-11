# Kjemi 1 — interaktive kapittelsider

To selvstendige nettsider for Kjemi 1 (KJE01-02), én per kapittel. Alt ligger i hver sin
HTML-fil. Åpne fila i en nettleser, eller publiser mappa. Ingen byggesteg, ingen avhengigheter.

| Fil | Kapittel |
| --- | --- |
| `index.html` | Kapittel 1: Atomer, molekyler og ioner |
| `kapittel2.html` | Kapittel 2: Kjemiske bindinger |

Sidene lenker til hverandre nederst i sidemenyen.

## Søk

Begge sidene har et søk som åpnes fra topplinja, med tasten `/` eller Ctrl/Cmd+K. Det leter
gjennom overskrifter, oppgaver med fasit, figurtekster, tabeller og flashcard-begreper, og går
rett til treffet: riktig fane, oppgaven åpnes, sida ruller dit og treffet blinker. Piltaster og
Enter styrer trefflista. Tall skrevet med komma og punktum finner det samme.

## Kapittel 1 — Atomer, molekyler og ioner

| Del | Tema |
| --- | --- |
| Innledning | Hva kjemi er, fysiske og kjemiske endringer, grønn kjemi, modeller, enkle reaksjoner |
| 1.1 | Atomet: elektronet, protonet, nøytronet og forsøkene som avslørte dem |
| 1.2 | Grunnstoffer og isotoper, atomnummer og massetall |
| 1.3 | Elektronskall, 2n²-regelen og oktettregelen |
| 1.4 | Mendelejevs periodiske system, grupper og perioder |
| 1.5–1.8 | Kjemiske forbindelser, salter, formelenhet, ioneladninger og ionespalting |
| 1.9 | Lys: bølge eller partikkel, fotoelektrisk effekt |
| 1.10 | Bohrs modell, eksitasjon, atomspektre og elektronets bølgenatur |
| 1.11–1.12 | Atomorbitaler, underskall, elektronkonfigurasjon og blokkene |

Alle oppgavene fra kapitlet med løsning, aktivitetene A 1.1–A 1.10, øvingene Ø 1.1–Ø 1.5,
laboratoriehåndbok med feilkilder og måleusikkerhet, temasidene om grunnstoffer, formelark,
59 flashcards, 32 quizspørsmål og 10 sant/usant-påstander med forklaring.

**Seks interaktive verktøy:** interaktivt periodisk system med alle 118 grunnstoffene,
skallbygger for de 20 første, isotopregner, saltbygger som balanserer ladningene,
lysregner (λ ↔ f ↔ E) og flammeprøve med linjespekter for seks salter. I tillegg
elektronkonfigurasjonsverktøyet og standardavviksregneren i laboratoriedelen.

## Kapittel 2 — Kjemiske bindinger

| Del | Tema |
| --- | --- |
| 2.1 | Periodiske egenskaper: Coulombs lov, atomradius, elektronegativitet, ioniseringsenergi |
| 2.2 | Elektronegativitet og bindingstype: ionebinding, elektronparbinding, polar binding |
| 2.3 | Dipoler og molekylgeometri (VSEPR), resonans |
| 2.4 | Metallbinding |
| 2.5 | Bindinger mellom molekyler: van der Waals, dipol-dipol, ion-dipol, hydrogenbindinger |
| 2.6 | Bindingsforholdene i vann og is |
| 2.7 | Oversikt over bindingstyper og oppsummering |

Alle oppgavene til 2.1–2.5 med løsning, temasidene om kjernekrefter (fisjon, fusjon, thorium
og solenergi) og om utnyttelse av fiskeråstoff, formelark, 39 flashcards, 25 quizspørsmål og
11 sant/usant-påstander.

**Fem interaktive verktøy:** trendgraf for atomradius, ioniseringsenergi og elektronegativitet,
bindingstypeverktøy som viser ΔEN på en skala, VSEPR-verktøy for åtte molekyler og ioner,
massetetthetskurven for vann med maksimum ved 3,97 °C, og energiregner for E = mc².

## Om oppgavetekstene

Noen oppgavetekster i kilden var ufullstendige. Der er de fylt ut slik at de gir mening, i tråd
med det delkapitlet de hører til. Løsningsforslagene er skrevet ut i sin helhet, og
programmeringsoppgavene har hele det ferdige programmet i fasiten.

## Teknisk

- Én fil per kapittel med HTML, CSS og JavaScript. Ingen rammeverk.
- Lyst og mørkt tema. Følger systemet til du velger selv, og virker uten JavaScript.
- Skiplenke, synlig fokusmarkering, tastaturstyrt flashcard og tekstalternativ til hvert lerret.
- Trykkmål på minst 44 px på berøringsskjerm, og ingen vannrett rulling ned til 360 px.
- Dyplenker: hver fane har sin egen adresse, som `#del-a`, og tilbakeknappen virker.
- Søket bygger indeksen sin fra sida selv, første gang det åpnes.
- Respekterer `prefers-reduced-motion`.
- Framdrift og flashcard-statistikk ligger i `localStorage` og sendes ingen steder.
