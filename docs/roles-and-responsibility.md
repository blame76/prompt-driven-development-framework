# Rollen & Verantwortung im Prompt-Driven Development

Prompt-Driven Development (PDD) funktioniert nur, wenn klar ist,
**wer welche Verantwortung trägt** – und welche Verantwortung ausdrücklich
*nicht* delegiert werden kann.

Dieses Dokument beschreibt die drei zentralen Rollen im PDD-Kontext:

1. **Der Mensch**  
2. **Die KI**  
3. **Das System (Kontext & Constraints)**

PDD ist kein Dialog zwischen Mensch und Maschine.  
Es ist ein **Verantwortungsmodell**.

---

## 1. Die Rolle des Menschen

Der Mensch ist die **entscheidende Instanz** in jedem PDD-Prozess.

### Verantwortlichkeiten

- **Ziele definieren**  
  Der Mensch entscheidet, *was* erreicht werden soll – nicht die KI.

- **Spezifikationen formulieren**  
  Anforderungen, Kriterien, Annahmen und Grenzen müssen explizit gemacht werden.

- **Kontext kuratieren**  
  Nicht alles, was bekannt ist, ist relevant.  
  Der Mensch entscheidet, *welcher* Kontext notwendig ist.

- **Ergebnisse prüfen**  
  Die KI liefert Vorschläge.  
  Der Mensch bewertet sie anhand klarer Kriterien.

- **Konsequenzen tragen**  
  Jede Entscheidung hat Auswirkungen.  
  Verantwortung bleibt beim Menschen – immer.

### Was der Mensch nicht tun darf

- Entscheidungen an die KI delegieren  
- Unklare Ziele durch „mal schauen“ ersetzen  
- Plausibilität mit Korrektheit verwechseln  
- Ergebnisse akzeptieren, weil sie gut formuliert sind

**Kurz:**  
Der Mensch denkt. Die KI unterstützt.  
Nicht umgekehrt.

---

## 2. Die Rolle der KI

Die KI ist ein **Werkzeug zur Strukturierung, Beschleunigung und Spiegelung von Denken**.

### Verantwortlichkeiten

- **Vorschläge generieren**  
  Die KI liefert Optionen, Alternativen, Varianten.

- **Strukturen sichtbar machen**  
  Sie hilft, Muster, Lücken und Inkonsistenzen aufzudecken.

- **Spezifikationen verfeinern**  
  Die KI kann Anforderungen präzisieren – aber nicht definieren.

- **Qualität steigern**  
  Durch Wiederholung, Variation und kritische Rückfragen.

### Was die KI nicht leisten kann

- Verantwortung übernehmen  
- Entscheidungen treffen  
- Kontext verstehen, der nicht explizit gegeben wurde  
- Fachliche Korrektheit garantieren  
- Risiken bewerten

**Kurz:**  
Die KI ist ein Verstärker – kein Entscheider.

---

## 3. Die Rolle des Systems (Kontext & Constraints)

Das System ist der **Rahmen**, in dem Mensch und KI arbeiten.

Es besteht aus:

- Domänenlogik  
- Geschäftsregeln  
- technischen Constraints  
- organisatorischen Vorgaben  
- Qualitätskriterien  
- Risiken & Konsequenzen  

### Verantwortlichkeiten des Systems

- **Grenzen definieren**  
  Was ist erlaubt? Was ist ausgeschlossen?

- **Konsequenzen sichtbar machen**  
  Welche Auswirkungen haben Entscheidungen?

- **Qualitätsmaßstäbe festlegen**  
  Was bedeutet „gut“ in diesem Kontext?

- **Stabilität sichern**  
  Das System verhindert, dass Entscheidungen beliebig werden.

### Was das System nicht leisten kann

- Unklare Anforderungen kompensieren  
- Verantwortung ersetzen  
- Fehlende Kriterien durch „Best Practices“ auffüllen

**Kurz:**  
Das System ist der Rahmen, der verhindert, dass PDD zum Ratespiel wird.

---

## Zusammenspiel der Rollen

PDD funktioniert nur, wenn die Rollen **klar getrennt**, aber **eng verzahnt** sind:

- Der **Mensch** definiert Ziele, Kriterien und Verantwortung.  
- Die **KI** liefert Vorschläge, Strukturen und Varianten.  
- Das **System** gibt Grenzen, Konsequenzen und Qualitätsmaßstäbe vor.

Wenn eine dieser Rollen unscharf wird, entstehen typische Anti-Patterns:

- Delegierte Verantwortung  
- Plausibilitätsakzeptanz  
- Kontext-Überladung  
- Wunschzettel-Prompts  
- Iteration ohne Lernschleife

---

## Leitprinzip

> PDD ist kein Dialog zwischen Mensch und Maschine.  
> Es ist ein Prozess, der Verantwortung explizit macht.

