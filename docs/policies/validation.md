# Policy: Validation

## 1. Zweck
Validation stellt sicher, dass Ergebnisse objektiv überprüfbar sind – unabhängig von Stil, Sprache oder Überzeugungskraft.

## 2. Definition
Validation bedeutet:
- Kriterien sind eindeutig.
- Ergebnisse sind testbar.
- Annahmen werden eingehalten.
- Keine Plausibilitätsakzeptanz.

## 3. Metriken
- Validation Coverage (% der Kriterien, die erfüllt sind)
- Anzahl nicht prüfbarer Aussagen
- Anzahl Verstöße gegen Annahmen
- Validation‑Score (0.0–1.0)

## 4. Typische Verstöße
- „Klingt gut“ als Akzeptanzgrund
- fehlende Prüfkriterien
- Vermischung von Meinung und Spezifikation
- untestbare Aussagen

## 5. Beispiele
**Gut:**  
„Der Gesamtpreis ist größer als 0.“

**Schlecht:**  
„Der Warenkorb wirkt sinnvoll.“

## 6. Default‑Thresholds
- Validation Coverage ≥ **0.9**
- Validation‑Score ≥ **0.85**

**Begründung:**  
Unterhalb dieser Schwelle ist die Spezifikation nicht robust genug für Automatisierung.

## 7. Grenzen
Validation prüft *Ergebnisse*, nicht *Ziele*.  
Ein valides Ergebnis kann ein falsches Ziel erfüllen.

