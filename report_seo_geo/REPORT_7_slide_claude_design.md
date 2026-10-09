# Report SEO & GEO per il proprietario: 7 slide (Claude Design)

**Stato:** testi concordati il 9 ottobre 2026 · consegna al proprietario: **10 ottobre 2026**
**Destinatario:** il proprietario dell'hotel (non tecnico). Il report deve essere rapido e comprensibile: dati positivi, problemi, soluzioni, cronologia, richieste. Niente servizi né costi: la parte economica si discute a voce.
**Chi fa cosa:** **Noi** = N8 (correzioni su WordPress) · **DIGIVAL** = solo dove serve un webmaster · **Voi** = l'hotel.

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
Slide 2 – Titolo: COSA FUNZIONA GIÀ
Griglia di 6 riquadri bianchi (3 per riga), ognuno con un numero grande
e una riga di spiegazione sotto:
- 4,8/5 — Google (301 recensioni)
- 9,4/10 — Booking (oltre 540 recensioni)
- 4,8/5 — Tripadvisor
- 11 — volte in cui ChatGPT, Gemini e Google AI nominano l'hotel
  (sotto, più piccolo: "Pagine del sito usate come fonte: Home · Pet friendly ·
  Spa · Contatti — dati Semrush")
- +39% — visitatori da Francia e Svizzera rispetto al 2025
- 92/100 — velocità del sito su mobile
Sotto la griglia, una fascia bianca con due righe:
- "Hotel Morgex" è la ricerca che rende di più: un contatto costa circa
  un terzo rispetto alle altre ricerche.
- I clienti premiano: l'accoglienza dei cani · la colazione con torte
  fatte in casa · la posizione · e ora c'è la nuova Spa Alpina.
```

> **Tolto di proposito:** "13.622 € di prenotazioni online (lug–set 2026)". È il valore delle prenotazioni Beddy registrate da GA4 (slide 5 del vecchio report): lordo, senza cancellazioni, e senza chi rifiuta i cookie. Non è verificato e forse nemmeno il proprietario lo conosce. Diventa un'azione del piano (confronto GA4 / Beddy).

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
   non trovata". Visite da Google: -63% rispetto all'estate 2025.
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
8. Mancano le informazioni pratiche
   Prezzi, orari, distanze in km, parcheggi agli impianti.

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

## Slide 4 · Il piano: ottobre

```
Slide 4 – Titolo: IL PIANO · OTTOBRE
Sfondo blu con sfumatura come da stile (niente foto).
Tre colonne affiancate a forma di linea del tempo, da sinistra a destra.
In cima a ogni colonna: le date in grande e sotto un sottotitolo corto.
In ogni colonna un elenco di attività su box bianchi, una riga ciascuna,
con a destra un'etichetta colorata "chi": Noi (blu), Voi (giallo),
DIGIVAL (grigio).

12–16 OTTOBRE · Le urgenze
- Correggere il telefono nel menu — Noi
- Collegare i 108 vecchi indirizzi alle nuove pagine — Noi
- Installare Google Search Console — Noi
- Darci l'accesso all'account Google dell'hotel — Voi
- Tasto "Chiama" sul cellulare — DIGIVAL
- Rispondere alle domande dell'ultima slide — Voi

19–23 OTTOBRE · Informazioni giuste
- Carta d'identità definitiva, con le vostre risposte — Noi
- Correggere le 4 pagine lette dalle AI: Home, Pet friendly, Spa,
  Contatti — Noi
- Correggere le altre pagine: camere, garage, offerte scadute — Noi
- Contare le telefonate dal sito e confrontare le prenotazioni
  con Beddy — Noi

26 OTTOBRE – 6 NOVEMBRE · Farsi capire da Google e dalle AI
- Riscrivere le pagine in francese e inglese — Noi
- Rifare il "codice a barre" del sito: l'hotel con i suoi dati — Noi
- Aggiornare scheda Google, Booking, Expedia e portale regionale —
  Noi + Voi
- Chiedere a Beddy i vostri prezzi su Google, accanto a Booking — Voi
- Primo controllo su ChatGPT e Gemini: il punto di partenza — Noi

Logo N8 piccolo in basso a destra. Nessun altro testo.
```

**Cosa dire:**
- "Ottobre serve a mettere a posto la casa; da novembre la facciamo crescere."
- "Da voi servono solo tre cose: l'accesso all'account Google, le risposte alle domande e l'accesso a Booking ed Expedia. Il resto lo facciamo noi."

## Slide 5 · Il piano: da novembre

```
Slide 5 – Titolo: IL PIANO · DA NOVEMBRE
Linea del tempo orizzontale con 4 tappe, sotto ogni tappa un box bianco.

NOVEMBRE (prima della stagione sci)
- Pagine Courmayeur e La Thuile con distanze, parcheggi agli impianti e
  "niente skibus: si va in auto"
- Pagina Cani completa
- Articolo 1

DICEMBRE
- Pagine Spa e Morgex complete, con prezzi e orari
- Articolo 2

OGNI MESE, DA GENNAIO
- 1 articolo
- Controllo di 3 numeri: visite da Google · presenza su ChatGPT e Gemini ·
  telefonate, WhatsApp e prenotazioni dal sito (verificate su Beddy)

METÀ GENNAIO 2027
- Primo bilancio insieme: confronto con il punto di partenza
```

## Slide 6 · Un articolo al mese

```
Slide 6 – Titolo: UN ARTICOLO AL MESE
Griglia 4×3 di 12 riquadri bianchi: in alto il mese in piccolo, sotto il
titolo dell'articolo. Nota in basso: "Ogni articolo esce circa un mese
prima del periodo a cui serve."
Nov — Sciare a Courmayeur e La Thuile dormendo a Morgex
Dic — In vacanza con il cane a Morgex: passeggiate, regole, servizi
Gen — Weekend romantico vicino a Courmayeur: due notti tra Spa e Monte
      Bianco
Feb — Cosa fare a Morgex in inverno senza sciare
Mar — Skyway Monte Bianco con il cane: regole e consigli
Apr — Dove dormire tra Courmayeur e La Thuile: perché Morgex
Mag — 5 passeggiate facili con il cane vicino a Morgex
Giu — Da Morgex al Lago d'Arpy: percorso, tempi, consigli
Lug — Rafting e sport estivi vicino a Morgex
Ago — Terme di Pré-Saint-Didier: una giornata partendo da Morgex
Set — Autunno a Morgex: vendemmia, larici e silenzio
Ott — Dove mangiare a Morgex e in Valdigne
```

## Slide 7 · Cosa ci serve da voi

```
Slide 7 – Titolo: COSA CI SERVE DA VOI
Due box bianchi affiancati.

Box 1 – DA CONFERMARE
- Check-in: 14–19 o 15–22? Si può arrivare più tardi?
- Cani: c'è un limite di peso o taglia? (Expedia e Hotels.com scrivono
  "fino a 10 kg"). C'è un supplemento? Quanto costa il dog-sitter?
  Fornite cuccia e ciotole?
