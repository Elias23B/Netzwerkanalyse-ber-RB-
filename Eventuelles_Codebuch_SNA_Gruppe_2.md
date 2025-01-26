# Codebuch für die Transferanalyse von RB 

## Edge-Liste

| **Spalte**     | **Beschreibung**                                                                    | **Beispiel**              |
|-----------------|------------------------------------------------------------------------------------|---------------------------|
| `From`         | Abgebender Verein oder Spieler (als ID).                                           | RBS (FC Red Bull Salzburg)|
| `To`           | Aufnehmender Verein (als ID).                                                     | RBL (RB Leipzig)          |
| `Weight`       | Gewichtung des Transfers in Millionen Euro (z. B. Transferkosten, bei ablösefrei: 0). | 15.00                   |
| `Transferart`  | Art des Transfers (Kauf, Leihe, ablösefrei, Leih-Ende).                            | Kauf                      |
| `Saison`       | Saison des Transfers (z. B. 2020/21).                                              | 2020/21                   |

---

## Node-Liste

| **Spalte**     | **Beschreibung**                                                                    | **Beispiel**              |
|-----------------|------------------------------------------------------------------------------------|---------------------------|
| `ID`           | Eindeutige ID für jeden Spieler oder Verein.                                       | RBS                       |
| `Name`         | Vollständiger Name des Spielers oder Vereins.                                      | FC Red Bull Salzburg      |
| `Typ`          | Typ des Knotens: **1 für Spieler, 2 für Verein**.                                  | 2                         |
| `Alter`        | Alter des Spielers zum Zeitpunkt des Transfers (bei Vereinen: leer).               | 25                        |
| `Nationalität` | Nationalität des Spielers (bei Vereinen: leer).                                    | Ungarn                    |
| `Land`         | Land des Vereins (bei Spielern: leer).                                             | Österreich                |
