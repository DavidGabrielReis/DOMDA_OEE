# Präsentationsskript — Linie 4 (Abfüllanlage 4-E2G)

**Dauer:** ca. 20 Minuten  
**Zielgruppe:** Business Owner Linie 4  
**Ziel:** Aufmerksamkeit für das Projekt schaffen, Input sammeln, Interessen identifizieren

---

## Folie 1 — Titelfolie & Vorstellung

**Titel:** Datenbasierte Produktionsanalyse — Abfüllanlage 4-E2G

**Inhalt der Folie:**
- Name, Studiengang, dualer Student bei [Firma]
- Projekttitel: „DOMDA" — Datenbasierte OEE-Analyse und Optimierungspotenzialermittlung
- Datum der Präsentation

**Sprechtext:**
> Guten Tag, mein Name ist [Name], ich bin dualer Student im Bereich [Studiengang]. Im Rahmen meines Praxiseinsatzes arbeite ich an einem Projekt, in dem ich Produktionsdaten aus dem OEE-System auswerte, um Optimierungspotenziale sichtbar zu machen. Heute möchte ich Ihnen zeigen, was ich bisher speziell für Ihre Linie 4 — die Abfüllanlage 4-E2G — herausgefunden habe. Mir ist dabei besonders wichtig, Ihren Input zu bekommen: Was ist für Sie relevant? Wo möchten Sie tiefer einsteigen? Was soll ich mir noch genauer anschauen?

**(~1 Minute)**

---

## Folie 2 — Überblick: Was wurde analysiert?

**Titel:** Was wurde analysiert?

**Inhalt der Folie:**
- Datenquelle: OEE-System (Chargen-Daten der Abfüllanlage 4-E2G)
- Analysierter Zeitraum (z. B. Mitte 2024 – März 2026)
- Anzahl ausgewerteter Chargen (nach Bereinigung)
- Verwendete Kennzahl: OEE₂ — reiner Produktions-OEE ohne Kapazitätsfaktor
- Kurze Bullet-Liste der Analysebereiche:
  - OEE-Verlauf über Zeit
  - OEE-Komponenten (Verfügbarkeit, Leistung, Qualität)
  - Bestleistungspotenzial (BDP)
  - Materialvergleich
  - Schichtvergleich
  - Ungeplante Stillstände
  - Korrelationsanalyse

**Sprechtext:**
> Ich habe Chargendaten Ihrer Linie aus dem OEE-System ausgewertet. Nach der Bereinigung — also dem Entfernen von Leerläufen und fehlerhaften Datensätzen — bleiben mehrere tausend Chargen im Analysezeitraum. Die Kennzahl, die ich verwende, ist der sogenannte OEE₂. Das ist der reine Produktions-OEE, bei dem die Kapazitätsauslastung außen vor bleibt — also: Wie effizient läuft die Linie, wenn sie läuft. Ich möchte Ihnen heute sechs Analysebereiche zeigen, die ich daraus abgeleitet habe.

**(~2 Minuten)**

---

## Folie 3 — Monatlicher OEE-Verlauf

**Titel:** Wie hat sich der OEE Ihrer Linie über die Zeit entwickelt?

**Inhalt der Folie:**
- Interaktiver Plotly-Chart: Monatlicher OEE-Verlauf
  - Einzelchargen als kleine Punkte im Hintergrund
  - Monatlicher Durchschnitt als blaue Linie mit Markern
  - ±1-Standardabweichungs-Band (grau/blau schattiert)
  - Rote gestrichelte Referenzlinie: Gesamtdurchschnitt
  - Orange gepunktete Linie: System-OEE aus vw_monthly_kpis (Vergleichswert)
- Legende und Achsenbeschriftung

**Sprechtext:**
> Dieses Diagramm zeigt den monatlichen OEE-Verlauf Ihrer Linie. Jeder kleine Punkt ist eine einzelne Charge. Die blaue Linie verbindet die monatlichen Durchschnittswerte — gewichtet nach Chargendauer, damit lange Chargen stärker zählen als kurze. Das blaue Band zeigt die Schwankungsbreite: In diesem Bereich liegen die meisten Chargen eines Monats. Die rote gestrichelte Linie ist der Gesamtdurchschnitt über den gesamten Zeitraum. Die orange gepunktete Linie zeigt zum Vergleich den OEE-Wert, wie ihn das System berechnet.
>
> **Frage an Sie:** Gibt es Monate, in denen etwas Besonderes passiert ist — z. B. eine Umstellung, ein Maschinenumbau oder ein Personalwechsel? Das würde mir helfen, Ausschläge besser einzuordnen.

