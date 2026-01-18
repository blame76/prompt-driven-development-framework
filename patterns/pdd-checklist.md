# Prompt-Driven Development – Checkliste

Diese Checkliste ist kein Qualitätsversprechen.  
Sie ist ein letzter Realitätscheck, bevor ein Prompt ernsthaft genutzt wird.

Wenn du mehrere Punkte nicht klar beantworten kannst,  
ist der Prompt wahrscheinlich zu früh.

---

## 1. Ziel & Erwartung

☐ Kann ich in einem Satz sagen, was das Ziel dieses Prompts ist?  
☐ Beschreibt das Ziel ein Ergebnis – nicht einen Lösungsweg?  
☐ Ist klar, wann das Ziel erreicht ist?

**Merksatz:**  
Wenn das Ziel vage bleibt, wird das Ergebnis plausibel – aber zufällig.

---

## 2. Prüfbarkeit

☐ Woran erkenne ich, ob das Ergebnis richtig oder falsch ist?  
☐ Gibt es explizite Kriterien oder Akzeptanzbedingungen?  
☐ Könnte eine andere Person das Ergebnis überprüfen, ohne mich zu fragen?

**Grundsatz:**  
Was nicht prüfbar ist, ist keine Spezifikation.

---

## 3. Annahmen & Kontext

☐ Welche Annahmen treffe ich gerade – und habe ich sie explizit gemacht?  
☐ Welche Informationen fehlen bewusst?  
☐ Habe ich relevante Randbedingungen genannt (Domäne, Technik, Constraints)?

**PDD-Perspektive:**  
Alles, was nicht im Prompt steht, existiert für die KI nicht.

---

## 4. Verantwortung

☐ Welche Entscheidungen will ich nicht an die KI delegieren?  
☐ Nutze ich den Prompt zur Unterstützung – oder zur Vermeidung eigener Entscheidungen?  
☐ Könnte ich das Ergebnis fachlich vertreten, auch ohne auf die KI zu verweisen?

**Grundsatz:**  
Die KI kann Vorschläge machen.  
Verantwortung bleibt nicht optional.

---

## 5. Konsequenzen

☐ Welche Folgen hätte ein falsches oder unvollständiges Ergebnis?  
☐ Ist das Risiko der Aufgabe bewusst – oder nur implizit?  
☐ Passt die Tiefe des Prompts zum Risiko der Entscheidung?

**Regel:**  
Je höher die Konsequenzen, desto höher die Spezifikationspflicht.

---

## 6. Klarheit vor Vollständigkeit

☐ Ist der Prompt strukturiert und priorisiert?  
☐ Enthält er nur Kontext, der für diese Entscheidung relevant ist?  
☐ Würde weniger Kontext das Ziel klarer machen?

**Erkenntnis:**  
Mehr Kontext ist kein Ersatz für Klarheit.

---

## 7. Lernfähigkeit

☐ Was lerne ich, wenn das Ergebnis nicht wie erwartet ist?  
☐ Kann ich erklären, warum eine Änderung am Prompt sinnvoll wäre?  
☐ Ist dieser Prompt als Artefakt wiederverwendbar oder versionierbar?

**Warnung:**  
Ohne Lernschleife ist Prompting nur Raten.

---

## 8. Plausibilitätsfalle

☐ Überzeuge ich mich gerade durch Sprache statt durch Kriterien?  
☐ Würde ich das Ergebnis auch akzeptieren, wenn es schlechter formuliert wäre?  
☐ Verwechsel ich Vertrautheit mit Korrektheit?

**Merksatz:**  
Gute Sprache ist kein Qualitätsmerkmal.

---

## Minimal-Check (wenn es schnell gehen muss)

Wenn du nur 30 Sekunden hast, beantworte diese drei Fragen:

1. **Was genau erwarte ich – überprüfbar?**  
2. **Welche Entscheidung bleibt meine?**  
3. **Was passiert, wenn das Ergebnis falsch ist?**

Wenn eine davon unklar ist:  
👉 Prompt überarbeiten.

---

## Abschlusssatz

Prompt-Driven Development beginnt nicht mit der Frage  
„Was soll die KI tun?“  
sondern mit  
**„Was bin ich bereit zu verantworten?“**
