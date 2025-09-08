# Notazione GDR Solitari
**Uno standard per registrare il gioco in solitaria - versione 1.6**

## 1. Introduzione  

Il gioco di ruolo in solitaria produce spesso storie ricche, ma registrarle può risultare caotico.  
Questo sistema di notazione fornisce un **metodo abbreviato** per catturare gli elementi essenziali del gioco, lasciando spazio opzionale a narrativa, dialoghi e tracciamento della campagna.  

La notazione è progettata per essere:  
- **Flessibile** — utilizzabile con sistemi diversi.  
- **Stratificata** — funziona sia come appunto rapido che come narrativa estesa.  
- **Ricercabile** — tag e codici rendono semplice tracciare PNG, eventi e luoghi.  

## 1.1 Come usare questa notazione  

Questo SRD è pensato come una **cassetta degli attrezzi, non come una prescrizione**.  
Il sistema è completamente modulare: usa solo le parti utili per i tuoi appunti e ignora il resto.  

Al centro ci sono i **Simboli** (vedi Sezione 7: Legenda Notazione GDR in Solitaria).  
Essi definiscono il linguaggio minimo del gioco:  
- `>` per le azioni del giocatore  
- `?` per le domande all’oracolo  
- `d:` per i tiri di meccanica  
- `->` per i risultati dell’oracolo  
- `=>` per le conseguenze  

Tutto il resto in questo SRD (scene, intestazioni di campagna, intestazioni di sessione, fili narrativi, orologi, estratti narrativi) **sono strati opzionali**.  
Puoi aggiungerli se vuoi tenere traccia di campagne lunghe, organizzare il tuo log o condividere resoconti di gioco, ma non sono **necessari per giocare**.  

Pensalo come cerchi concentrici:  
- **Nucleo:** Simboli (Sezione 7)  
- **Strati Opzionali:** Struttura delle scene, Frontespizio, Intestazioni di sessione, Elementi persistenti, Tracciamento progressi, ecc.  

Inizia in piccolo e aggiungi solo ciò che ti aiuta a mantenere appunti chiari e piacevoli.  

## 2. Frontespizio  

Usa questo blocco all’inizio del diario di campagna per registrare i dettagli essenziali.  

### Intestazione di Campagna  

```

\=== Diario di Campagna: Titolo Campagna ===
\[Titolo]       Titolo della campagna
\[Regolamento]  Regolamento e strumenti usati
\[Genere]
\[Giocatore]
\[PG]
\[Data Inizio]  aaaa-mm-gg
\[Ultimo Agg.]  aaaa-mm-gg

```

### Campi Opzionali  
- **[Strumenti]** — Oracoli, generatori, house rule usati  
- **[Temi]** — Mistero, romanticismo, orrore cosmico…  
- **[Tono]** — Crudo, leggero, surreale, ecc.  
- **[Note]** — Qualsiasi preparazione o aspettativa prima del gioco  

### Esempio  

```

\=== Diario di Campagna: Star Hauler ===
\[Titolo]       Star Hauler
\[Regolamento]  Loner Space
\[Genere]       Commercio spaziale / avventura fantascientifica
\[Giocatore]    Roberto
\[PG]           Capitano Elara (PG\:Elara|Nave: Rustwing)
\[Data Inizio]  2025-09-03
\[Ultimo Agg.]  2025-09-03
\[Strumenti]    Oracoli: Mythic, Tabelle PNG Stars Without Number
\[Temi]         Commercio, esplorazione, dilemmi morali
\[Tono]         Avventuroso con tinte oscure
\[Note]         Si inizia dalla Stazione Argus, il giorno dopo lo sciopero dei carichi.

```

## 3. Intestazione di Sessione  

Usa un breve blocco all’inizio di ogni sessione per mantenere ordine.  

### Intestazione Base di Sessione  

```

\=== Sessione 1 ===
\[Data]        2025-09-03
\[Durata]      90 minuti
\[Scena Iniz.] S1

```

### Campi Opzionali  
- **[Riepilogo]** — Breve nota sugli eventi precedenti  
- **[Obiettivi]** — Attese del giocatore per questa sessione  
- **[Note]** — Condizioni al tavolo, varianti, atmosfera  

### Esempio  

```

\=== Sessione 2 ===
\[Data]        2025-09-10
\[Durata]      2h
\[Scena Iniz.] S8
\[Riepilogo]   Jonah è stato catturato al faro. Complotto dei cultisti a 3/6.
\[Obiettivi]   Salvare Jonah, seguire l’indizio dal diario.
\[Note]        In prova nuova tabella di reazione PNG.

```

### Posizionamento dei Confini  

