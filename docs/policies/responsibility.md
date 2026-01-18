# Policy: Responsibility

## 1. Zweck
Responsibility stellt sicher, dass Entscheidungen dort getroffen werden, wo sie hingehören: beim Menschen.

## 2. Definition
Responsibility bedeutet:
- Die KI schlägt vor.
- Der Mensch entscheidet.
- Verantwortungsgrenzen sind explizit.
- Keine Delegation von Urteilen, die Konsequenzen tragen.

## 3. Metriken
- Anzahl Responsibility Breaches
- Anzahl KI‑Entscheidungen ohne menschliche Freigabe
- Anteil menschlicher Entscheidungen pro Task

## 4. Typische Verstöße
- KI ergänzt Geschäftslogik
- KI entscheidet über Risiken
- KI bewertet Alternativen ohne Kriterien
- Mensch akzeptiert Ergebnisse aufgrund von Plausibilität

## 5. Beispiele
**Gut:**  
„Die KI schlägt drei Alternativen vor, der Mensch wählt anhand der Kriterien.“

**Schlecht:**  
„Die KI entscheidet, welche Architektur am besten ist.“

## 6. Default‑Thresholds
- Responsibility Breaches = **0**
- Jede Entscheidung mit Risiko-Level ≥ medium muss menschlich bestätigt werden.

**Begründung:**  
Verantwortung ist nicht teilbar.

## 7. Grenzen
Responsibility bewertet *Entscheidungswege*, nicht die Qualität der Entscheidung selbst.

