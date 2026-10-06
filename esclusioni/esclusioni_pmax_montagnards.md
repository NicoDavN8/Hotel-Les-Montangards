# Hotel Les Montagnards: esclusioni PMax

**Campagna:** PMax_Hotel_Summer 26
**Data analisi:** 6 ottobre 2026
**Periodo dati:** 29 settembre 2026 / 5 ottobre 2026
**Totale esclusioni preparate in questo file:** 176 (87 generiche, 61 a frase, 28 esatte). **Stato reale su Google Ads: vedi sezione "Stato live" in fondo al contesto.**

## Contesto

- Hotel: B&B-Hotel da 12 camere nel centro di Morgex, wellness con sauna, pet friendly, colazione con prodotti locali, circa 10 km dalle piste.
- Tutte le campagne Search sono in pausa: i termini di ricerca arrivano solo dalla PMax.
- Spesa sui termini di ricerca: 49,93 € su 105,52 € totali PMax (il resto va su display, YouTube, Gmail).
- 6 conversioni: 1 dal brand, 4 da termini già esclusi in precedenza.
- Circa il 90% dei termini sono nomi di altri hotel, quasi tutti con 1 o 2 impressioni.

## Problemi trovati

### 1. Esclusione [aosta] inefficace
`[aosta]` è a corrispondenza esatta, quindi blocca solo la ricerca "aosta" da sola. Ricerche come "hotel aosta 4 stelle" passano.
Non si può usare "aosta" a frase o generica perché bloccherebbe anche "valle d aosta".

**Soluzione:** esclusioni a frase nella forma `"parola aosta"`. In "valle d aosta" la parola prima di "aosta" è sempre "d", quindi non viene toccata.
Da evitare la forma `"aosta parola"`: "valle d aosta hotel" contiene "aosta hotel" e verrebbe bloccata.

### 2. Portali OTA
`[booking]`, `[airbnb]` ecc. erano a corrispondenza esatta, quindi "booking com", "booking aosta" passavano. Sostituite con esclusioni generiche.

### 3. Traffico disperso
Molto traffico da Trentino, Alto Adige, Piemonte, Lombardia, bassa valle, ricerche generiche e servizi non offerti.

## Categorie di esclusioni

| Categoria | Tipo | Esempi |
|---|---|---|
| Aosta città | Frase | "hotel aosta", "spa aosta", "ad aosta" |
| Competitor Aosta | Generica | hirondelle, cecchin, norden, borbey |
| OTA e portali | Generica | booking, trivago, airbnb, expedia, kayak, vrbo |
| Fuori zona | Generica / Frase | trentino, fassa, piemonte, torino, "alto adige" |
| Bassa e media valle | Generica / Frase | ayas, cervinia, cogne, bard, "saint vincent" |
| Servizi non offerti | Frase | "mezza pensione", "piscina", "spa privata", "sulle piste" |
| Generiche e informative | Frase / Esatta | "vicino a me", "cerca hotel", [albergo], [terme] |
| QC Terme navigazionale | Generica / Frase / Esatta | qcterme, [qc terme monte bianco] |

**Lasciati attivi volutamente:**
- Courmayeur, La Thuile, La Salle, Pré-Saint-Didier, Val Ferret, Valsavarenche
- Ricerche "dormire / hotel vicino alle terme di Pré-Saint-Didier"
- Competitor di Courmayeur, Pré-Saint-Didier e Morgex (strategia di conquista come nelle vecchie campagne Search)


## Stato live su Google Ads (letto via API il 6 ottobre 2026)

Account `4130469299`, campagna `PMax_Hotel_Summer 26`: **760 negative a livello campagna** (531 esatte, 121 a frase, 108 generiche). Elenco completo in `esclusioni/PMax_negative_live_2026-10-06.csv`.

- **97 delle 176 voci di questo file sono live.** Tutte le frasi, quasi tutte le esatte e 15 generiche.
- **79 voci NON sono live**, tutte generiche (più 7 esatte QC Terme / spa Monte Bianco / terme Courmayeur): comuni di fuori zona (andalo, moena, torino, trento, ayas, cogne-area...), competitor di Aosta (hirondelle, cecchin, norden, borbey, bondaz, mancuso...), parole corte (hb, express) e OTA minori (kayak, vrbo). Non risultano nemmeno con un altro tipo di corrispondenza: o non sono state incollate, o sono state tolte di proposito. **Da confermare.**
- **661 voci in più, non presenti in questo file**: 510 esatte (soprattutto nomi di altri hotel, dai termini di ricerca), 91 generiche, 60 a frase.
  - A frase, tema lavoro (assunzioni, curriculum, cameriere, receptionist, stipendio...), località dolomitiche e siti di annunci (indeed, linkedin, jobrapido).
  - Generiche: tipologie (agriturismo, camping, rifugio, baita, chalet, meublè, affittacamere), servizi non offerti (piscina, ristorante, mezza pensione, all inclusive, 5 stelle), località fuori zona (cortina, livigno, bormio, chamonix, sestriere, brusson, pila...), "economici", "sconti", "offerte".
