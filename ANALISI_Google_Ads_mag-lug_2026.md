# Hotel Les Montagnards — Analisi Google Ads
**Periodo:** 5 maggio – 2 agosto 2026 (90 giorni)
**Account:** Hotel Les Montagnards (nicolo.balzani@gmail.com)
**Analisi svolta:** agosto 2026
**Fonte dati:** export in `google ads_maggio>luglio_26/`

---

## 0. Sintesi in cinque righe

1. Una sola campagna spende: `PMax_Hotel_Summer 26`, Performance Max, 15 €/giorno.
2. Il 95,5% dei clic e il 68% del budget finiscono su inventory **non-ricerca** (display/Discover/YouTube/Maps) a 0,05 € per clic.
3. Delle 244 conversioni, **solo 83 sono un dato pulito** (chiamate dagli annunci). Il resto è inquinato da azioni che scattano anche su traffico organico.
4. Il cluster **"hotel morgex"** converte al 12% a 5 €, contro i 16 € di tutto il resto. È il motore dell'account ed è sottoalimentato.
5. Contro Booking.com la battaglia della copertura è persa in partenza (10,27% contro 72,48% di quota impressioni). La strategia è vincere le aste locali, non inseguire il volume.

---

## 1. Numeri complessivi

| Metrica | Valore |
|---|---|
| Clic | 19.259 |
| Impressioni | 260.101 |
| Costo | 1.355,45 € |
| Conversioni | 244 |
| CTR | 7,40% |
| CPC medio | 0,070 € |
| Costo/conversione | 5,56 € |
| Spesa media giornaliera | ~15,06 € |

### Andamento mensile

| Mese | Clic | Impressioni | Costo | CTR | CPC |
|---|---|---|---|---|---|
| Maggio (dal 5) | 4.490 | 72.906 | 409,57 € | 6,16% | 0,091 € |
| Giugno | 7.546 | 99.061 | 457,78 € | 7,62% | 0,061 € |
| Luglio | 6.802 | 82.054 | 456,40 € | 8,29% | 0,067 € |
| Agosto (1-2) | 421 | 6.080 | 31,71 € | 6,92% | 0,075 € |

Budget stabile, CTR in crescita costante, CPC in calo. Letti da soli sembrano ottimi — il paragrafo 2 spiega perché non lo sono.

---

## 2. Il problema strutturale: dove finiscono davvero i soldi

Confrontando i totali del report termini di ricerca con i totali di campagna:

| | Clic | Costo | Conversioni | CPC | Tasso conv. | Costo/conv. |
|---|---|---|---|---|---|---|
| **Totale campagna** | 19.259 | 1.355,45 € | 244 | 0,070 € | 1,27% | 5,56 € |
| **Rete di ricerca** | 872 (4,5%) | 433,23 € (32,0%) | 32,4 (13,3%) | 0,497 € | 3,71% | 13,38 € |
| **NON ricerca** | 18.387 (95,5%) | 922,22 € (68,0%) | 211,6 (86,7%) | 0,050 € | 1,15% | 4,36 € |

**Il CPC di 0,07 € e il CTR del 7,4% sono metriche di display, non di ricerca.** Sulla ricerca vera il CPC è 0,50 €, dieci volte tanto, ma il tasso di conversione è più che triplo.

Performance Max con budget basso tende a spostarsi dove il traffico costa meno. Il risultato è che due terzi del budget comprano 18.387 clic a 5 centesimi di dubbia qualità.

> ⚠️ **Limite noto:** PMax non consente la segmentazione per rete in interfaccia. Questa ripartizione è ricavata per differenza tra i totali dei report. Da confermare con *Insight e report → Rendimento del canale*.

---

## 3. Analisi dei termini di ricerca

2.355 termini analizzati. Raggruppati per cluster:

| Cluster | Termini | Clic | Costo | Conv. | Costo/conv. | Tasso conv. |
|---|---|---|---|---|---|---|
| **Morgex / Valdigne generico** | 93 | 66 | 40,19 € | 7,84 | **5,13 €** | **11,9%** |
| Brand (les montagnards) | 43 | 361 | 119,20 € | 7,25 | 16,44 € | 2,0% |
| Tutto il resto | 2.219 | 248 | 182,14 € | 10,79 | 16,88 € | 4,4% |

### Il cluster Morgex è il motore

`hotel morgex`, `hotel a morgex`, `morgex hotel`, `alberghi a morgex`, `b&b morgex` convertono al **12%** a **5 € l'una**. Tre volte meglio del brand e del resto, con un margine enorme.

