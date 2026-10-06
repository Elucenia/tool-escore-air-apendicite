<!-- ELUCENIA technical documentation · escore-air-apendicite · it · no clinical/professional/rights approval -->

# Punteggio AIR (risposta infiammatoria nell’appendicite)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/escore-air-apendicite)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Vomito

`vomito`

### Dolore in fossa iliaca destra

`dor`

### Dolore al rilascio o difesa muscolare

`defesa`

- `0` — Assente
- `1` — Lieve
- `2` — Moderata
- `3` — Intensa

### Temperatura ≥ 38,5 °C

`temp`

### Neutrofili

`neut`

- `0` — \< 70%
- `1` — 70 a 84%
- `2` — ≥ 85%

### Leucociti

`leuco`

- `0` — \< 10.000/mm³
- `1` — 10.000 a 14.900/mm³
- `2` — ≥ 15.000/mm³

### Proteina C-reattiva

`pcr`

- `0` — \< 10 mg/L
- `1` — 10 a 49 mg/L
- `2` — ≥ 50 mg/L

## Edizione del metodo

AIR di Andersson (2008), con le Tabelle 2 e 7 corrette dall’erratum del 2012: sette componenti, totale 0–12, PCR in mg/L; gruppi originali 0–4, 5–8 e 9–12. La modifica della soglia inferiore proposta nel 2021 non è stata applicata.

## Formula documentata

Vomito (1) + dolore fossa iliaca destra (1) + irritazione peritoneale lieve (1), moderata (2), intensa (3) + temperatura ≥38,5 °C (1) + neutrofili 70–84% (1) o ≥85% (2) + leucociti 10.000–14.900 (1) o ≥15.000 (2) + PCR 10–49 (1) o ≥50 mg/L (2). Totale 0 a 12.

## Limiti e popolazione

L’AIR del 2008 è stato studiato in persone ricoverate per sospetta appendicite; parte della coorte è rimasta nel gruppo indeterminato e ha richiesto ulteriori accertamenti. Dell’articolo originale del 2008 è stato letto soltanto l’abstract. L’erratum del 2012 è stato letto direttamente: le sue Tabelle 2 e 7 correggono le concentrazioni di PCR e documentano punti, unità e gruppi originali. La verifica numerica si limita alla somma dei sette componenti già selezionati; non approva i gruppi clinici né le decisioni diagnostiche, di imaging o chirurgiche. La revisione del 2021 ha proposto un rischio basso con punteggio \<4, distinto dal gruppo originale 0–4; tale modifica non è stata applicata in questa edizione. Età minima, esclusioni e protocollo completo non sono stati confermati dalla lettura dell’abstract del 2008. I reperti non osservati non devono essere considerati assenti. Non sono state effettuate una revisione clinica o linguistica da parte di professionisti indipendenti né un’autorizzazione dei diritti dello strumento.

## Riferimenti

- [Andersson M, Andersson RE. The appendicitis inflammatory response score: a tool for the diagnosis of acute appendicitis that outperforms the Alvarado score. World J Surg, 2008.](https://doi.org/10.1007/s00268-008-9649-y)

- [Di Saverio S et al. Diagnosis and treatment of acute appendicitis: 2020 update of the WSES Jerusalem guidelines. World J Emerg Surg, 2020.](https://doi.org/10.1186/s13017-020-00306-3)

- [Andersson M, Andersson RE. Erratum to: The Appendicitis Inflammatory Response Score: A Tool for the Diagnosis of Acute Appendicitis that Outperforms the Alvarado Score. World J Surg, 2012;36:2269–2270. Corrected Tables 2 and 7.](https://doi.org/10.1007/s00268-012-1679-9)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Bassa probabilità (0 a 4)

Alta con rivalutazione se i sintomi persistono, in un paziente con follow-up garantito.


### 2

Probabilità indeterminata (5 a 8)

Osservazione attiva con rivalutazione clinica e di laboratorio e/o esame di imaging.


### 3

Alta probabilità (9 a 12)

Valutazione chirurgica.