- **Brand e zona:** nessuna negativa su "les montagnards" né su "morgex" in generale. Presenti solo esatte su copie di indirizzo e nomi simili ("b&b morgex", "le montagnards balme", "les rêves des montagnards appartements de charme", "via saint marc 5 11017 morgex ao"). Esatta anche `[courmayeur]`.
- Nessuna modifica registrata al 5-6 ottobre nel change history (la lettura è dello stato finale, non delle operazioni).
- Elenco condiviso collegato: solo "Località" (1 voce, da verificare). Nessun elenco condiviso di negative.

### Generiche live da ricontrollare (potenziale blocco di ricerche utili)

| Parola | Rischio |
|---|---|
| `offerte`, `sconti` | bloccano "offerte hotel valle d aosta", già segnalato nel piano (punto E) |
| `centro` | blocca "hotel centro morgex", proprio il posizionamento dell'hotel |
| `montagna`, `montana` | bloccano "hotel in montagna morgex" |
| `economici`, `economico` | bassa intenzione: ok se voluto, ma l'hotel è 3 stelle superior |
| `chalet`, `baita`, `alpin`, `walser` | ok per tipologie diverse, ma "alpin" e "walser" possono comparire in ricerche di zona |
| `saint vincent`, `nus`, `verres`, `arnad` | ok, bassa valle |
| `th` | parola cortissima, controllare cosa blocca |

## Verifica (simulazione del 6 ottobre, prima dell'inserimento)

Simulazione delle esclusioni sui 798 termini reali: ne bloccano circa 300.
Nessuna ricerca brand ("les montagnards", "hotel montagnard morgex") e nessuna ricerca generica "valle d aosta" viene bloccata.

## Da valutare prima di pubblicare

- [ ] "mezza pensione", "pensione completa", "cenone": togliere se l'hotel offre la cena
- [ ] "piscina": togliere se l'hotel ha una piscina
- [ ] hb, express: parole corte, controllare che non blocchino ricerche utili
- [ ] Verificare il contenuto dell'elenco condiviso "Località" collegato alla PMax
- [ ] Decidere se escludere anche i competitor di zona (Courmayeur, Pré-Saint-Didier, Morgex)

## Prossimi passi

- [x] Inserire le esclusioni nella PMax (parziale: 97 su 176, più 661 altre; vedi stato live)
- [ ] Decidere cosa fare delle 79 voci non inserite
- [ ] Valutare un elenco condiviso "OTA e portali" per tutte le campagne hotel
- [ ] Ricontrollare i termini di ricerca tra 2 o 3 settimane
- [ ] Valutare la riattivazione di una campagna Search brand separata, con esclusione brand sulla PMax

## Elenco completo

Da incollare in Campagna > Parole chiave escluse, una per riga.

### Generica
```
hirondelle
cecchin
express
norden
mancuso
borbey
bondaz
colombot
belle epoque
hb
mignon
bucaneve
mochettaz
booking
trivago
airbnb
expedia
hotels com
kayak
vrbo
trentino
trento
fassa
andalo
moena
corvara
marebbe
pusteria
sarentino
valmalenco
pontresina
macugnaga
valsesia
valdobbia
piemonte
torino
milano
lombardia
ceresole
piamprato
presolana
imagna
zambla
baceno
braies
solda
trafoi
olang
riscone
lutago
funes
malosco
pellizzano
coredo
marilleva
valdidentro
racines
laces
martell
karpacz
strzyżów
трявна
alvito
ayas
champoluc
gressoney
challand
cervinia
valtournenche
cogne
valnontey
lillaz
bard
donnas
fenis
fénis
chatillon
châtillon
verrayes
gaby
issime
lillianes
pontboset
brissogne
pollein
qcterme
termemontebianco
```

### Frase
```
"hotel aosta"
"albergo aosta"
"alberghi aosta"
"b&b aosta"
"spa aosta"
"ad aosta"
"booking aosta"
"centro aosta"
"maison"
"locanda"
"apartments"
"vecchio mulino"
"duca"
"alto adige"
"val casies"
"valle aurina"
"val ridanna"
"ad alba"
"pont saint martin"
"saint vincent"
"st vincent"
"gran san bernardo"
"saint rhemy"
"mezza pensione"
"pensione completa"
"all inclusive"
"cenone"
"piscina"
"spa privata"
"camera con spa"
"suite con spa"
"spa in camera"
"hotel con vasca"
"bubble room"
"sulle piste"
"adults only"
"family resort"
"animazione"
"5 stelle"
"5 star"
"vicino a me"
"vicini a me"
"near me"
"nearby"
"prenotazione hotel"
"prenotare hotel"
"sito per prenotare"
"cerca hotel"
"cerco un albergo"
"prezzi hotel"
"preventivi hotel"
"info alberghi"
"strutture alberghiere"
"hotel details"
"dove andare"
"foliage"
"borghi da visitare"
"regala"
"spa and resort"
"spa of wonders"
"qc terme monte bianco recensioni"
```

### Esatta
```
[albergo]
[b&b]
[resort]
[resort hotel]
[resort con spa]
[hotel spa]
[spa hotel]
[hôtel]
[un hotel]
[turismo]
[vacanza]
[voi]
[nh]
[terme]
[staycation]
[hotel 3 stelle]
[hotel aperti]
[settimana relax]
[settimana bianca]
[weekend romantico]
[soggiorno spa e relax]
[qc terme monte bianco]
[qc monte bianco]
[terme qc monte bianco]
[spa monte bianco]
[spa montebianco]
[spa monte bianco qc terme]
[terme courmayeur]
```