Riceve pochissimo traffico: 66 clic in 90 giorni. Dagli Insight di campagna la categoria `hotel morgex` ha un volume di ricerca di **1.000-10.000 al mese in crescita del 10%** — un ordine di grandezza sopra tutte le altre categorie. **C'è domanda non intercettata.**

### Il brand costa caro

119,20 € per 7,25 conversioni = 16,44 € l'una, con un tasso di conversione del 2%. Si sta pagando per intercettare chi già cerca l'hotel per nome.

**Da verificare prima di decidere:** quanto traffico brand arriva già gratis dall'organico (GA4 → acquisizione, sessioni organiche con query brand). Se le persone arrivano comunque, buona parte di quei 119 € è un pedaggio. Se invece è Booking a intercettarli e portarseli via con la commissione, difendere il brand è il miglior investimento dell'account.

### Sprechi

- **200 termini non-brand con spesa e zero conversioni: 178,42 €** (250 clic)
- **96 query fuori target, non ancora escluse, con spesa e zero conversioni: 84,34 €**

---

## 4. Parole chiave escluse

**243 esclusioni** sulla campagna `PMax_Hotel_Summer 26`:
- 216 a corrispondenza esatta (quasi tutte nomi di hotel concorrenti, aggiunte una a una)
- 27 generiche

### Valutazione

L'approccio è **reattivo e non scalabile**: 216 nomi di concorrenti aggiunti a mano non chiudono il rubinetto, perché ogni mese ne compaiono di nuovi (96 già presenti e non esclusi).

### Le 27 esclusioni generiche

```
5 stelle · Località · agriturismo · alagna · all inclusive · antagnod · antey
brusson · cervinia · chamois · champoluc · champorcher · cinque stelle · cogne
cogne bellevue · crevacol · mont avic · offerte · pila · piscina · piscine
resort mont avic · rhemes · ristorante · sconti · torgnon · valtournenche
```

**Coerenti:** le località concorrenti (concentra la campagna sulla Valdigne), `5 stelle`, `cinque stelle`, `all inclusive`, `piscina`/`piscine`.

**Problematiche:**
- `offerte` e `sconti` → bloccano query ad alta intenzione tipo "offerte hotel valle d'aosta"
- `ristorante` → se l'hotel ha ristorante interno, blocca anche "hotel ristorante les montagnards" *(aggiornamento 25 set 2026: l'hotel non ha ristorante, la negativa è corretta)*

### Aggiunta agosto 2026 — negative a tema lavoro

Aggiunte 47 negative a frase su tema lavoro (curriculum, assunzioni, receptionist, cameriere, job, emploi, ecc.).

**Impatto atteso: nullo.** Verifica fatta: su 2.355 termini di ricerca, **zero** a tema lavoro. Il segmento "offerte di lavoro" negli Insight non entra dalla ricerca. È manutenzione preventiva, non ottimizzazione.

**Da non aggiungere mai:** `stelle` (blocca "hotel 3 stelle"), `lavoro` da sola (blocca "viaggio di lavoro"), `stagionale` da sola (blocca "affitto stagionale", che potrebbe essere un lead vero di lungo soggiorno).

---

## 5. Geografia

| Località | Impressioni | Quota |
|---|---|---|
| Città Metropolitana di Milano | 170.694 | 65,6% |
| Città Metropolitana di Torino | 47.662 | 18,3% |
| Genova | 26.025 | 10,0% |
| Provincia di Novara | 15.720 | 6,0% |

Targeting sui **mercati di provenienza**, non sulla Valle d'Aosta. Per un hotel di montagna è la scelta corretta.

**Aperto:** Milano si prende due terzi delle impressioni, ma non sappiamo se converta in proporzione. Serve il report geografico con costi e conversioni, non con le sole impressioni.

---

## 6. Contesto competitivo (informazioni aste)

> Copre solo la porzione ricerca della PMax, cioè il 32% della spesa.

| Concorrente | Quota impr. | Sovrapposizione | Ti supera | **Tu superi lui** | In cima alla pagina |
|---|---|---|---|---|---|
| **Tu** | **10,27%** | — | — | — | **19,15%** |
| booking.com | 72,48% | 71,71% | 71,47% | **28,53%** | 63,20% |
| trivago.it | 27,35% | 25,59% | 49,37% | **50,63%** | 15,27% |
| online-reservations.com | 14,92% | 14,75% | 42,77% | **57,23%** | 6,47% |
| airbnb.it | 12,91% | 11,26% | 43,84% | **56,16%** | 7,80% |

### Lettura

**Non è un problema di posizionamento, è un problema di presenza.** Quando sei in asta te la giochi: batti Airbnb, trivago e online-reservations più della metà delle volte, e contro Booking vinci quasi 3 aste su 10.