- Garage coperto: quanto costa? È incluso nelle offerte? Chi ricarica
  l'auto elettrica (la colonnina è nel garage) paga il garage?
  (oggi il sito in alcuni punti lo chiama "gratuito")
- Spa: 35 € l'ora a persona o per il gruppo? Orari? Quante persone
  per turno? Possiamo scrivere che è aperta anche a chi non dorme
  in hotel?
- Colazione: orari?

Box 2 – ACCESSI E CONTATTI
- Account Google dell'hotel (Search Console e scheda Google)
- Accesso a Booking e alle altre OTA (per aggiornare le descrizioni)
- Accesso al pannello Beddy (per vedere le prenotazioni arrivate dal sito)
- Beddy: chiedere se può mostrare i vostri prezzi direttamente su Google
```

---

## Note per la presentazione

- **Slide 2, riquadro "11":** le 4 pagine citate (Home, Pet friendly, Spa, Contatti) sono confermate da Nicolò in Semrush (9 ott). Da dire: Home e Contatti sono entrambe lette dalle AI e danno **due orari di check-in diversi** (14–19 e 15–22). È l'esempio concreto per il problema 5 della slide 3.

- **Slide 2:** i 92/100 (Lighthouse mobile), il 4,8 di Tripadvisor e le 11 menzioni (Semrush) vengono dal vecchio report e non li ho ricontrollati. Il +39% è calcolato da GA4: Francia da 84 a 117 utenti, Svizzera da 69 a 96, luglio–settembre. Il "un terzo" viene dall'analisi Google Ads: cluster Morgex circa 5 € a contatto contro circa 16 € del resto, quindi è un **rapporto**, non un valore assoluto (il segnale di conversione era inquinato).
- **Slide 3, punto 1:** il -63% confronta luglio–settembre 2025 (vecchio sito) con luglio–settembre 2026 (sito nuovo, online da ottobre 2025). La causa più probabile sono le vecchie pagine perse: 108 su 128 vecchi indirizzi trovati su Wayback Machine danno 404 (verificato il 9 ottobre 2026). Search Console servirà a confermarlo.
- **Slide 4, "chi":** il tasto "Chiama" è assegnato a DIGIVAL; se si riesce a farlo da Oxygen, diventa "Noi".
- **Carta d'identità:** non è nel deck. Si consegna come allegato dopo le risposte della slide 7 (`CARTA_IDENTITA_HOTEL.md`).
