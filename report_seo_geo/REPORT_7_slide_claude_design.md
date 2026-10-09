# Report SEO & GEO per il proprietario: 7 slide (Claude Design)

**Stato:** testi concordati il 9 ottobre 2026 · consegna al proprietario: **10 ottobre 2026**
**Destinatario:** il proprietario dell'hotel (non tecnico). Il report deve essere rapido e comprensibile: dati positivi, problemi, soluzioni, cronologia, richieste. Niente servizi né costi: la parte economica si discute a voce.
**Chi fa cosa:** non va sulle slide, che riportano solo le cose da fare. All'interno: N8 fa le correzioni su WordPress, DIGIVAL solo dove serve un webmaster (vedi checklist).

> Tutto il dettaglio tecnico (URL, schema, redirect) è in `CHECKLIST_TECNICA.md`, che non va al proprietario.
> La revisione del vecchio report da 35 slide è in `REVISIONE_report_originale.md`.

---

## Come procedere in Claude Design

1. Carica il PDF del vecchio report (o 2-3 screenshot) come riferimento di stile, il logo dell'hotel in bianco e il logo N8.
2. Incolla il **prompt di stile**, poi i prompt delle slide **uno alla volta**, controllando ogni slide prima di passare alla successiva.

### Prompt di stile (una volta sola)

```
Crea una presentazione 16:9 in italiano per il proprietario di un hotel,
chiara e poco testuale. Stile ripreso dal PDF allegato: sfondo blu con
sfumatura (dal blu medio #2F63A8 al blu scuro #0D3B7E), titoli bianchi
in maiuscolo con carattere geometrico bold e spaziatura larga, box bianchi
con angoli arrotondati e testo blu #1B4A8F. Logo dell'hotel in bianco in
alto al centro solo in copertina, logo N8 piccolo in basso a destra su
tutte le slide. Molto spazio bianco, numeri grandi, frasi brevi.
Iniziamo dalla slide 1.
```

---

## Slide 1 · Copertina

File da caricare (cartella `asset/`): `drone.jpg` (foto dell'hotel dal drone con il Monte Bianco, 1920×1080, dal sito) e `logo-hotel-bianco.png` (logo del sito ricolorato in bianco, sfondo trasparente). Alternativa per lo sfondo: `montagna.jpg` (Lago d'Arpy).

```
Slide 1 – Copertina.
Sfondo a tutta pagina: la foto drone.jpg allegata (l'hotel con il Monte
Bianco dietro), con una velatura blu #0D3B7E al 55% di opacità, più
scura in basso, in modo che i testi bianchi si leggano bene.
In alto al centro: il logo logo-hotel-bianco.png, largo circa un quarto
della slide.
Al centro, titolo molto grande in bianco: SEO & GEO
Sotto, sottotitolo in bianco più piccolo:
Come farsi trovare su Google e consigliare da ChatGPT e Gemini
In basso al centro, piccolo e con spaziatura larga: OTTOBRE 2026
Logo N8 piccolo in basso a destra.
Nessun altro testo oltre a questi.
```

> Sottotitolo cambiato il 9 ott rispetto alla bozza ("Come migliorare il sito di Hotel Les Montagnards"): il proprietario non sa cosa significa GEO, e la copertina lo spiega in una riga.

## Slide 2 · Cosa funziona già

```
Sostituisci la slide 2 con questa versione.
Slide 2 – Titolo: COSA FUNZIONA GIÀ
Sfondo blu con sfumatura come da stile (niente foto).
Griglia di 8 riquadri bianchi uguali con angoli arrotondati, 4 per riga.
In ogni riquadro un numero molto grande in blu #1B4A8F e sotto una riga
di spiegazione più piccola:
- 4,8/5 — Google (301 recensioni)
- 9,4/10 — Booking (oltre 540 recensioni)
- 4,8/5 — Tripadvisor
- 11 — volte in cui ChatGPT, Gemini e Google AI nominano l'hotel
  (sotto, più piccolo: "Pagine usate come fonte: Home · Pet friendly ·
  Spa · Contatti — dati Semrush")
- +39% — visitatori da Francia e Svizzera rispetto al 2025
- 92/100 — velocità del sito su mobile
- 1 min 19 s — tempo medio sul sito di chi arriva da Google (+29%
  rispetto al 2025)
- 89/100 — quanto il sito è leggibile dalle intelligenze artificiali
  (Semrush)
Sotto la griglia, una fascia bianca larga quanto la griglia con due
righe, ognuna con una piccola icona a sinistra:
- "Hotel Morgex" è la ricerca che rende di più: un contatto costa circa
  un terzo rispetto alle altre ricerche.
- I clienti premiano: l'accoglienza dei cani · la colazione con torte
  fatte in casa · la posizione · e ora c'è la nuova Spa Alpina.
Logo N8 piccolo in basso a destra. Nessun altro testo.
```