- Inserisci il **Frontespizio** una sola volta, all’inizio del diario di campagna.  
- Inizia ogni sessione di gioco con un’**Intestazione di Sessione**.  
- Termina ogni sessione con:  

```
\=== Sessione X Fine ===
```

- Aggiorna `[Ultimo Agg.]` nel Frontespizio ogni volta che aggiungi una nuova Intestazione di Sessione.  

## 4. Diario delle Scene  

### 4.1 Scene  

Le scene sono l’unità base di gioco.  

```

\[S#] *Contesto / Inquadratura*

```

- `S#` = scena numerata (`[S1]`, `[S2]`, …).  
- Contesto = breve descrizione (*faro abbandonato, mezzanotte*).  
- Usa lettere per flashback o diramazioni: `[S3a]`.  
- Usa ID di fili narrativi per trame parallele: `[T2-S5]`.  
- Marcatori temporali opzionali: `Giorno 3`, `Mezzanotte`.  

### 4.2 Azioni  

Due tipi di incertezza guidano il gioco:  

- **Azioni del giocatore (meccaniche)**  

```
> Forzare la serratura
```

- **Domande al mondo / GM (oracolo)**  

```
? C’è qualcuno dentro?
```

### 4.3 Risoluzioni  

#### Meccaniche  

```
d: \[tiro o regola] => esito
```
Esempio:  

`d: d20+Scassinare=17 vs CD 15 => Successo`  

#### Oracolo  

```
-> \[risposta] (tiro se rilevante)
```

Esempio: `-> Sì, ma… (d6=4)`  

**Convenzione abbreviata**:  
- Usa `>` o `<` per confronti (es. `d:2<4` = fallimento, `d:5>3` = successo).  
- Aggiungi `S` o `F` se serve: `d:2<4 F`.  

### 4.4 Conseguenze  

Annota il risultato narrativo dopo i tiri:  

```
\=> La porta si apre cigolando, ma il rumore riecheggia nella sala.
```

### 4.5 Elementi Persistenti  

Traccia elementi in corso con tag.  

- **PNG**: `[N:Jonah|amichevole|ferito]` → più tardi `[N:Jonah|catturato]`  
- **Luoghi**: `[L:Faro|in rovina|tempestoso]`  
- **Eventi e Orologi**: `[E:ComplottoCultisti 2/6]`  
- **Fili narrativi**: `[Thread: Trovare la sorella di Jonah | Aperto]` → `[Thread:…|Chiuso]`  
- **Personaggio Giocante**: `[PG:Nome|PF 6|Stress 2|Equip:Daga]` → `[PG:PF-1]`  

Riusa gli ID nelle scene successive per collegare il diario: `[#N:Jonah]`, `[#L:Faro]`, `[#E:ComplottoCultisti]`.  

### 4.6 Tracciamento Progressi  

Forme diverse di progresso possono essere tracciate in modo coerente:  

- **Orologi** (riempi): `[Clock:Rituale 5/12]`  
- **Tracciati** (barre di avanzamento): `[Track:Fuga 3/8]`  
- **Timer** (conto alla rovescia): `[Timer:Alba 2]`  

### 4.7 Tabelle Casuali  

Quando usi tabelle di ispirazione o generatori, annota il tiro:  

- **Tabella semplice**: `tbl: d100=42 => "Una spada spezzata"`  

- **Generatore complesso**: `gen: Evento Mythic d100=78 + 11 => Azione PNG / Tradire`  

### 4.8 Estratti Narrativi (Opzionale)  

Puoi aggiungere narrativa o dialoghi dove serve.  

- **Prosa inline**:  
  `=> La stanza puzza di muffa.`  

- **Dialogo**:  

```
N (Guardia): "Chi va là?"
PG: "Stai calmo…"
```

- **Blocco lungo**:  

```
-----------------------------------------

Il diario dice:
"Le maree non obbediscono più alla luna."
-----------------------------------------
```

Questo è opzionale — l’abbreviazione basta da sola.  

### 4.9 Note Meta  

Usa parentesi per promemoria, riflessioni o house rule.  

```
(nota: test regola furtività alternativa)
```

## 5. Esempi  

### Esempio 1 — Diario Ibrido  

```
\[S7] *Vicolo buio dietro la taverna, Mezzanotte*

> Passare furtivo oltre le guardie
> d: Furtività d6=2 vs CD 4 => Fallimento
> \=> Colpisco un barile col piede. \[E\:OrologioAllerta 2/6]

? Mi vedono?
-> No, ma… (d6=3)
\=> Distratti, ma una guardia rimane. \[N\:Guardia|vigile]

N (Guardia): "Chi va là?"
PG: "Stai calmo… solo stai calmo."
```

### Esempio 2 — Solo Abbreviazione  

