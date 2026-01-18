# Policy: Decomposition

## 1. Zweck
Dekomposition stellt sicher, dass komplexe Probleme in handhabbare, pipeline‑fähige Teilaufgaben zerlegt werden.

## 2. Definition
Decomposition bedeutet:
- Komplexität wird reduziert.
- Abhängigkeiten werden sichtbar.
- Teilaufgaben sind unabhängig prüfbar.
- Jede Teilaufgabe kann durch die Pipeline laufen.

## 3. Metriken
- Anzahl der Teilaufgaben
- Komplexitätsgrad pro Teilaufgabe
- Abhängigkeitsgraph (Tiefe/Breite)
- Decomposition‑Score (0.0–1.0)

## 4. Typische Verstöße
- „One‑Shot‑Prompts“ für komplexe Probleme
- Vermischung von Analyse und Lösung
- fehlende Abgrenzung zwischen Teilaufgaben
- Pipeline‑Schritte werden übersprungen

## 5. Beispiele
**Gut:**  
„Zuerst Kriterien definieren → dann Datenmodell → dann Validierungslogik.“

**Schlecht:**  
„Erstelle ein komplettes Checkout‑System.“

## 6. Default‑Thresholds
- maximal 1 Abhängigkeitstiefe > 3
- Decomposition‑Score ≥ **0.75**

**Begründung:**  
Tiefe Abhängigkeiten führen zu Fehlerketten und unprüfbaren Ergebnissen.

## 7. Grenzen
Dekomposition bewertet Struktur, nicht Inhalt.  
Eine gut zerlegte falsche Idee bleibt falsch.