> **Tolto di proposito:** "13.622 € di prenotazioni online (lug–set 2026)". È il valore delle prenotazioni Beddy registrate da GA4 (slide 5 del vecchio report): lordo, senza cancellazioni, e senza chi rifiuta i cookie. Non è verificato e forse nemmeno il proprietario lo conosce. Diventa un'azione del piano (confronto GA4 / Beddy).

## Slide 2b · Google Ads (dopo la slide 2)

> Aggiunta il 9 ott 2026. Dati Google Ads lug–set 2026, verificati azione per azione: le "chiamate" sono **richieste di chiamata** (tocchi sul tasto o sul numero), non telefonate verificate. Le telefonate vere senza risposta vengono dal dettaglio chiamate (call_view, 2026).

```
Aggiungi una nuova slide subito dopo la slide 2.
Titolo: GOOGLE ADS · LUGLIO–SETTEMBRE 2026
Sfondo blu con sfumatura come da stile (niente foto).
In alto 3 riquadri bianchi grandi, uguali, con un numero molto grande e
una riga sotto:
- 153 — richieste di chiamata (tocchi sul tasto "Chiama" e sul numero)
- 177 — chat WhatsApp aperte
- 2 — prenotazioni online
Sotto, una fascia bianca con tre numeri più piccoli affiancati:
- 1.370 € — spesa in tre mesi (456 € al mese)
- circa 4 € — costo per contatto
- 2–3 prenotazioni — bastano a ripagare tre mesi di pubblicità
In fondo un riquadro bianco con bordo rosso:
"1 persona su 3 che chiama dagli annunci non riesce a parlare con
l'hotel (41 su 117 nel 2026). Ogni chiamata persa è un cliente che può
finire su Booking."
Nota piccola in basso: "Contatti registrati da Google Ads: persone
arrivate tramite gli annunci."
Logo N8 piccolo in basso a destra. Nessun altro testo.
```

**Cosa dire:** "La pubblicità i contatti li porta: più di 300 in tre mesi, a circa 4 € l'uno. Il punto debole è rispondere: circa 1 persona su 3 che chiama non riesce a parlarvi, soprattutto a metà mattina e nel pomeriggio."
> **Verificato il 9 ott:** 55 chiamate perse su 138 nel 2026 (40%), ma raggruppando i tentativi ravvicinati della stessa persona (entro 30 minuti) sono **41 persone su 117 (35%)**. È stabile tra 32% e 36% in tutti i periodi e con finestre da 10 a 60 minuti. **Non dire "4 su 10".** Soluzioni, se chiede:
- deviare le chiamate su un cellulare;
- negli orari scoperti, mostrare negli annunci WhatsApp al posto del tasto "Chiama".

## (Slide "Visite da Google": tolta)

> Tolta il 9 ott 2026 su richiesta di Nicolò: il dato "479 visite, -63%" in una slide di risultati fa una brutta figura. I due dati organici positivi vanno nella slide 2:
> - **1 min 19 s:** tempo medio di chi arriva da Google, +29% sul 2025;
> - **89/100:** sito leggibile dalle AI (Semrush).
>
> **Prompt per la slide 2:** "Nella slide 2 passa da 6 a 8 riquadri (4 per riga) e aggiungi: '1 min 19 s — tempo medio sul sito di chi arriva da Google (+29% rispetto al 2025)' e '89/100 — quanto il sito è leggibile dalle intelligenze artificiali (Semrush)'. Mantieni lo stesso stile e non cambiare gli altri sei."
>
> **Il -63%** (479 visite organiche lug–set 2026 contro 1.287 nel 2025, GA4) resta solo nelle note, da usare se il proprietario chiede. Risposta: "Il calo coincide con il nuovo sito di ottobre 2025, che ha perso i vecchi indirizzi. È la prima cosa che sistemiamo."

## Slide 3 · I problemi in breve