Il punto è che **partecipi solo al 10,27% delle aste**. Booking è al 72,48%: sette volte tanto. E compare nel 71,71% delle aste in cui compari tu, nel 63% dei casi in posizione assoluta di testa.

Questo suggerisce anche che **Booking faccia offerte sul nome dell'hotel**, il che spiegherebbe il costo elevato del cluster brand.

### Conseguenza strategica

Con 15 €/giorno la quota impressioni contro Booking **non è comprabile**. Il 10,27% non è un errore da correggere: è strutturale.

→ **Non inseguire la copertura. Vincere le aste locali di Morgex**, dove Les Montagnards è il risultato più pertinente e Booking è generalista. Su quelle query l'obiettivo è l'80-90% di quota impressioni, non il 10%.

---

## 7. Le conversioni: cosa stiamo davvero misurando

| Azione | Origine | Conv. | Valore | Tipo |
|---|---|---|---|---|
| Whatsapp Organico | Sito web | 130 | 0,00 | ⚠️ inquinata |
| Chiamate Organiche | Sito web | 120 | 0,00 | ⚠️ inquinata |
| **Chiamate da ADS \| Click-to-call** | Google | **83** | **3.320,00** | ✅ **pulita** |
| MSG WhatsApp da ADS | Google | 8 | 8,00 | ✅ pulita |
| Calls from Smart Campaign Ads | Chiamata annunci | 0 | 0,00 | legacy |
| Click to call campagne intelligenti 🔒 | Chiamata annunci | 0 | 0,00 | legacy |
| Click-to-call su Maps 🔒 | Google | 0 | 0,00 | legacy |
| Indicazioni stradali su Maps 🔒 | Google | 0 | 0,00 | legacy |
| **Acquisto** (⚠️ **Secondario**) | Sito web | **2** | **1.720,40** | ✅ **prenotazioni vere** |

Tutte **Principali** tranne `Acquisto`, che è Secondario. Totale azioni: 343.

### I quattro problemi

**1. Il tracciamento prenotazioni esiste ma è spento e forse rotto.**
L'azione `Acquisto` registra **2 prenotazioni per 1.720,40 €** — cioè **860,20 € di valore medio**, con valori dinamici passati dal booking engine. È il dato di business che serve, ma:
- è impostata su **Secondario**, quindi non conta nelle Conversioni e non guida le offerte
- ha stato **"Richiede attenzione"**
- l'obiettivo Acquisto risulta in *Configurazione errata* proprio perché ha zero azioni principali

**Perché solo 2 — spiegato dal cliente (3 ago 2026):** il percorso di prenotazione online è **tortuoso, e la maggior parte delle persone entra nel motore e poi esce per telefonare o scrivere una mail**. Le 2 conversioni sono quindi un dato corretto, non un tracciamento rotto. Lo stato "Richiede attenzione" è verosimilmente "nessuna conversione recente".

→ **Conseguenza fondamentale per tutta l'analisi:** clic sul telefono e su WhatsApp **non sono micro-conversioni**, sono il canale di vendita principale dell'hotel. Il setup delle conversioni misura la cosa giusta; il difetto è solo che ci mescola dentro il traffico organico. Ottimizzare la campagna sulle chiamate non è un ripiego: è puntare al punto in cui l'hotel incassa davvero.

ROAS sul tracciato: **1.720,40 € ÷ 1.355,45 € = 1,27x sul fatturato**, sotto la pari sul margine. Ma il numero **esclude le prenotazioni nate dalle 83 telefonate**, che non passano dal booking engine e non sono tracciate da nessuna parte.

**2. Il 73% delle conversioni viene da azioni "Organico".** `Whatsapp Organico` (130) e `Chiamate Organiche` (120) sono tracciate dal sito e scattano su qualsiasi visitatore, non solo su chi arriva dagli annunci. Essendo *Principali*, finiscono nella colonna Conversioni **e guidano lo Smart Bidding**.

→ **È il motivo per cui il CPA di 5,56 € è irrealistico.** Google si prende in parte il merito di contatti che sarebbero arrivati comunque, e ci ottimizza sopra.

**3. Scala di valori incoerente.** 40 € a chiamata è una stima ragionata del valore atteso (implica un ROAS obiettivo di 2,45x, coerente). Ma WhatsApp vale 1 € e le due azioni più voluminose valgono 0. La scala è rotta *tra* le azioni, quindi l'offerta a valore non può funzionare.

**4. Probabile doppio conteggio delle chiamate.** `Chiamate Organiche` (dal sito) e `Chiamate da ADS` (da Google) possono contare la stessa telefonata due volte a seconda di dove l'utente tocca il numero.

