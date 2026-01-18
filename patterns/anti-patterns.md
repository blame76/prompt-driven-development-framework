# Anti-Patterns in Prompt-Driven Development

Dieses Dokument beschreibt typische Fehlmuster im Umgang mit KI,
die **nicht durch bessere Modelle**, sondern nur durch **besseres Denken** lösbar sind.

Anti-Patterns sind hier keine Anfängerfehler.
Sie treten besonders häufig bei erfahrenen Entwickler:innen auf.

> Anti-Patterns sind nicht das Gegenteil von Best Practices,  
> sondern das Ergebnis unklarer Verantwortung im Umgang mit KI.

---

## 1. Der Wunschzettel-Prompt

**Symptom**  
Der Prompt beschreibt, *was man gerne hätte* – nicht, *was überprüfbar erwartet wird*.

**Typische Formulierungen**

* „Erstelle mir eine saubere Architektur für …“
* „Optimiere den Code bestmöglich“
* „Mach das robuster / performanter / wartbarer“

**Warum das problematisch ist**

* Begriffe wie „sauber“, „robust“ oder „bestmöglich“ sind **nicht operationalisiert**
* Die KI muss raten, welche Kriterien gemeint sind
* Das Ergebnis klingt überzeugend, ist aber **nicht prüfbar**

**Was stattdessen nötig wäre**

* Explizite Kriterien  
* Akzeptanzbedingungen  
* Ausschlüsse („Was ist *nicht* Teil der Lösung?“)

---

## 2. Die implizite Annahme-Falle

**Symptom**  
Der Prompt setzt stillschweigend Wissen voraus, das nie explizit gemacht wurde.

**Beispiele**

* Domänenlogik wird vorausgesetzt  
* Randbedingungen werden „als klar angenommen“  
* Bestehende Entscheidungen werden nicht erwähnt  

**Warum das problematisch ist**

* KI füllt Lücken mit plausiblen, aber falschen Annahmen  
* Fehler wirken später wie „Halluzinationen“, sind aber **Spezifikationsfehler**

**Typisches Missverständnis**

> „Das hätte die KI doch wissen müssen.“

Nein.  
Was nicht im Prompt oder Kontext steht, **existiert nicht**.

---

## 3. Ergebnis-Akzeptanz durch Plausibilität

**Symptom**  
Ein Ergebnis wird akzeptiert, weil es logisch klingt, gut formuliert ist oder vertraute Muster nutzt.

**Warnsignale**

* „Klingt sinnvoll.“  
* „Sieht sauber aus.“  
* „Das machen andere auch so.“  

**Warum das problematisch ist**

* Sprachliche Qualität wird mit fachlicher Korrektheit verwechselt  
* Entscheidungen werden nicht mehr hinterfragt  
* Verantwortung verschiebt sich implizit zur KI  

**PDD-Perspektive**  
Ein gutes Ergebnis ist nicht das, was überzeugt –  
sondern das, **was überprüfbar richtig ist**.

---

## 4. Prompt-Iteration ohne Lernschleife

**Symptom**  
Prompts werden immer wieder leicht angepasst, ohne systematisch zu reflektieren.

**Typisches Verhalten**

* „Mach es nochmal, aber anders“  
* „Jetzt bitte kürzer“  
* „Berücksichtige noch X“  

**Warum das problematisch ist**

* Es entsteht Trial-and-Error ohne Erkenntnisgewinn  
* Fehlerursachen bleiben unklar  
* Verbesserungen sind nicht reproduzierbar  

**Was fehlt**

Eine sinnvolle Iteration beantwortet drei Fragen:

1. Was war schlecht?  
2. Was soll besser werden?  
3. Woran erkenne ich, dass es besser wurde?

---

## 5. Delegierte Verantwortung

**Symptom**  
Die KI wird implizit zur Entscheidungsinstanz.

**Beispiele**

* Architekturentscheidungen ohne eigene Bewertung  
* Übernahme von Empfehlungen ohne Kontextprüfung  
* „Die KI hat gesagt, das ist Best Practice“  

**Warum das problematisch ist**

* Verantwortung wird verschoben, nicht geteilt  
* Fehler lassen sich nicht mehr sauber zuordnen  
* Lernen findet nicht statt  

**Grundsatz von PDD**

> KI darf Vorschläge machen.  
> Entscheidungen trifft immer der Mensch.

---

## 6. Kontext-Überladung statt Klarheit

**Symptom**  
Der Prompt enthält „alles“, um nichts zu vergessen.

**Erkennbar an**

* sehr langen Kontextblöcken  
* unstrukturierten Code- oder Textmengen  
* fehlender Priorisierung  

**Warum das problematisch ist**

* Relevanz geht verloren  
* Wichtiges wird nicht von Unwichtigem getrennt  
* Die KI optimiert auf falsche Signale  

**PDD-Alternative**

* Kontext ist kuratiert, nicht vollständig  
* Relevanz wird explizit gemacht  
* Alles andere ist Rauschen  

---

## 7. Der Prompt als Ersatz für Denken

**Symptom**  
Der Prompt wird genutzt, um Unsicherheit zu vermeiden.

**Typische Gedanken**

* „Ich lass die KI erstmal überlegen“  
* „Mal schauen, was sie vorschlägt“  
* „Vielleicht sehe ich dann klarer“  

**Warum das problematisch ist**

* Eigene Unklarheit wird nicht adressiert  
* Denken wird ausgelagert, nicht unterstützt  
* Die Qualität des Outputs sinkt zwangsläufig  

**PDD-Haltung**  
Ein Prompt ersetzt kein Denken.  
Er **legt offen**, wie gut gedacht wurde.

---

## Zusammenfassung

Anti-Patterns in PDD entstehen nicht durch schlechte Technik,  
sondern durch **implizites Arbeiten in einem expliziten Medium**.

Wer diese Muster erkennt,

* schreibt weniger Prompts  
* aber bessere  
* und übernimmt wieder Verantwortung für das Ergebnis