**(~3 Minuten)**

---

## Folie 4 — OEE-Komponenten im Zeitverlauf

**Titel:** Was beeinflusst den OEE am stärksten?

**Inhalt der Folie:**
- Plotly-Chart: OEE-Komponenten über die Zeit
  - Blaue Linie: Verfügbarkeit (%)
  - Orange Linie: Leistungsgrad (%)
  - Grüne Linie: Qualität (%)
  - Rote Linie: OEE-Ist (%)
  - Einzelchargen (OEE) als dezente Punkte im Hintergrund
  - Gestrichelte rote Referenzlinie: Gesamtdurchschnitt OEE

**Sprechtext:**
> Jetzt schauen wir uns an, warum der OEE so ist, wie er ist. Der OEE setzt sich aus drei Faktoren zusammen: Verfügbarkeit — also wie viel der geplanten Zeit die Anlage tatsächlich läuft. Leistungsgrad — also ob die Anlage auf Soll-Geschwindigkeit produziert. Und Qualität — der Anteil der einwandfreien Produkte. Die rote Linie unten ist der resultierende OEE.
>
> Sie sehen hier, welche Komponente die stärkste Bremse ist. Wenn z. B. die Verfügbarkeit deutlich unter den anderen Werten liegt, wissen wir, dass Stillstände das Hauptproblem sind und nicht etwa die Geschwindigkeit oder Ausschuss.
>
> **Frage an Sie:** Deckt sich das mit Ihrer Wahrnehmung? Gibt es einen Bereich, den Sie für besonders kritisch halten?

**(~3 Minuten)**

---

## Folie 5 — Bestleistungspotenzial (BDP)

**Titel:** Wie viel Potenzial steckt noch in der Linie?

**Inhalt der Folie:**
- Plotly-Chart: Rollierendes BDP-Potenzial
  - Blaue Punkte: Einzelchargen
  - Grüne Punkte: „Golden Batches" (Chargen ≥ 90. Perzentil)
  - Blaue Linie: Monatlicher Ø OEE
  - Grüne Treppenlinie: Rollierendes BDP je Quartal (90. Perzentil)
  - Gestrichelte Referenzlinien: Gesamtdurchschnitt und Gesamt-BDP
- Kennzahlen als Text auf der Folie:
  - Ø OEE: [Wert] %
  - Ziel-OEE (Top 10 %): [Wert] %
  - Ungenutztes Potenzial: +[Wert] Prozentpunkte
  - Anzahl Golden Batches

**Sprechtext:**
> Dieser Chart beantwortet die Frage: Wie gut könnte die Linie laufen, wenn sie immer so gut produzieren würde wie in ihren besten Momenten? Dafür schaue ich mir die besten 10 Prozent aller Chargen an — die grünen Punkte. Die haben es bereits geschafft, unter denselben Bedingungen einen deutlich höheren OEE zu erreichen. Die Differenz zwischen dem Durchschnitt und diesem Bestwert ist das ungenutzte Potenzial.
>
> Die grüne Treppenlinie zeigt, wie sich dieses Bestwert-Niveau von Quartal zu Quartal verändert. So sehen wir, ob die Linie tendenziell besser wird oder ob das Potenzial gleich bleibt.
>
> **Frage an Sie:** Haben Sie eine Ahnung, was bei den grünen Chargen anders gelaufen ist? Bestimmtes Material, bestimmte Schicht, bestimmter Maschinenfahrer?

**(~3 Minuten)**

---

## Folie 6 — Materialvergleich

**Titel:** Welche Materialien laufen gut — und welche nicht?

**Inhalt der Folie:**
- Plotly-Chart mit 3 übereinander liegenden Panels:
  1. **Balkendiagramm:** Produktionsvolumen (Gesamtmenge) der Top-10-Materialien
  2. **Boxplot:** OEE-Verteilung je Material (Median, Quartile, Ausreißer) mit gestrichelter Ø-Linie
  3. **Heatmap:** OEE-Komponenten je Material (Verfügbarkeit, Leistungsgrad, Qualität) — rot = niedrig, grün = hoch