```
S7 >Furtività d:2<4 F => rumore \[E\:Allerta 2/6] ?Visto? ->Nm3 => distratti, 1 resta
```

### Esempio 3 — Tracciamento Fili Narrativi  

```
\[S12] *Dentro il faro*

> Cercare nella camera
> d: Investigazione d6=5 vs CD 4 => Successo
> \=> Trovo un diario nascosto. \[E\:ComplottoCultisti 3/6] \[Thread: Trovare la sorella di Jonah|Aperto]

tbl: d100=42 => "Una spada spezzata"
```

### Esempio 4 — Diario Completo di Campagna  

```

\=== Diario di Campagna: Mistero di Clearview ===
\[Titolo]       Mistero di Clearview
\[Regolamento]  Loner + Oracolo Mythic
\[Genere]       Mistero adolescenziale / soprannaturale
\[Giocatore]    Roberto
\[PG]           Alex (PG\:Alex|PF 8|Stress 0|Equip: Torcia, Quaderno)
\[Data Inizio]  2025-09-03
\[Ultimo Agg.]  2025-09-10
\[Strumenti]    Oracoli: Mythic, Tabelle Eventi Casuali
\[Temi]         Amicizia, coraggio, segreti
\[Tono]         Inquietante ma giocoso
\[Note]         Ispirato a serie misteriose anni ’80

\=== Sessione 1 ===
\[Data]        2025-09-03
\[Durata]      1h30
\[Scena Iniz.] S1
\[Obiettivi]   Introdurre Alex, impostare primo indizio

\[S1] *Biblioteca scolastica di notte*

> Intrufolarsi per controllare gli archivi
> d: Furtività d6=5 vs CD 4 => Successo
> \=> Entro senza essere notato. \[L\:Biblioteca|buia|silenziosa]

? C’è un indizio strano in attesa?
-> Sì (d6=6)
\=> Trovo una pagina strappata di diario sul faro. \[E\:IndizioFaro 1/6]

\[S2] *Fuori dalla biblioteca, corridoio vuoto*
? Sento passi?
-> Sì, ma… (d6=4)
\=> Si avvicina un bidello, ma non mi nota ancora. \[N\:Bidello|stanco|sospettoso]

N (Bidello): "Credevo di aver sentito qualcosa…"
PG (Alex, sussurra): "Meglio filarsela."

\=== Sessione 1 Fine ===

\=== Sessione 2 ===
\[Data]        2025-09-10
\[Durata]      2h
\[Scena Iniz.] S3
\[Riepilogo]   Trovata pagina di diario che accenna al faro. Quasi scoperto in biblioteca.
\[Obiettivi]   Indagare il faro, evitare sospetti.

\[S3] *Sentiero verso il vecchio faro, Giorno 2*

> Avvicinarsi silenziosi al crepuscolo
> d: Furtività d6=2 vs CD 4 => Fallimento
> \=> Calpesto vetri rotti, forte rumore. \[Clock\:Sospetti 1/6]

? Qualcuno risponde dall’interno?
-> No, ma… (d6=3)
\=> La luce lampeggia brevemente nella finestra della torre. \[L\:Faro|in rovina|infestato]

\[S4] *Ingresso del faro*

> Cercare segni di attività
> d: Investigazione d6=6 vs CD 4 => Successo
> \=> Trovo impronte fresche nella polvere. \[Thread: Chi usa il faro?|Aperto]

tbl: d100=42 => "Una lanterna rotta"
\=> Una lanterna incrinata giace vicino alle scale. \[E\:IndizioFaro 2/6]

PG (Alex, pensa): "Qualcuno è stato qui… di recente."
\=== Sessione 2 Fine ===

```

## 6. Appendice Micro-Riferimenti  

Un rapido riepilogo delle abbreviazioni più comuni:  

```

S1 >Forzare serratura d\:d20=17>15 => Successo => rumore cigolio
S2 ?Qualcuno dentro? ->Sì, ma… => guardia distratta
S3 >Combattere guardia d\:d6=1<4 F => PF-2 \[PG\:PF 8]
S4 ?Arriva alleato? ->No, e… => Thread "Salvataggio" Aperto
S5 >Cercare stanza d\:d6=6>4 S => trova indizio \[#indizio]
S6 tbl: d100=42 => "Una spada spezzata" \[E\:ComplottoCultisti 3/6]
S7 >Convincere Jonah d\:d20=12<14 F => Jonah arrabbiato \[N\:Jonah|ostile]
S8 ?Scade tempo? ->Sì => \[Timer\:Alba 0]
S9 >Fuga nei tunnel d\:d6=5>3 S => \[Track\:Fuga 6/8]
S10 === Sessione 1 Fine ===

```

