# ATCRoom Map Creator

Makes the maps of **AuroraPAR v2 Trainer** and **TWR Trainer** from your own files: IVAO (`.geo .fix .vor .ndb .ap .vfi
.str .mva`), EuroScope (`.ese .sct`), KML / KMZ, an AIP table (PDF). The maps are saved in the open **ATCRoom map
format** ([docs/MAP-FORMAT.md](docs/MAP-FORMAT.md)) into the maps folder shared by the programs.

## Download

**[Releases](https://github.com/ATCRoom/MapCreator/releases/latest)**: `ATCRoomMapCreator-win-x64.zip` (Windows 64-bit,
no installation, .NET not needed). Unzip and run `ATCRoomMapCreator.exe`; Windows may show a SmartScreen warning
(More info → Run anyway). Put it beside `AuroraPARTrainer.exe` to open it from the Maps window of the Trainer.

> **⚠ Personal use only — simulation only.** The Map Creator reads files of any kind (IVAO, VATSIM, AIP, KML…), but the
> maps you make from them are **for your own use only**: **do not distribute them** (no sharing, no uploading) without the
> permission of the owner of the data. They are for flight simulation and training only and **must never be used for
> real-world navigation or air traffic control**.

## What is here

- `MapCreator/Core` — **ATCRoom Maps**, the map format and its importers (a library used by the programs).
- `MapCreator/App` — **ATCRoom Map Creator**, the program.
- `MapCreator/SelfTest` — the checks of the format and the importers, run at every build.

The source is the same as the folder `MapCreator/` of [ATCRoom/TWR-Trainer](https://github.com/ATCRoom/TWR-Trainer),
where it is developed; this repository publishes the program. Free and open source (MIT, see LICENSE).
