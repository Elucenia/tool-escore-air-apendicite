<!-- ELUCENIA technical documentation · escore-air-apendicite · de · no clinical/professional/rights approval -->

# AIR-Score (entzündliche Reaktion bei Appendizitis)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/escore-air-apendicite)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Erbrechen

`vomito`

### Schmerzen im rechten Unterbauch

`dor`

### Loslassschmerz oder muskuläre Abwehrspannung

`defesa`

- `0` — Nicht vorhanden
- `1` — Leicht
- `2` — Mäßig
- `3` — Stark

### Temperatur ≥ 38,5 °C

`temp`

### Neutrophile

`neut`

- `0` — \< 70%
- `1` — 70 bis 84%
- `2` — ≥ 85%

### Leukozyten

`leuco`

- `0` — \< 10.000/mm³
- `1` — 10.000 bis 14.900/mm³
- `2` — ≥ 15.000/mm³

### C-reaktives Protein

`pcr`

- `0` — \< 10 mg/L
- `1` — 10 bis 49 mg/L
- `2` — ≥ 50 mg/L

## Fassung der Methode

AIR nach Andersson (2008), mit den durch das Erratum von 2012 korrigierten Tabellen 2 und 7: sieben Komponenten, Gesamtwert 0–12, CRP in mg/L; ursprüngliche Gruppen 0–4, 5–8 und 9–12. Die 2021 vorgeschlagene Änderung des unteren Grenzwerts wurde nicht übernommen.

## Dokumentierte Formel

Erbrechen (1) + rechter Unterbauchschmerz (1) + leichte (1), mäßige (2), starke (3) Peritonealreizung + Temperatur ≥38,5 °C (1) + Neutrophile 70–84% (1) oder ≥85% (2) + Leukozyten 10.000–14.900 (1) oder ≥15.000 (2) + CRP 10–49 (1) oder ≥50 mg/L (2). Gesamt 0 bis 12.

## Grenzen und Population

Der AIR von 2008 wurde bei Personen untersucht, die wegen eines Appendizitisverdachts aufgenommen wurden; ein Teil der Kohorte blieb in der unbestimmten Gruppe und benötigte weitere Untersuchungen. Vom Originalartikel von 2008 wurde nur die Zusammenfassung gelesen. Das Erratum von 2012 wurde direkt gelesen: Seine Tabellen 2 und 7 korrigieren die CRP-Konzentrationen und dokumentieren Punkte, Einheiten und ursprüngliche Gruppen. Die numerische Prüfung beschränkt sich auf die Addition der sieben bereits ausgewählten Komponenten; sie bestätigt weder klinische Gruppen noch diagnostische, bildgebende oder chirurgische Entscheidungen. Die Überarbeitung von 2021 schlug ein niedriges Risiko bei einem Score \<4 vor, abweichend von der ursprünglichen Gruppe 0–4; diese Änderung wurde in dieser Ausgabe nicht übernommen. Mindestalter, Ausschlusskriterien und vollständiges Protokoll wurden durch das Lesen der Zusammenfassung von 2008 nicht bestätigt. Nicht beobachtete Befunde dürfen nicht als nicht vorhanden behandelt werden. Eine klinische oder sprachliche Prüfung durch unabhängige Fachleute sowie eine Genehmigung der Instrumentenrechte wurden nicht durchgeführt.

## Referenzen

- [Andersson M, Andersson RE. The appendicitis inflammatory response score: a tool for the diagnosis of acute appendicitis that outperforms the Alvarado score. World J Surg, 2008.](https://doi.org/10.1007/s00268-008-9649-y)

- [Di Saverio S et al. Diagnosis and treatment of acute appendicitis: 2020 update of the WSES Jerusalem guidelines. World J Emerg Surg, 2020.](https://doi.org/10.1186/s13017-020-00306-3)

- [Andersson M, Andersson RE. Erratum to: The Appendicitis Inflammatory Response Score: A Tool for the Diagnosis of Acute Appendicitis that Outperforms the Alvarado Score. World J Surg, 2012;36:2269–2270. Corrected Tables 2 and 7.](https://doi.org/10.1007/s00268-012-1679-9)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Geringe Wahrscheinlichkeit (0 bis 4)

Hoch mit erneuter Beurteilung, wenn die Symptome anhalten, bei einem Patienten mit gesichertem Follow-up.


### 2

Unbestimmte Wahrscheinlichkeit (5 bis 8)

Aktive Beobachtung mit klinischer und laborchemischer Neubewertung und/oder Bildgebung.


### 3

Hohe Wahrscheinlichkeit (9 bis 12)

Chirurgische Beurteilung.

