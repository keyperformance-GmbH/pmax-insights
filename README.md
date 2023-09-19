# pmax-insights Google Ads Script - Datenanalyse und Reporting

Dieses Skript ist dafür ausgelegt, verschiedene Arten von Daten aus Google Ads zu extrahieren und in einem Google Spreadsheet zu speichern. Das Skript verwendet die Google Ads API, um Abfragen für verschiedene Metriken und Dimensionen zu erstellen und die Ergebnisse in bestimmten Arbeitsblättern des Spreadsheets zu speichern.

## Funktionen des Skripts

### `main()`
Dies ist die Hauptfunktion, die alle anderen Funktionen und Abfragen steuert. 

#### Variablen
- `ss`: Referenz zum Google Spreadsheet, in dem die Daten gespeichert werden sollen.
- `zombieDays`: Anzahl der Tage, die zur Identifikation von "Zombie"-Produkten (Produkten ohne Klicks) verwendet werden.
- `prodDays`: Anzahl der Tage, die zur Identifikation von "Langzeit"-Produkten verwendet werden.

#### Abfragen
Die Funktion baut verschiedene SQL-ähnliche Abfragen für die Google Ads API auf. Diese Abfragen enthalten unterschiedliche Metriken und Dimensionen, die von der API extrahiert werden sollen.

### `runReport(q, sh)`

Diese Funktion führt eine Abfrage aus und speichert die Ergebnisse in einem bestimmten Arbeitsblatt des Google Spreadsheets.

#### Parameter
- `q`: Die Abfrage, die ausgeführt werden soll.
- `sh`: Das Arbeitsblatt, in dem die Ergebnisse gespeichert werden sollen.

## Anleitung zur Verwendung
1. Kopieren Sie das Google Spreadsheet von diesem [Link](https://docs.google.com/spreadsheets/d/1aGOBOLNUjEIwwlYuS0D3fcIimRnzGdLSJxVd9rHOQ0E/copy).
2. Fügen Sie die URL des kopierten Spreadsheets in die Variable `ss` ein.
3. Führen Sie das Skript aus.

## Wichtige Hinweise
Ändern Sie keinen Code unter der Zeile `// don’t change any code below this line`.

## Abhängigkeiten
- Google Ads API
- Google Apps Script

## Version
v28 - Zusätzliche 180-Tage-Produktdaten im neuen Tab `r_prod_t_180`

---

Fügen Sie diese Readme-Datei in Ihr GitHub-Repository ein, um anderen Nutzern die Verwendung des Skripts zu erleichtern.