## 7. Legenda Notazione GDR in Solitaria  

Riferimento rapido alla notazione standard per il gioco in solitaria.  

### Simboli Base  
- `[S#]` — Numero e inquadratura della scena  
- `>` — Azione del giocatore (meccanica)  
- `?` — Domanda all’oracolo (mondo / incertezza)  
- `d:` — Tiro / risultato meccanico  
- `->` — Risultato dell’oracolo  
- `=>` — Conseguenza / esito  

### Tracciamento  
- `[N:Nome|tag]` — PNG  
- `[L:Nome|tag]` — Luogo  
- `[E:Nome X/Y]` — Evento / Orologio  
- `[Thread:Nome|Aperto/Chiuso]` — Filo narrativo  
- `[PG:Nome|statistiche|equip]` — Personaggio giocante  

### Progresso  
- `[Clock:Nome X/Y]` — Orologio (riempi)  
- `[Track:Nome X/Y]` — Tracciato (avanza)  
- `[Timer:Nome X]` — Timer (conto alla rovescia)  

### Narrativa (Opzionale)  
- Inline: `=> Prosa breve`  
- Dialogo:  
```

N (Guardia): "Chi va là?"
PG: "Stai calmo…"

```
- Blocco:  
```

## Estratto di testo

```

### Meta  
- `(nota: … )` — Riflessione, promemoria, house rule  

### Riga di esempio  

```
S3 >Forzare serratura d\:d20=17>15 => Successo => rumore cigolio \[N\:Guardia|allerta]
```

## 8. Changelog  

**v1.6 – Chiarimento Modulare (2025-09-08)**  
- Aggiunta Sezione 1.1 *Come usare questa notazione* per chiarire che il sistema è modulare e plug-and-play.  
- Enfatizzato che i **Simboli in Sezione 7** costituiscono il nucleo della notazione; tutti gli altri strati (Scene, Frontespizio, Intestazioni di Sessione, Fili narrativi, Orologi, Narrativa, ecc.) sono opzionali.  
- Chiarito il linguaggio sull’uso facoltativo dei confini di campagna/sessione.  

**v1.5 – Standardizzazione ASCII (2025-09-08)**  
- Sostituiti tutti i caratteri speciali (▶, 🎲, ⤷, ⇒, ecc.) con equivalenti solo ASCII (`>`, `d:`, `->`, `=>`).  
- Standardizzata la notazione per tabelle e generatori (`tbl:` e `gen:`).  
- Aggiornati tutti gli esempi, Micro-Riferimento e Legenda per riflettere lo stile solo ASCII.  

**v1.4 – Revisione di Consistenza (2025-09-03)**  
- Numerate le sezioni principali per chiarezza.  
- Standardizzati i marcatori di fine sessione come `=== Sessione X Fine ===`.  
- Chiarita la sintassi abbreviata per i confronti (`d:2<4 F`).  
- Uniformato lo stile dei dialoghi (`N:` / `PG:`).  
- Racchiuso l’Esempio Completo in blocco di codice.  
- Rimossa sezione Confini ridondante (consolidata sotto Intestazione di Sessione).  

**v1.3 – Struttura e Confini (2025-09-01)**  
- Eliminata duplicazione di confini campagna/sessione.  
- Definito il posizionamento di Frontespizio, Intestazioni di Sessione e marcatori di fine sessione in un unico punto.  

**v1.2 – Esempi Estesi (2025-08-28)**  
- Aggiunto un esempio completo di campagna (due sessioni, più scene).  
- Migliorata la chiarezza sui marcatori temporali e aggiornamenti degli elementi persistenti.  

**v1.1 – Espansione Funzionalità (2025-08-23)**  
- Aggiunto Frontespizio e Intestazione di Sessione.  
- Espanso il tracciamento persistente per PNG, luoghi, eventi, fili narrativi, PG.  
- Introdotto tracciamento progressi (Orologi, Tracciati, Timer).  
- Aggiunta notazione per Tabelle Casuali (`tbl:` / `gen:`).  
- Inclusi Estratti Narrativi e Note Meta opzionali.  

**v1.0 – Bozza Iniziale (2025-08-15)**  
- Notazione abbreviata di base per i diari di gioco in solitaria.  
- Simboli per azioni, oracoli, meccaniche e conseguenze.  
- Primi esempi e legenda.  

## 9. Crediti & Licenza  

Questa notazione è ispirata al [Valley Standard](https://alfredvalley.itch.io/the-valley-standard).  

Quest’opera è distribuita con licenza Creative Commons Attribution-ShareAlike 4.0 International.  
Per consultare una copia della licenza, visita http://creativecommons.org/licenses/by-sa/4.0/  
oppure invia una lettera a Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