**Sprechtext:**
> Jetzt schauen wir uns an, ob das Material, das produziert wird, einen Einfluss auf den OEE hat. Oben sehen Sie die zehn am häufigsten produzierten Materialien — sortiert nach Gesamtmenge. In der Mitte zeigt der Boxplot, wie stark der OEE bei jedem Material schwankt. Manche Materialien haben eine enge Box — die laufen stabil. Andere streuen stark — da gibt es gute und schlechte Chargen.
>
> Unten in der Heatmap sehen Sie farblich, wo der OEE-Verlust bei jedem Material herkommt: Ist es die Verfügbarkeit? Der Leistungsgrad? Oder die Qualität? Grün heißt gut, rot heißt Handlungsbedarf.
>
> **Frage an Sie:** Gibt es Materialien, die Ihnen bekanntermaßen Schwierigkeiten machen? Oder wo Sie wissen, dass die Sollwerte im System nicht aktuell sind?

**(~3 Minuten)**

---

## Folie 7 — Schichtvergleich

**Titel:** Gibt es Unterschiede zwischen den Schichten?

**Inhalt der Folie:**
- **Chart 1:** Monatlicher OEE-Verlauf nach Schicht (3 farbige Linien: Früh-, Spät-, Nachtschicht)
- **Chart 2:** Zwei übereinander liegende Panels:
  1. Boxplot: OEE-Verteilung je Schicht
  2. Gestapeltes Balkendiagramm: Geplanter vs. ungeplanter Stillstand je Schicht (Minuten)

**Sprechtext:**
> Hier vergleichen wir die drei Schichten miteinander. Im oberen Diagramm sehen Sie den monatlichen OEE-Verlauf — eine Linie pro Schicht. So erkennen wir, ob eine Schicht systematisch besser oder schlechter liegt als die anderen.
>
> Im zweiten Chart zeigt der Boxplot die Gesamtverteilung je Schicht, und darunter sehen Sie die kumulierten Stillstandszeiten: blau ist geplanter Stillstand, rot ist ungeplanter Stillstand. Wenn eine Schicht deutlich mehr ungeplanten Stillstand hat, ist das ein Ansatzpunkt.
>
> **Frage an Sie:** Ist der Schichtvergleich für Sie relevant? Haben Sie den Eindruck, dass es schichtabhängige Unterschiede gibt?

**(~2 Minuten)**

---

## Folie 8 — Ungeplante Stillstände im Detail

**Titel:** Wo geht die meiste Zeit durch ungeplante Stillstände verloren?

**Inhalt der Folie:**
- Visualisierung der ungeplanten Stillstandsphasen, aufgeteilt in Subgruppen:
  - Equipment Breakdown (Maschinenausfall)
  - Changeover Time (Umrüstzeit)
  - Cleaning (Reinigung)
  - Organizational Downtime (organisatorischer Stillstand)
  - Non-Technical Breakdown (nicht-technische Ausfälle)
- Darstellung als gestapeltes Balkendiagramm oder Treemap: welche Art wie viele Minuten ausmacht
- Optional: Trend über die Zeit — nehmen bestimmte Stillstandsarten zu oder ab?

**Sprechtext:**
> Jetzt gehen wir tiefer in die ungeplanten Stillstände hinein. Bisher haben wir gesehen, wie viel ungeplanter Stillstand insgesamt anfällt. Aber nicht jeder Stillstand ist gleich — es gibt verschiedene Kategorien: Maschinenausfälle, Umrüstzeiten, Reinigung, organisatorische Ausfälle und nicht-technische Störungen.
>
> Dieser Chart zeigt, wie sich die ungeplante Stillstandszeit auf diese Kategorien verteilt. So sehen wir sofort, wo der größte Hebel liegt. Wenn z. B. Maschinenausfälle den Löwenanteil ausmachen, ist das ein anderes Thema als wenn die Umrüstzeit dominiert.
>
> **Frage an Sie:** Welche Stillstandsarten sind aus Ihrer Sicht die kritischsten? Gibt es Kategorien, bei denen Sie genauer hinschauen möchten?

**(~2 Minuten)**

---

## Folie 9 — Korrelationsanalyse (Scatterplot)

**Titel:** Hängen die Variablen zusammen?