---

## 8. Le 83 chiamate: il vero KPI

L'unico dato ad attribuzione pubblicitaria certa. Origine "In hosting su Google": la chiamata parte dall'asset dentro l'annuncio o dalla scheda Maps, **senza nemmeno passare dal sito**. È l'intenzione più alta possibile.

| | |
|---|---|
| Costo per chiamata (tutta la spesa) | **16,33 €** |
| Costo per chiamata (sola ricerca) | 5,22 € |
| Frequenza | ~1 al giorno, 6,5 a settimana |
| Quota su tutte le chiamate tracciate | **40,9%** (83 su 203) |
| ROAS implicito col valore 40 € | 2,45x |

**Gli annunci generano il 41% di tutte le telefonate dell'hotel.** Non è un canale marginale.

### Break-even

Con margine di contribuzione di **150 €** per prenotazione diretta (due notti, nessuna commissione OTA), la campagna va in pari chiudendo il **10,9% delle chiamate**.

| Margine/prenotazione | Tasso di chiusura per andare in pari |
|---|---|
| 100 € | 16,3% |
| **150 €** | **10,9%** |
| 200 € | 8,2% |
| 250 € | 6,5% |

### Scenari (margine 150 €)

| Chiusura | Prenotazioni | Margine | Ritorno |
|---|---|---|---|
| 10% | 8,3 | 1.245 € | 0,9x |
| **20%** | **16,6** | **2.490 €** | **1,8x** |
| **30%** | **24,9** | **3.735 €** | **2,8x** |
| 40% | 33,2 | 4.980 € | 3,7x |

Sul telefono di un piccolo albergo il tasso di chiusura reale sta tipicamente tra il **25% e il 40%**. Se siamo in quella forbice, **la campagna rende tra 2,5x e 3,7x**.

> ⚠️ **Da verificare:** l'azione si chiama "Click-to-call". Se non ha una **durata minima** impostata, sta contando **tocchi sul pulsante**, non telefonate connesse. In quel caso il break-even va rifatto sul numero pulito.
> Controllo: `Obiettivi → Conversioni → Chiamate da ADS | Click-to-call` → cercare "durata minima della chiamata".

---

## 9. Insight di campagna (ultimi 7 giorni: 27 lug – 2 ago)

| | |
|---|---|
| Stato campagna | ⚠️ **Limitato dal budget** |
| Budget | 15 €/giorno |
| Punteggio di ottimizzazione | 100% |
| Conversioni (7gg) | 28,71 (**+47,92%**) |
| Costo (7gg) | 97,66 € (−3,93%) |
| **CPA attuale** | **3,40 €** |
| **CPA target** | **12,15 €** |

La campagna gira a **un quarto del CPA obiettivo ed è strozzata dal budget**. In condizioni normali è il segnale da manuale per scalare — ma non prima di aver pulito il segnale, altrimenti si comprano più conversioni fasulle.

### Segmenti di pubblico

| Segmento | Quota conversioni | **Indice** |
|---|---|---|
| Viaggi in Italia | 34,4% | **34,7x** |
| Offerte di lavoro nel settore tempo libero e accoglienza | 41,7% | **2,8x** |

**Lettura corretta:** l'indice è il dato che conta. 34,7x è un bersaglio vero; **2,8x è appena sopra il rumore**. La quota del 41,7% riflette la dimensione del segmento, non un'intenzione.

Sono segmenti **descrittivi, non causali**: Google classifica gli utenti in base a cosa navigano in giro per il web, non in base a cosa fanno sul sito.

**Verificato:** nessuna pagina "lavora con noi" sul sito. Zero query di lavoro nei termini di ricerca.
**Ipotesi residua:** i posizionamenti display girano su portali di annunci di lavoro e siti di contenuti. Sarebbe un'altra faccia del problema display, non un problema di pubblico.
**Ipotesi alternativa da verificare in reception:** lavoratori stagionali che cercano alloggio per la stagione (soggiorni lunghi, bassa stagione — potenzialmente un segmento da coltivare, non da escludere).

---

## 10. Tracciamento prenotazioni: c'è già, va fatto funzionare

**Aggiornamento 3 agosto 2026.** La posizione iniziale era che il tracciamento del booking engine non si sarebbe implementato perché troppo complesso. Poi è emerso che **esiste già ed è attivo**: l'azione `Acquisto` ha registrato 2 prenotazioni per 1.720,40 € con valori dinamici reali.

Non è quindi da costruire da zero: è **da diagnosticare e completare**, a un costo molto inferiore a quello preventivato.

