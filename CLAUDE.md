# Regole di lavoro per ATCRoom Map Creator

Repository **ATCRoom/MapCreator**: pubblica ATCRoom Map Creator come download separato (deciso dall'utente il 9 novembre 2026).

## Comunicazione
- Rispondi sempre in italiano.
- L'utente prova le build su Windows e le passa ad alcuni amici: ogni build deve essere utilizzabile da chi non è sviluppatore.

## Dove si sviluppa
- Il sorgente si sviluppa in **ATCRoom/TWR-Trainer** (cartella `MapCreator/`): qui si ricopia la cartella `MapCreator/` e `docs/MAP-FORMAT.md` prima di ogni release del Map Creator.
- Alza `<Version>` in `MapCreator/App/ATCRoomMapCreator.csproj` a ogni release.
- Il formato delle mappe deve restare compatibile all'indietro.

## Quando scrivere codice
- Prima proponi; scrivi codice solo dopo un via esplicito ("vai", "parti", "procedi", "ok").
- Niente SDK dotnet in locale: si compila solo tramite GitHub Actions (`.github/workflows/build.yml`).

## Pubblicazione
- Ogni push su `main` pubblica la release `v<Version>` (sostituita a ogni push della stessa versione): su `main` solo quando lo dice l'utente.

## Mappe e dati di terzi
- I file di esempio dell'utente (IVAO, EuroScope, AIP, KML...) non vanno nel repository.
- Le mappe fatte con il Map Creator sono per uso personale e solo per simulazione: mai distribuite.
