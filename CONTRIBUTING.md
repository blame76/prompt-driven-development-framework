# Contributing Guide – Prompt-Driven Development Framework

Vielen Dank für dein Interesse an diesem Framework.  
Dieses Repository ist kein Code-Projekt, sondern ein **Meta-Framework für Denken, Spezifikation und Verantwortung** im Umgang mit KI.

Beiträge sind willkommen – aber sie folgen denselben Prinzipien wie PDD selbst:
**klar, prüfbar, verantwortbar, reproduzierbar.**

---

# 1. Grundhaltung

Dieses Framework ist kein Ort für schnelle Ideen oder spontane Eingebungen.  
Beiträge sollen:

- **klar begründet** sein  
- **explizite Annahmen** enthalten  
- **prüfbar** sein  
- **verantwortbare Entscheidungen** treffen  
- **tool-agnostisch** bleiben  

Wenn du etwas beiträgst, übernimmst du Verantwortung für die Konsequenzen.

---

# 2. Arten von Beiträgen

Du kannst beitragen durch:

- neue oder verbesserte **Dokumentation**
- neue **Policies**, **Patterns** oder **Anti-Patterns**
- Erweiterungen der **Automation Architecture**
- Verbesserungen an **Schemas** oder **Beispielen**
- neue **Issue Templates** oder **Artefakt-Templates**
- Korrekturen von Fehlern, Unklarheiten oder Inkonsistenzen

**Nicht** erwünscht sind:

- Tool-spezifische Implementierungen  
- Prompt-Sammlungen ohne Spezifikationswert  
- Marketing, Hype oder „10× Productivity“-Material  
- Code, der nicht Teil eines Beispiels ist  

---

# 3. Vor jedem Beitrag: Issue anlegen

Jeder Beitrag beginnt mit einem **Issue**, das das PDD-Issue-Template nutzt.

Das Issue muss enthalten:

- **Ziel** (abgegrenzt, präzise)
- **Prüfbarkeit** (Kriterien)
- **Annahmen** (explizit)
- **Verantwortung** (was entscheidest du selbst?)
- **Kontext**
- **Risiken**
- **Artefakte**

Ohne Issue → kein PR.

---

# 4. Anforderungen an Pull Requests

Ein PR muss:

- auf ein existierendes Issue verweisen  
- ein **Artefakt** erzeugen oder verbessern  
- **keine impliziten Annahmen** enthalten  
- **keine Verantwortung an KI delegieren**  
- **prüfbar** sein  
- **reproduzierbar** sein  
- **tool-agnostisch** bleiben  

Jeder PR muss ein **„Was wurde verändert und warum?“** enthalten.

---

# 5. Qualitätskriterien (Gates)

Jeder Beitrag wird gegen die folgenden Policies geprüft:

### **Clarity**
- Ist das Ziel klar?
- Sind Begriffe eindeutig?
- Sind Annahmen explizit?

### **Responsibility**
- Trifft der Mensch die Entscheidungen?
- Werden keine KI-Urteile übernommen?

### **Validation**
- Sind die Ergebnisse testbar?
- Sind Kriterien erfüllt?

### **Decomposition**
- Ist das Problem sinnvoll zerlegt?
- Sind Teilaufgaben unabhängig prüfbar?

Wenn ein Gate nicht bestanden wird, wird der PR nicht gemerged.

---

# 6. Struktur und Stil

Beiträge sollen:

- präzise sein  
- minimalistisch sein  
- ohne Buzzwords auskommen  
- keine Tool-Abhängigkeiten einführen  
- Markdown nutzen  
- Diagramme in **Mermaid** schreiben  
- Beispiele in **/examples/** ablegen  
- Schemas in **/schemas/** ablegen  
- Policies in **/docs/policies/** ablegen  

---

# 7. Wie du mit KI arbeitest (wenn du möchtest)

Du darfst KI nutzen – aber:

- **KI ist Vorschlagsgenerator, nicht Entscheider**
- Ergebnisse müssen **validiert** werden
- Prompts gehören **nicht** in PRs
- Artefakte müssen **menschlich verantwortet** sein

---

# 8. Review-Prozess

Ein PR wird gemerged, wenn:

- alle Gates bestanden sind  
- die Änderungen konsistent mit dem Framework sind  
- die Dokumentation vollständig ist  
- die Konsequenzen verstanden und akzeptiert sind  

Der Review ist **kollaborativ**, aber **streng**.

---

# 9. Lizenz & Ownership

Mit deinem Beitrag erklärst du dich einverstanden, dass:

- dein Beitrag unter der Projektlizenz veröffentlicht wird  
- dein Beitrag Teil eines öffentlichen Meta-Frameworks wird  
- du keine exklusiven Rechte an einzelnen Texten behältst  

---

# 10. Abschlusssatz

> Dieses Framework lebt von Klarheit, Verantwortung und reproduzierbarem Denken.  
> Wenn du dazu beitragen möchtest, bist du herzlich willkommen – aber bring deine beste Version mit.
