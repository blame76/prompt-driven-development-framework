-------- KI GENERIERTER INHALT --------

# Glossary – Prompt-Driven Development

Dieses Glossar definiert zentrale Begriffe des Prompt-Driven Development (PDD).  
Es schafft eine gemeinsame Sprache für Spezifikation, Verantwortung und Zusammenarbeit mit KI.

---

## **Artefakt**
Ein dauerhaftes Ergebnis des PDD-Prozesses.  
Versionierbar, nachvollziehbar, wiederverwendbar und unabhängig vom ursprünglichen Prompt.

---

## **Annahme**
Eine Aussage, die als gegeben vorausgesetzt wird.  
Explizite Annahmen sind erlaubt.  
**Implizite Annahmen sind ein Risiko**, weil die KI sie mit plausiblen, aber falschen Ergänzungen füllt.

---

## **Ausschluss**
Bewusste Begrenzung des Lösungsraums.  
Definiert, was *nicht* Teil des Ergebnisses sein darf.  
Wichtig, um Standardannahmen der KI zu verhindern.

---

## **Checkliste**
Ein Werkzeug zur Selbstprüfung vor der Prompt-Formulierung.  
Dient der Klarheit, nicht der Automatisierung.

---

## **Coverage (Anforderungsabdeckung)**
Maß dafür, wie viele definierte Kriterien durch ein Ergebnis oder Artefakt überprüfbar erfüllt werden.  
Wird in PDD nicht automatisch gemessen, sondern bewusst reflektiert.

---

## **Dekomposition**
Aufteilung eines komplexen Problems in handhabbare Teilprobleme, die jeweils durch die Pipeline geführt werden können.  
Wichtig für Skalierbarkeit bei hoher Komplexität.

---

## **Ergebnis**
Die Antwort der KI auf einen Prompt.  
Nicht das Ziel des Prozesses, sondern ein Zwischenschritt auf dem Weg zum Artefakt.

---

## **Format**
Strukturelle Vorgabe für die KI-Ausgabe (z. B. Liste, Tabelle, JSON).  
Reduziert Interpretationsspielraum und erhöht Prüfbarkeit.

---

## **Hypothese**
Begründete Annahme darüber, warum ein Ergebnis unzureichend war.  
Grundlage jeder sinnvollen Iteration.

---

## **Iteration**
Gezielte Verbesserung eines Prompts basierend auf Hypothese, Änderung, Erwartung und Vergleich.  
Keine Trial-and-Error-Schleife.

---

## **Kriterium**
Ein überprüfbarer Maßstab zur Bewertung eines Ergebnisses.  
Grundlage für Prüfbarkeit und Verantwortung.

---

## **Kontext**
Kuratiertes Hintergrundwissen, das für die Aufgabe relevant ist.  
Nicht vollständig, sondern bewusst ausgewählt.

---

## **Lernschleife**
Der Mechanismus, durch den Iterationen Erkenntnis erzeugen.  
Ohne Lernschleife ist Prompting nur Raten.

---

## **Plausibilität**
Eigenschaft eines Ergebnisses, logisch oder vertraut zu wirken.  
**Kein Qualitätsmerkmal.**  
Kann fachlich falsch und dennoch überzeugend sein.

---

## **Prompt**
Eine explizite Darstellung des eigenen Denkens, nicht ein Befehl an die KI.  
Besteht aus Ziel, Kontext, Anforderungen, Format und Ausschlüssen.

---

## **Prüfbarkeit**
Fähigkeit, ein Ergebnis objektiv als richtig oder falsch zu bewerten.  
Zentraler Qualitätsmaßstab im PDD.

---

## **Responsibility Breach (Verantwortungsverletzung)**
Wenn die KI Entscheidungen trifft, die dem Menschen vorbehalten sind, oder implizite Annahmen ergänzt.  
Wird durch klare Rollen und Ausschlüsse minimiert.

---

## **Spezifikation**
Eine präzise Beschreibung dessen, was erreicht werden soll.  
Unabhängig von Implementierung, Stil oder Technologie.

---

## **Template**
Vordefinierte Struktur für Prompts, Artefakte oder Reviews.  
Erhöht Wiederverwendbarkeit und Konsistenz.

---

## **Validierung**
Bewertung eines Ergebnisses anhand definierter Kriterien und Annahmen.  
Nicht zu verwechseln mit „klingt gut“.

---

## **Ziel**
Der präzise, abgegrenzte Zweck eines Prompts.  
Definiert, *was* erreicht werden soll – und was nicht.

---

# Abschluss

Dieses Glossar ist kein Wörterbuch, sondern ein **Verantwortungsrahmen**.  
Es stellt sicher, dass Begriffe im PDD-Prozess eindeutig, prüfbar und gemeinsam verstanden werden.
