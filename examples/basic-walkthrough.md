# PDD Walkthrough – Ein einfaches, vollständiges Beispiel

Dieses Beispiel zeigt Schritt für Schritt, wie Prompt-Driven Development (PDD)
in der Praxis funktioniert.  
Es ist bewusst klein gehalten, um den Fokus auf **Denken, Struktur und Verantwortung**
zu legen – nicht auf Code.

---

# 1. Ausgangssituation

Eine Entwickler:in möchte eine Funktion entwerfen, die prüft,
ob ein Warenkorb für den Checkout gültig ist.

Die naive Frage wäre:

> „Schreib mir eine Funktion, die prüft, ob ein Warenkorb gültig ist.“

Das ist ein klassischer **Wunschzettel-Prompt**.  
PDD beginnt anders.

---

# 2. Schritt: Ziel definieren

**Ziel (in einem Satz):**

> Eine überprüfbare Liste von Kriterien, wann ein Warenkorb als „checkout-fähig“ gilt.

**Nicht das Ziel:**

- Code
- Implementierung
- Optimierung
- Best Practices

---

# 3. Schritt: Prüfbarkeit herstellen

**Akzeptanzkriterien:**

- Die Kriterien müssen eindeutig sein  
- Sie müssen unabhängig vom Code überprüfbar sein  
- Eine dritte Person muss sie verstehen können  
- Keine impliziten Annahmen

---

# 4. Schritt: Annahmen explizit machen

**Explizite Annahmen:**

- Es handelt sich um einen typischen E-Commerce-Warenkorb  
- Preise sind bereits berechnet  
- Verfügbarkeit ist *nicht* Teil dieser Prüfung  
- Rabatte sind bereits angewendet  
- Der Warenkorb enthält mindestens 1 Position

**Bewusst ausgeschlossen:**

- Steuerberechnung  
- Versandlogik  
- Payment-Provider-Details

---

# 5. Schritt: Verantwortung klären

**Was die KI tun darf:**

- Kriterien strukturieren  
- Lücken sichtbar machen  
- Alternativen vorschlagen

**Was die KI nicht tun darf:**

- Geschäftslogik erfinden  
- Annahmen ergänzen  
- Entscheidungen treffen

---

# 6. Schritt: Der eigentliche Prompt

```text
Ziel:
Erstelle eine überprüfbare Liste von Kriterien, wann ein Warenkorb im E-Commerce
als „checkout-fähig“ gilt.

Kontext:
- Preise sind bereits berechnet
- Rabatte sind angewendet
- Verfügbarkeit wird nicht geprüft
- Steuerberechnung ist ausgeschlossen
- Versandlogik ist ausgeschlossen
- Der Warenkorb enthält mindestens 1 Position

Anforderungen:
- Kriterien müssen eindeutig und testbar sein
- Keine impliziten Annahmen
- Keine Architektur- oder Implementierungsvorschläge
- Keine Best Practices

Format:
- Liste nummerierter Kriterien
- Jeder Punkt maximal 1 Satz
```

# 7. Schritt: Ergebnis prüfen

Angenommen, die KI liefert:

1. Der Warenkorb enthält mindestens eine Position.  
2. Jede Position hat einen gültigen Preis.  
3. Der Gesamtpreis ist größer als 0.  
4. Alle Pflichtfelder des Kundenprofils sind ausgefüllt.  
5. Die Lieferadresse ist vollständig.  
6. Es existiert eine gültige Zahlungsmethode.

**Bewertung:**

- Punkt 1–3: gut  
- Punkt 4–6: **falsch**, weil sie nicht Teil des Kontexts sind  
  (Checkout-Fähigkeit ≠ Kundenprofil-Vollständigkeit)

**Erkenntnis:**  
Die KI hat Lücken mit plausiblen Annahmen gefüllt → Anti-Pattern 2.

---

# 8. Schritt: Iteration mit Lernschleife

**Hypothese:**  
Die KI ergänzt Kundenprofil-Daten, weil der Prompt nicht klar genug trennt
zwischen „Warenkorb“ und „Checkout-Prozess“.

**Verbesserung am Prompt:**

```text
Ergänzung:
Der Prompt bezieht sich ausschließlich auf den Warenkorb.
Kundenprofil, Adressen und Zahlungsmethoden sind ausdrücklich ausgeschlossen.
```

**Erwartung:**  
Die KI liefert jetzt nur warenkorbbezogene Kriterien.

---

# 9. Schritt: Finales Ergebnis (nach Iteration)

1. Der Warenkorb enthält mindestens eine Position.  
2. Jede Position hat einen gültigen Preis.  
3. Der Gesamtpreis ist größer als 0.  
4. Alle Positionen sind aktiv und nicht gelöscht.  
5. Der Warenkorb enthält keine negativen Mengen.  
6. Der Warenkorb enthält keine ungültigen Rabatte.

**Bewertung:**  
- vollständig  
- prüfbar  
- kontextgerecht  
- ohne implizite Annahmen  

---

# 10. Schritt: Artefakt erstellen

Das finale Ergebnis wird als **Spezifikation** abgelegt:

- versionierbar  
- nachvollziehbar  
- überprüfbar  
- wiederverwendbar  

Beispiel: `/examples/cart-checkout-criteria.md`

---

# Fazit

Dieses Beispiel zeigt:

- PDD beginnt **vor** dem Prompt  
- Spezifikation schlägt Kreativität  
- KI verstärkt Klarheit – oder Unklarheit  
- Iteration braucht eine Lernschleife  
- Verantwortung bleibt beim Menschen  

PDD ist kein Weg, schneller zu arbeiten.  
Es ist ein Weg, **besser zu denken**, bevor Arbeit entsteht.


# Wichtig: Anmerkungen zur Ergebnis-Präzision

**Hinweis:** Dies ist ein Beispiel für kritische Prüfung im PDD-Prozess – keine Blaupause oder "production-ready"-Spezifikation. In der Praxis würden Geschäftslogik, Domänenkontext und zusätzliche Rahmenbedingungen berücksichtigt werden.

---

## Beispiel: Von "gut" zu "präzise"

**Original-Liste (KI-Antwort nach Verbesserung):**
1. Der Warenkorb enthält mindestens eine Position.  
2. Jede Position hat einen gültigen Preis.  
3. Der Gesamtpreis ist größer als 0.  
4. Alle Positionen sind aktiv und nicht gelöscht.  
5. Der Warenkorb enthält keine negativen Mengen.  
6. Der Warenkorb enthält keine ungültigen Rabatte.

--- LESS IS A POSSIBILITY - WENIGER IST AUCH EINE MÖGLICHKEIT