```
Slide 3 – Titolo: I PROBLEMI IN BREVE
Sfondo blu con sfumatura come da stile (niente foto).
8 riquadri bianchi numerati, su due colonne da 4, tutti della stessa
dimensione. In ogni riquadro: numero grande a sinistra, problema in
grassetto, sotto una sola riga di spiegazione, e in alto a destra
un'etichetta colorata con la scadenza:
- rossa "SUBITO" per i problemi 1, 2, 3
- arancione "ENTRO UN MESE" per i problemi 4, 5, 6, 7
- blu chiaro "OGNI MESE" per il problema 8

1. I vecchi indirizzi non portano alle nuove pagine
   Con il nuovo sito le pagine hanno cambiato indirizzo, ma i vecchi
   indirizzi non sono stati collegati ai nuovi: 108 portano a "pagina
   non trovata", e chi arriva da Google o da altri siti trova la porta
   chiusa.
2. Il telefono nel menu è sbagliato
   Da cellulare si chiama un numero inesistente. Ed è il canale con cui
   arrivano più prenotazioni.
3. Manca Google Search Console
   Non sappiamo per quali ricerche comparite né quali pagine hanno errori.
4. Francese e inglese dicono cose false
   "Spa gratuita con hammam"; alcuni testi sono rimasti in italiano.
5. Le pagine si contraddicono
   Home e Contatti, lette dalle AI, danno due orari di check-in; il garage
   risulta gratuito ma è a pagamento.
6. Le schede esterne non sono aggiornate
   Il portale della Regione non cita cani né Spa; Travelocity indica
   un ristorante che non c'è.
7. La carta d'identità digitale del sito è sbagliata
   Nel codice letto da Google e dalle AI il sito risulta solo come
   "Bieffepi Srl", ma l'hotel non c'è: mancano nome, indirizzo, orari,
   animali ammessi e servizi.
8. Il blog è fermo e mancano le informazioni pratiche
   6 articoli brevi, nessuno nuovo da agosto 2025 e nessuno su cani,
   Spa o sci. Sul sito mancano prezzi, orari, distanze e parcheggi agli
   impianti.

Logo N8 piccolo in basso a destra. Nessun altro testo.
```