### Ma il volume basso non è un problema di tag — è il percorso di prenotazione

Il cliente ha chiarito che **il processo di prenotazione online è tortuoso: la gran parte degli utenti entra nel motore e poi esce per telefonare o mandare una mail.** Il tracciamento funziona; è il funnel che perde.

**Cosa si sta perdendo:**
1. **Chi non telefona** — chi cerca la sera, gli stranieri, chi vuole solo confrontare un prezzo. Chiude e va su Booking, che ha il 72% di quota impressioni e un checkout che funziona.
2. **Le prenotazioni fuori orario** — ogni sera e ogni domenica senza qualcuno al telefono.
3. **Il traffico pagato** — si comprano clic per portarli su un percorso che li fa scappare, spesso verso l'OTA che prende la commissione.

### Come trasformarlo in un numero utilizzabile

Tracciare il **clic in uscita verso il booking engine** (evento su link in GTM/GA4, dieci minuti, nessun coinvolgimento del fornitore) e mettere in fila i due dati:

> *X persone hanno aperto il motore di prenotazione. 2 hanno completato.*

Tasso di abbandono × 860,20 € = **la cifra che l'hotel lascia sul tavolo ogni trimestre**. È l'unico modo per far pesare il problema: finché è "il booking è scomodo" non si muove niente, quando diventa "abbiamo perso N mila euro in tre mesi" si muove.

Effetto collaterale utile: dà un segnale di conversione ad alto volume, molto più sfruttabile dallo Smart Bidding delle 2 prenotazioni complete.

### Nel frattempo, assecondare il comportamento
- Numero e WhatsApp **sempre visibili**, non solo nella pagina contatti
- **Pulsante di chiamata fisso su mobile**
- WhatsApp Business con risposte rapide su disponibilità e tariffe
- Verificare la **copertura oraria**: le chiamate perse sono prenotazioni perse

### Restano da fare
1. Portare `Acquisto` da Secondario a **Principale** (affiancata alle chiamate — da sola non basta per lo Smart Bidding)
2. Verificare che l'obiettivo Acquisto (`1 di 6 campagne`) sia applicato a `PMax_Hotel_Summer 26`

### I proxy restano comunque utili

**Proxy tracciabile senza il fornitore:** il **clic in uscita verso il booking engine**. Il pulsante "Prenota" / "Verifica disponibilità" sta sul sito: si traccia con un evento su link in uscita in GTM o GA4, senza cross-domain e senza coinvolgere nessuno. È il segnale più vicino all'acquisto disponibile e si sporca molto meno di un tocco su WhatsApp.

**Controlli offline (costo zero):**
1. Riconciliazione mensile PMS/channel manager: prenotazioni dirette del mese contro spesa Google Ads del mese. Dopo 3-4 mesi si ha una correlazione utilizzabile.
2. Report per sorgente interno al booking engine (quasi tutti ne hanno uno, anche senza integrazione Google).
3. "Come ci ha trovati?" in reception e al telefono — sulle 203 chiamate è l'unica verifica disponibile.

**Conseguenza metodologica:** le decisioni si prendono sui **rapporti tra cluster**, non sui valori assoluti. Non si potrà mai dire "rende 4x", ma si può dire — e basta — che il cluster Morgex genera contatti a un quinto del costo del resto.

---

## 11. Conclusioni

### Cosa funziona
- Il cluster **hotel morgex**: 12% di conversione a 5 €, con volume di ricerca in crescita non ancora intercettato
- Le **83 chiamate**: 41% di tutte le telefonate dell'hotel, con un break-even raggiungibile
- Il **targeting geografico** sui mercati di provenienza
- La **posizione in asta** quando si partecipa (si batte tutto tranne Booking)

### Cosa non funziona
- **Il segnale di conversione è inquinato** al 73% da azioni organiche che guidano lo Smart Bidding
- **Il 68% del budget** compra clic display a 5 centesimi di qualità non verificata
- **Zero visibilità sul risultato finale** (prenotazioni) — vincolo accettato, gestito per proxy
- **La strategia di esclusione** è manuale e reattiva: 216 nomi a mano, 96 ancora scoperti
- **La quota impressioni al 10,27%** non è recuperabile con questo budget

### La tesi
> L'account produce risultati reali, ma li misura male e li alimenta peggio. Il segnale d'oro (83 chiamate ad alta intenzione) è annegato in 250 azioni organiche che sviano l'algoritmo, e il budget che dovrebbe finire sulle query locali di Morgex se ne va in clic display da 5 centesimi.

---

*Documento generato con Claude Code. Piano operativo in `PIANO_OPERATIVO.md`.*
