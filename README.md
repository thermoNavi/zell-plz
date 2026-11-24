# ThermoNavi: Zensus-Rasterzellen und Postleitzahlen

`zell_plz.csv.zip` enthält genau eine Datei, `zell_plz.csv`. Sie enthält
3.087.816 Zuordnungen in UTF-8:

- `cell_id`: Kennung der bewohnten 100-m-Rasterzelle aus dem Zensus 2022.
- `plz`: fünfstellige Postleitzahl als Text (führende Nullen beibehalten).

Eine Zelle wird zugeordnet, wenn ihr Mittelpunkt von genau einem
fünfstelligen PLZ-Gebiet abgedeckt wird. Nicht zuordenbare Zellen sind nicht
enthalten. Die Datei enthält keine Temperaturwerte oder Einwohnerzahlen.
Der Datenstand ist Zensus 2022 mit OSM-PLZ-Auszug `2024.12`. Der Zeitraum
2007–2025 betrifft die separat berechneten Temperaturprofile, nicht diese
Zuordnung.

## Quellen und Lizenz

- **Postleitzahlgebiete:** © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright),
  [ODbL 1.0](https://opendatacommons.org/licenses/odbl/1-0/). Verwendeter
  [PLZ-Auszug 2024.12 von yetzt/postleitzahlen](https://github.com/yetzt/postleitzahlen/releases/tag/2024.12).
- **Rasterzellen:** Statistische Ämter des Bundes und der Länder, [Zensus 2022,
  Bevölkerungszahl im 100-m-Raster](https://www.destatis.de/static/DE/zensus/gitterdaten/Zensus2022_Bevoelkerungszahl.zip),
  [Datenlizenz Deutschland – Namensnennung – Version 2.0](https://www.govdata.de/dl-de/by-2-0).
- **Verarbeitung:** ThermoNavi; Geometrien umprojiziert und bei Bedarf repariert,
  Zensus-Raster gefiltert und Zellmittelpunkte PLZ-Gebieten zugeordnet.
  Die Zuordnungsdatenbank wird unter der [ODbL 1.0](https://opendatacommons.org/licenses/odbl/1-0/)
  bereitgestellt. Die Lizenzhinweise der Quelldaten bleiben unberührt.

SHA-256 der entpackten CSV:
`75117ea32ba063277c02c979ded57f29a50360c9c59f87bc5f809be510b32834`.