**Cosa dire:**
- **Problema 2, da far vedere dal vivo:** apri il sito dal cellulare del proprietario, poi Menu, poi tocca il numero.
- **Problema 1, in parole semplici:** "È come cambiare casa senza lasciare al postino il nuovo indirizzo: chi arriva dai vecchi link trova la porta chiusa".
- **Problema 7, da far vedere:** apri il [Test dei risultati multimediali di Google sulla home](https://search.google.com/test/rich-results?url=https%3A%2F%2Fwww.hotelmontagnards.com%2F) oppure [validator.schema.org](https://validator.schema.org/): il risultato non parla mai di un hotel, ma di "Bieffepi Srl", registrata sia come "Organization" (società generica) sia come "Person", e di un "Article" scritto da "digival". **Spiegazione semplice (il codice a barre):** "Pensi a una scatola di biscotti al supermercato. Fuori c'è la foto dei biscotti: quella è per le persone. Poi c'è il codice a barre: quello è per la cassa, che non guarda la foto e legge solo il codice. Il vostro sito è uguale: le pagine dicono chiaramente 'Hotel Les Montagnards', ma il codice a barre che leggono Google e ChatGPT dice solo 'Bieffepi Srl' e 'articolo'. Non dice hotel, né Morgex, né cani ammessi. Noi lo rifacciamo: 'Hotel Les Montagnards, 3 stelle, Morgex, cani ammessi, sauna, parcheggio, di proprietà di Bieffepi Srl'. Così quando qualcuno chiede a ChatGPT 'hotel con il cane vicino a Courmayeur', la risposta la trova già scritta da voi." Se chiede "è complicato?": "No, è un'impostazione del sito, un paio d'ore." Se chiede "cosa cambia per me?": "Le AI vi descrivono con i vostri dati, invece che con quelli di Booking o Expedia." **Bieffepi Srl è la holding proprietaria dell'hotel e resta**: va aggiunto l'hotel, con Bieffepi indicata come proprietaria. Da dire: "Bieffepi resta, è giusto che ci sia. Ma alle macchine dobbiamo presentare anche l'hotel, perché è quello che i clienti cercano."
- **Se chiede di chi è la colpa:** "Succede spesso quando si rifà un sito: si corregge in pochi giorni". Nessuna accusa a DIGIVAL.

### Prova del punto 1 (da mostrare dal vivo)
Ogni coppia mostra **com'era la pagina il 6 ottobre 2025**, tre giorni prima del nuovo sito, e **cosa si vede oggi** allo stesso indirizzo ("Non è colpa tua, è colpa nostra!").

| Pagina | Com'era il 6 ottobre 2025 | Oggi | Dove sta ora |
|---|---|---|---|
| Articolo "A due passi dal relax" | [archivio](https://web.archive.org/web/20251006005612/https://www.hotelmontagnards.com/a-due-passi-dal-relax/) | [hotelmontagnards.com/a-due-passi-dal-relax/](https://www.hotelmontagnards.com/a-due-passi-dal-relax/) | [/a-due-passi-dal-relax.html](https://www.hotelmontagnards.com/a-due-passi-dal-relax.html) |
| Camera Comfort vista Monte Bianco (EN) | [archivio](https://web.archive.org/web/20251006010251/https://www.hotelmontagnards.com/en/room_type/comfort-room-with-balcony-and-mont-blanc-view-2/) | [/en/room_type/comfort-room…](https://www.hotelmontagnards.com/en/room_type/comfort-room-with-balcony-and-mont-blanc-view-2/) | [/en/rooms/comfort-double-room-mont-blanc](https://www.hotelmontagnards.com/en/rooms/comfort-double-room-mont-blanc) |
| Lake Arpy (EN) | [archivio](https://web.archive.org/web/20251006013134/https://www.hotelmontagnards.com/en/lake-arpy/) | [/en/lake-arpy/](https://www.hotelmontagnards.com/en/lake-arpy/) | nessuna pagina equivalente |

Elenco completo: `prova_404_2026-10-09.csv`, con 108 URL ricontrollate il 9 ottobre 2026. Tutte rispondono 404, e per ognuna c'è il link alla copia d'archivio che dimostra che esisteva. Chiunque può rifare la verifica incollando la colonna `vecchia_url` su httpstatus.io.
**Composizione:**
- 24 articoli e pagine informative;
- 21 offerte e promozioni;
- 19 schede camere;
- 14 pagine stagionali;
- 11 contatti e richieste;
- 8 privacy e cookie;
- 5 categorie del blog;
- 6 altre pagine in spagnolo.

In tutto 25 delle 108 pagine sono in spagnolo, perché la versione spagnola è stata eliminata.
**Attenzione:** il -63% di visite da Google è un dato certo (GA4), ma che dipenda dalle pagine perse è la **causa più probabile**, non una prova. La conferma arriverà da Search Console.

## Slide 4 · Il piano: le tre fasi

> ✅ **Approvata da Nicolò** (9 ott 2026). Decisioni:
> - **niente etichette "chi"** (Noi/Voi): sulla slide solo cosa fare;
> - niente tasto "Chiama", niente scheda Google (è già corretta), niente account Google né conteggio delle telefonate (già tracciate in Ads);
> - **niente date** sulle fasi (le tempistiche le decide il cliente), solo l'ordine 1-2-3;
> - ogni voce dice cosa c'è oggi e cosa diventa.

```
Slide 4 – Titolo: IL PIANO IN TRE FASI
Sfondo blu con sfumatura come da stile (niente foto).
Tre colonne affiancate, da sinistra a destra, unite da una linea
orizzontale con tre punti numerati 1, 2, 3, a indicare l'ordine.
Nessuna data. In cima a ogni colonna: FASE 1 / FASE 2 / FASE 3 in grande
e sotto un sottotitolo corto. In ogni colonna un elenco di box bianchi con
angoli arrotondati. In ogni box: in grassetto la pagina o il tema, sotto
la modifica in una o due righe. Nessuna etichetta su chi fa cosa. Testo
piccolo ma leggibile, stessa larghezza per tutti i box.

FASE 1 · Le urgenze
- Telefono nel menu: correggere il link, oggi da cellulare chiama un
  numero inesistente
- Vecchi indirizzi: collegare i 108 vecchi indirizzi alle nuove pagine
- Google Search Console: installarla
- Domande dell'ultima slide: raccogliere le risposte

FASE 2 · Le pagine in italiano
- Home e Contatti: un solo orario di check-in (oggi 14–19 in Home e
  15–22 in Contatti); garage "a pagamento", non "gratuito"
- Pet friendly: correggere la descrizione per Google (oggi "cani ammessi
  fino senza limitazioni"); aggiungere massimo 2 cani, dog-sitter
  e supplemento
- Spa: aggiungere prezzo, orari, posti per turno e apertura agli esterni
- Camere: togliere "spa inclusa"; Family Junior Suite 38 m² per 4
  persone (oggi "33 m², letto king"); Superior con un solo nome
  (oggi anche "Matrimoniale Deluxe")
- Offerte: togliere la Last Minute Primavera/Estate 2026 scaduta;
  scrivere "parcheggio scoperto incluso"

FASE 3 · Francese, inglese, Google e AI
- Spa in francese e inglese: togliere "hammam" e "accesso gratuito";
  tinozze "riscaldate a legna" (oggi in inglese "a temperatura ambiente")
- Cani in francese e inglese: "senza supplemento" solo se confermato;
  Lago d'Arpy, Val Veny e Val Ferret "a pochi minuti in auto"
  (oggi "dall'hotel")
- Home in francese: descrizione per Google e titolo "Tra cime, vallate
  e borghi autentici" tradotti (oggi in italiano)
- Camere in francese e inglese: "personnes / guests" e "m²" al posto
  di "persone" e "mq"
- Dati strutturati (il "codice a barre" del sito): presentare "Hotel
  Les Montagnards" con indirizzo, servizi, animali e check-in, e Bieffepi
  Srl come proprietaria; togliere "Persona" e "Articolo"
- Schede esterne: Travelocity senza ristorante; Expedia e Hotels.com
  con il limite cani giusto; portale della Regione con cani e Spa

Logo N8 piccolo in basso a destra. Nessun altro testo.
```

**Prima di generarla:**
- **Travelocity:** controllare che dica davvero "ristorante" (dato preso da un riassunto di ricerca).

**Se è troppo piena** (14 box):
- **4 · "Il piano in tre fasi":** solo date, sottotitoli e nome di ogni box;
- **4b · "Cosa correggiamo, pagina per pagina":** tabella "Pagina · Oggi · Dopo".

**Cosa dire:** "Prima mettiamo a posto la casa, poi la facciamo crescere."

## Slide 5 · Piano Autunno

> Rinominata il 9 ott 2026 (prima era "Il piano: da novembre"). Stesse regole della slide 4: niente date, niente "chi", voci concrete. Non ripete le correzioni della slide 4: qui c'è solo il lavoro per **far crescere** il sito.

```
Slide 5 – Titolo: PIANO AUTUNNO
Sottotitolo piccolo sotto il titolo: "Dopo le correzioni: far crescere il
sito prima della stagione invernale"
Sfondo blu con sfumatura come da stile (niente foto).
Tre colonne affiancate di box bianchi con angoli arrotondati, ognuna con
un titolo in maiuscolo e una piccola icona. La colonna centrale (il blog)
è leggermente evidenziata: bordo più spesso o sfondo bianco pieno.
In ogni box: in grassetto la pagina o il tema, sotto una o due righe.
Nessuna data, nessuna etichetta su chi fa cosa.

PAGINE PIÙ COMPLETE
- Courmayeur e La Thuile: distanze in km e minuti (10 e 20 minuti in
  auto), dove si parcheggia agli impianti, niente skibus: si va in auto
- Pet friendly: passeggiate con il cane dall'hotel e a pochi minuti in
  auto, veterinario più vicino, domande frequenti
- Spa: cosa include, come si prenota, cosa portare, massaggi, domande
  frequenti
- Morgex: cosa fare in paese, il Blanc de Morgex, lo sci di fondo
  ad Arpy

IL BLOG: UN ARTICOLO AL MESE
- Perché: ogni articolo risponde a una domanda che i clienti fanno
  a Google, ChatGPT e Gemini
- Si parte da: "Sciare a Courmayeur e La Thuile dormendo a Morgex"
- Poi: "In vacanza con il cane a Morgex"
- Poi: "Weekend romantico tra Spa e Monte Bianco"
- Tutti i titoli nella slide successiva

OGNI MESE, COSA MISURIAMO
- ChatGPT e Gemini: quante volte consigliano l'hotel su 20 domande fisse
- Chiamate e WhatsApp: oggi circa 50 richieste di chiamata e 60 chat
  WhatsApp al mese (media luglio–settembre 2026), da far crescere
- Primo bilancio insieme: confronto con il punto di partenza

Logo N8 piccolo in basso a destra. Nessun altro testo.
```

**Numeri di partenza** (Google Ads, 9 ott 2026):

| Conversione | Luglio | Agosto | Settembre |
|---|---|---|---|
| Chiamate Organiche | 37,3 | 39,0 | 26 |
| Chiamate da ADS | 19 | 20 | 12 |
| Whatsapp Organico | 81 | 48 | 18 |
| MSG WhatsApp da ADS | 0 | 10 | 20 |
| Acquisto | 0 | 0 | 2 (766 €) |

Richieste di chiamata 153 in tutto, circa 51 al mese; clic WhatsApp 177, circa 59 al mese. ⚠️ Le due azioni "chiamate" contano i **tocchi sul tasto o sul numero**, non telefonate verificate: le telefonate vere sono solo nel dettaglio chiamate (call_view) e il 40% resta senza risposta.
- **Prenotazioni online escluse** dalla slide: Ads ne vede 2, mentre GA4 riporta 13.622 € (lug–set). Da confrontare prima con Beddy.
- **Da sapere:** Ads registra solo i contatti che riesce a collegare a una pubblicità, e le "Chiamate da ADS" partono dagli annunci, non dal sito.
- **Calo a settembre:** WhatsApp da 81 a 38 e telefonate da 56 a 38. Probabilmente è stagionalità.
- **"Visite da Google" tolta:** Nicolò le misura già.

**Cosa dire:** "Con la slide 4 mettiamo a posto la casa. Questa è la parte che porta clienti nuovi, e va fatta prima che inizi la stagione sciistica."

## Slide 6 · Il blog: 12 articoli

> Versione del 9 ott 2026:
> - **niente mesi:** gli articoli sono raggruppati per stagione, le tempistiche le decide il cliente;
> - **tolti i doppioni** con pagine che esistono già: "Rafting" (/esperienze/rafting) e "Terme di Pré-Saint-Didier" (/esperienze/terme-*), sostituiti con "Valdigne con i bambini" e "Cosa fare quando piove";
> - **l'ordine dell'inverno** è lo stesso della slide 5.

```
Slide 6 – Titolo: IL BLOG · 12 ARTICOLI, UNO AL MESE
Sfondo blu con sfumatura come da stile (niente foto).
Quattro colonne affiancate, una per stagione, con il nome della stagione
in maiuscolo in cima e una piccola icona (fiocco di neve, fiore, sole,
foglia). In ogni colonna 3 box bianchi con angoli arrotondati, uno per
articolo, con il titolo dell'articolo in grassetto. Nessuna data.
In basso, una riga piccola: "Ogni articolo esce prima della stagione a
cui serve e risponde a una domanda che i clienti fanno a Google, ChatGPT
e Gemini."

INVERNO
- Sciare a Courmayeur e La Thuile dormendo a Morgex
- In vacanza con il cane a Morgex: passeggiate, regole e servizi
- Weekend romantico vicino a Courmayeur: due notti tra Spa e Monte Bianco

PRIMAVERA
- Skyway Monte Bianco con il cane: regole e consigli
- Dove dormire tra Courmayeur e La Thuile: perché scegliere Morgex
- Cosa fare in Valdigne quando piove

ESTATE
- Da Morgex al Lago d'Arpy: percorso, tempi e consigli
- 5 passeggiate facili con il cane vicino a Morgex
- Valdigne con i bambini: cosa fare partendo da Morgex

AUTUNNO
- Autunno a Morgex: vendemmia, larici e silenzio
- Dove mangiare a Morgex e in Valdigne
- Cosa fare a Morgex in inverno senza sciare

Logo N8 piccolo in basso a destra. Nessun altro testo.
```

**Perché questi 12:**
- **3 sul cane:** è il primo motivo per cui i clienti vi scelgono.
- **1 sulla Spa, il weekend romantico:** è la novità, e ancora non ha recensioni.
- **1 sullo sci senza skibus:** è la domanda pratica di chi viene d'inverno.
- **1 sui ristoranti:** l'hotel non ha ristorante, e chi dorme lì se lo chiede.
- **Gli altri:** domande frequenti di chi pianifica un viaggio.

**Cosa dire:** "Ogni articolo è una domanda in più a cui rispondete voi, invece di Booking o di un altro sito."

**Nota interna:** gli articoli sul cane e quello sullo sci conviene tradurli anche in francese, per il mercato svizzero e francese, quando c'è tempo.

## Slide 7 · Cosa ci serve da voi

> Versione del 9 ott 2026:
> - **tolti** account Google, scheda Google e prezzi su Google (già a posto);
> - **aggiunte** distanze d'inverno e parcheggi agli impianti (servono per la slide 5) e la domanda su chi aggiorna il portale della Regione;
> - **un solo accesso OTA:** Expedia Partner Central gestisce anche Hotels.com e Travelocity.

```
Slide 7 – Titolo: COSA CI SERVE DA VOI
Sfondo blu con sfumatura come da stile (niente foto).
Due box bianchi affiancati con angoli arrotondati, il sinistro più largo.
In ogni box un titolo in maiuscolo e un elenco puntato: in grassetto il
tema, poi la domanda. Testo leggibile, molto spazio tra le voci.

Box 1 – DA CONFERMARE
- Check-in: 14–19 o 15–22? Si può arrivare più tardi?
- Cani: c'è un limite di peso o di taglia? (Expedia e Hotels.com
  scrivono "fino a 10 kg") C'è un supplemento? Quanto costa il
  dog-sitter? Fornite cuccia e ciotole?
- Garage coperto: quanto costa? È incluso nelle offerte? Chi ricarica
  l'auto elettrica (la colonnina è nel garage) paga il garage?
- Spa: i 35 € l'ora sono a persona o per il gruppo? Orari? Quante
  persone per turno? Possiamo scrivere che è aperta anche a chi non
  dorme in hotel?
- Colazione: in che orari?
- Sci: d'inverno quanto ci vuole davvero per Courmayeur e La Thuile?
  Dove consigliate di parcheggiare agli impianti?

Box 2 – ACCESSI E CONTATTI
- Expedia Partner Central (gestisce anche Hotels.com e Travelocity):
  per correggere le schede
- Report delle prenotazioni da Beddy: per sapere quante prenotazioni
  arrivano dal sito
- Portale della Regione (lovevda): chi aggiorna la vostra scheda?

Logo N8 piccolo in basso a destra. Nessun altro testo.
```

**Cosa dire:** "Con queste risposte partiamo con la Fase 2. Finché non le abbiamo, sul sito non scriviamo nulla che non sia sicuro."

**Domanda da fare a voce** (non sulla slide): "Nel contratto con DIGIVAL era prevista la migrazione SEO, cioè il passaggio degli indirizzi dal vecchio al nuovo sito?" Se sì, i 108 redirect spettano a DIGIVAL senza costi; se no, sono un lavoro nuovo (vedi `PREVENTIVO_proposta.md`).

**File collegati:**
- `DATI_GOOGLE_ADS_ott2026.md`: tutti i numeri Ads, le chiamate perse, cosa non mostrare;
- `PREVENTIVO_proposta.md`: proposta economica interna.

## Note per la presentazione

- **Slide 2, riquadro "11":** le 4 pagine citate (Home, Pet friendly, Spa, Contatti) sono confermate da Nicolò in Semrush (9 ott). Da dire: Home e Contatti sono entrambe lette dalle AI e danno **due orari di check-in diversi** (14–19 e 15–22). È l'esempio concreto per il problema 5 della slide 3.

- **Slide 2:** i 92/100 (Lighthouse mobile), il 4,8 di Tripadvisor e le 11 menzioni (Semrush) vengono dal vecchio report e non li ho ricontrollati. Il +39% è calcolato da GA4: Francia da 84 a 117 utenti, Svizzera da 69 a 96, luglio–settembre. Il "un terzo" viene dall'analisi Google Ads: cluster Morgex circa 5 € a contatto contro circa 16 € del resto, quindi è un **rapporto**, non un valore assoluto (il segnale di conversione era inquinato).
- **Slide 3, punto 1:** il -63% confronta luglio–settembre 2025 (vecchio sito) con luglio–settembre 2026 (sito nuovo, online da ottobre 2025). La causa più probabile sono le vecchie pagine perse: 108 su 128 vecchi indirizzi trovati su Wayback Machine danno 404 (verificato il 9 ottobre 2026). Search Console servirà a confermarlo.
- **Slide 4, "chi":** il tasto "Chiama" è assegnato a DIGIVAL; se si riesce a farlo da Oxygen, diventa "Noi".
- **Carta d'identità:** non è nel deck. Si consegna come allegato dopo le risposte della slide 7 (`CARTA_IDENTITA_HOTEL.md`).
