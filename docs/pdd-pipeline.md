# The PDD Pipeline

Diese Pipeline beschreibt keinen optimalen Weg zur Lösung.  
Sie beschreibt einen **verantwortbaren Weg zum Denken**, bevor eine Lösung entsteht.

Prompt-Driven Development beginnt **nicht mit der KI**  
und endet **nicht mit einem Ergebnis**,  
sondern mit einem **Artefakt**, für das ein Mensch Verantwortung trägt.

---

## 1. Ziel definieren

**Zweck:**  
Klarheit darüber herstellen, *was* erreicht werden soll – und was ausdrücklich nicht.

### Leitfragen

* Was soll erreicht werden?
* Welches Problem wird bearbeitet?
* Für wen ist das Ergebnis relevant?

### Ebenso wichtig

* Was ist **nicht** das Ziel?
* Welche Ergebnisse wären zwar plausibel, aber unerwünscht?
* Welche Fragen werden bewusst **nicht** beantwortet?

> Ein Ziel ist nur dann brauchbar, wenn es Abgrenzung enthält.  
> Alles andere ist ein Wunsch.

---

## 2. Prüfbarkeit herstellen

**Zweck:**  
Ein Ergebnis muss bewertbar sein – unabhängig von Sprache, Stil oder Überzeugungskraft.

### Leitfragen

* Woran erkenne ich, ob das Ergebnis richtig oder falsch ist?
* Welche Kriterien gelten?
* Sind diese Kriterien unabhängig von einer konkreten Implementierung?

### Mindestanforderung

* Eine dritte Person kann anhand der Kriterien prüfen,  
  ob das Ziel erreicht wurde – ohne Rückfragen.

> Was nicht prüfbar ist, ist keine Spezifikation.  
> Es ist eine Meinung.

---

## 3. Annahmen explizit machen

**Zweck:**  
Verhindern, dass implizite Annahmen unbemerkt in Entscheidungen einfließen.

### Leitfragen

* Welche Annahmen treffe ich über Domäne, Kontext oder System?
* Was halte ich für „gegeben“, ohne es ausgesprochen zu haben?
* Welche Aspekte schließe ich bewusst aus?

### Wichtig

* Annahmen sind erlaubt.  
* **Implizite** Annahmen sind das Problem.

> KI halluziniert nicht im luftleeren Raum.  
> Sie füllt Lücken, die wir offen gelassen haben.

---

## 4. Verantwortung klären

**Zweck:**  
Die Rollen zwischen Mensch und KI sauber trennen.

### Leitfragen

* Welche Entscheidungen treffe ich selbst?
* Wo will ich bewusst keine Delegation?
* Was darf die KI vorschlagen – und was nicht?

### Grundsatz

* Die KI ist ein **Vorschlagsgenerator**  
* Der Mensch bleibt **Entscheidungsträger**

> Verantwortung lässt sich nicht delegieren –  
> nur verschleiern.

---

## 5. Prompt formulieren

**Zweck:**  
Den Denkstand explizit und überprüfbar an die KI übergeben.

Ein PDD-Prompt besteht immer aus klar getrennten Bestandteilen:

### Ziel
* Ein überprüfbares, abgegrenztes Ziel

### Kontext
* Relevante Informationen  
* Keine Vollständigkeit, sondern Relevanz

### Anforderungen
* Kriterien, Bedingungen, Einschränkungen  
* Keine impliziten Erwartungen

### Format
* Klare Vorgaben zur Struktur des Ergebnisses  
* Reduziert Interpretationsspielraum

### Ausschlüsse
* Was ausdrücklich **nicht** geliefert werden soll  
* Besonders wichtig bei impliziten Standardannahmen

> Ein Prompt ist kein Befehl an die KI.  
> Er ist eine explizite Darstellung des eigenen Denkens.

---

## 6. Ergebnis prüfen

**Zweck:**  
Das Ergebnis kritisch bewerten – nicht akzeptieren.

### Prüfdimensionen

* Entspricht es den definierten Kriterien?
* Hält es die expliziten Annahmen ein?
* Überschreitet es Verantwortungsgrenzen?

### Warnsignal

* „Klingt gut“ ist **kein** Prüfkriterium.

> Ein gutes Ergebnis ist nicht das, was überzeugt,  
> sondern das, was überprüfbar richtig ist.

---

## 7. Iteration mit Lernschleife

**Zweck:**  
Verbesserung mit Erkenntnis verbinden – nicht mit Zufall.

Jede Iteration folgt demselben Muster:

### Hypothese
* Warum war das Ergebnis unzureichend?
* Welche Unklarheit hat dazu geführt?

### Änderung
* Gezielte Anpassung am Prompt  
* Keine kosmetischen Korrekturen

### Erwartung
* Was sollte sich konkret verbessern?

### Vergleich
* Was hat sich verändert?
* Entspricht das Ergebnis der Erwartung?

> Iteration ohne Hypothese ist Raten.  
> Raten ist kein Entwicklungsprozess.

---

## 8. Artefakt erstellen

**Zweck:**  
Das Ergebnis aus dem Prompt-Kontext lösen und dauerhaft nutzbar machen.

### Eigenschaften eines Artefakts

* Versionierbar  
* Nachvollziehbar  
* Wiederverwendbar  
* Unabhängig vom ursprünglichen Prompt

### Wichtig

* Der Prompt ist Mittel zum Zweck  
* Das Artefakt ist das Ergebnis

> Wert entsteht nicht im Dialog mit der KI,  
> sondern im Artefakt, das bleibt.

---

[Ziel] → [Prüfbarkeit] → [Annahmen] → [Verantwortung] → [Prompt]
                                       ↑
[Artefakt] ← [Iteration] ← [Prüfung] ← [KI]

## Abschluss

Diese Pipeline ist kein Rezept für Geschwindigkeit.  
Sie ist ein Schutzmechanismus gegen:

* implizite Entscheidungen  
* unklare Verantwortung  
* scheinbar überzeugende Ergebnisse  

Prompt-Driven Development bedeutet nicht,  
mehr KI zu nutzen –  
sondern **bewusster zu arbeiten**, bevor Ergebnisse entstehen.