**Inhalt der Folie:**
- Scatterplot-Matrix oder einzelne Scatterplots der wichtigsten Variablenpaare, z. B.:
  - Verfügbarkeit vs. OEE
  - Leistungsgrad vs. OEE
  - Chargendauer vs. OEE
  - Produktionsmenge vs. OEE
- Farbliche Kodierung nach Material oder Schicht (optional)
- Trendlinie / Korrelationskoeffizient, wenn sichtbar

**Sprechtext:**
> Zum Schluss der Analyse eine wichtige Frage: Hängen die verschiedenen Variablen miteinander zusammen? Dieser Scatterplot vergleicht jeweils zwei Kenngrößen. Jeder Punkt ist eine Charge. Wenn die Punkte einem klaren Muster folgen — z. B. eine Diagonale bilden — dann gibt es einen Zusammenhang.
>
> Zum Beispiel: Wenn Chargen mit hoher Verfügbarkeit auch einen hohen OEE haben, dann ist die Verfügbarkeit der entscheidende Stellhebel. Oder: Wenn längere Chargen generell einen niedrigeren OEE haben, wäre das ein Hinweis auf Ermüdungseffekte oder Maschinenverschleiß innerhalb einer Charge.
>
> **Frage an Sie:** Gibt es bestimmte Zusammenhänge, die Sie vermuten? Irgendwas, wo Sie sagen: „Das müsste doch eigentlich zusammenhängen"?

**(~2 Minuten)**

---

## Folie 10 — Ausblick & nächste Schritte

**Titel:** Wie geht es weiter?

**Inhalt der Folie:**
- Bullet-Liste der geplanten nächsten Schritte:
  - Vertiefung der Themen, die im Gespräch als besonders relevant identifiziert wurden
  - Erweiterung der Stillstandsanalyse (z. B. Ursachenzuordnung, zeitliche Muster)
  - Vergleich mit anderen Linien / Standorten, wenn gewünscht
  - Aufbau eines regelmäßigen Berichts oder Dashboards (falls Interesse besteht)
  - Rücksprache nach Aufbereitung der offenen Fragen
- Kontaktdaten / Erreichbarkeit

**Sprechtext:**
> Damit komme ich zum Ausblick. Mein Projekt läuft noch weiter, und ich möchte die Analyse dort vertiefen, wo es für Sie den größten Nutzen bringt. Deshalb ist mir Ihr Feedback heute besonders wichtig.
>
> Als nächste Schritte habe ich mir vorgenommen: Die Themen, die Sie heute als besonders interessant markiert haben, werde ich genauer analysieren und Ihnen die Ergebnisse nachliefern. Ich kann die Stillstandsanalyse weiter aufschlüsseln, z. B. nach Zeiträumen oder Ursachen. Wenn gewünscht, kann ich auch einen Vergleich mit anderen Linien oder Standorten machen. Und falls Sie Interesse haben, könnte man aus den Analysen ein regelmäßiges Reporting oder ein Dashboard ableiten.
>
> **Abschlussfrage:** Was hat Sie heute am meisten überrascht? Und welches Thema soll ich als Erstes vertiefen?

**(~2 Minuten)**

---

## Zusammenfassung der Folienstruktur

| Folie | Titel | Dauer |
|:-----:|-------|:-----:|
| 1 | Titelfolie & Vorstellung | ~1 min |
| 2 | Was wurde analysiert? | ~2 min |
| 3 | Monatlicher OEE-Verlauf | ~3 min |
| 4 | OEE-Komponenten im Zeitverlauf | ~3 min |
| 5 | Bestleistungspotenzial (BDP) | ~3 min |
| 6 | Materialvergleich | ~3 min |
| 7 | Schichtvergleich | ~2 min |
| 8 | Ungeplante Stillstände im Detail | ~2 min |
| 9 | Korrelationsanalyse (Scatterplot) | ~2 min |
| 10 | Ausblick & nächste Schritte | ~2 min |
| | **Gesamt** | **~23 min** |

> **Hinweis:** Die Zeitangaben ergeben ca. 23 Minuten, was Puffer für Zwischenfragen lässt. Wenn das Gespräch kürzer sein soll, Folien 7 (Schichtvergleich) und 9 (Scatterplot) können gekürzt oder optional gehalten werden.
