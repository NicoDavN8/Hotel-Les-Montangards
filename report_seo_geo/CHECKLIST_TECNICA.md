# Checklist tecnica del sito: solo per Nicolò

**Basata sul controllo dell'HTML del 9 ottobre 2026** (38 pagine IT/FR/EN, sitemap, container GTM, Wayback Machine). Prima di ogni intervento ricontrolla la pagina: potrebbe essere già cambiata.
**Regola:** quello che si fa da WordPress (Rank Math, WPML, Oxygen, GTM) lo fa N8. A DIGIVAL va solo ciò che richiede un webmaster (template, codice, DNS).
Sito: WordPress 7.1.3 · Oxygen Builder · WPML (IT/FR/EN) · Rank Math · LiteSpeed Cache · GTM `GTM-KB856LKL` · GA4 `G-MT3SKKT496` · Ads `AW-10987484992` · booking engine Beddy (`lesmontagnards.beddy.io`).

---

## Settimana 1 · 12–16 ottobre

### 1. Telefono sbagliato nel menu ⚠️
- **Dove:** pannello del menu (blocco "Contattaci" in alto, Oxygen `text_block-808-89`), presente su **tutte le pagine**.
- **Ora:** `href="tel:+3910651710000"` (1065 al posto di 0165) → chiama un numero inesistente.
- **Correggere in:** `href="tel:+3901651710000"`. Il footer (`link_text-19-108`) è già giusto.
- Dopo la modifica svuota la cache di LiteSpeed.

### 2. Tasto "Chiama" su mobile → DIGIVAL (se non si riesce da Oxygen)
- La barra fissa in basso (`bottom-bar`) ha WhatsApp, email e "Prenota ora", **ma nessun tasto per chiamare**. Il telefono è il canale di vendita principale (vedi analisi Ads).

### 3. Google Search Console + Bing
- **Non esiste.** Creare la proprietà con l'account Google dell'hotel (o dare accesso a N8):
  - **Dominio** (via DNS, serve chi gestisce il dominio), oppure
  - **Prefisso URL** `https://www.hotelmontagnards.com/`, verificabile tramite GTM/GA4 già installati o con il meta tag in Rank Math → Impostazioni generali → Strumenti per webmaster.
- **Inviare le sitemap:** `/sitemap_index.xml`, `/fr/sitemap_index.xml`, `/en/sitemap_index.xml`.
- **Esportare subito il rendimento:** Search Console conserva al massimo 16 mesi. Se mostra lo storico, il periodo prima del nuovo sito (giugno–ottobre 2025) esce dalla finestra entro febbraio 2027.
- **Collegare Search Console a GA4.**
- **Bing Webmaster Tools:** importare da Search Console (ChatGPT Search si appoggia molto a Bing).

### 4. Redirect delle vecchie pagine ⚠️
- **File:** `redirect_vecchie_url.csv`, con 108 vecchie URL in 404 e la nuova URL proposta (tutte le destinazioni verificate a 200).
- **Strumento:**
  - plugin **Redirection**, che importa direttamente il CSV, oppure
  - Rank Math → Redirezioni, una alla volta. Sempre **301**.
- **Casi particolari:**
  - **Privacy e cookie** (8 righe): la pagina privacy **non esiste**, e il link "Privacy Policy" nel footer punta a `#`. Prima va creata la pagina (anche per ragioni legali), poi si reindirizzano lì le vecchie URL.
  - `/1953/`: pagina sconosciuta, da guardare su Wayback prima di decidere.
  - **Spagnolo:** la versione ES è stata eliminata, quindi tutto va all'inglese.
- **Dopo:** ricontrollare con un crawl (Screaming Frog o il comando curl della sessione) e, quando Search Console sarà attiva, il report "Pagine → Non trovata (404)" per eventuali URL che mancano.

### 5. Pulizia della sitemap (Rank Math → Sitemap)
- Ci sono URL che reindirizzano: `/fr/hotel-les-montagrards` e `/en/hotel-les-montagrards` (refuso nello slug, 301 verso `/fr` e `/en`). Vanno tolte.
- Le categorie `non-categorizzato` / `non-classifiee` / `uncategorized` vanno messe in noindex o tolte.
- **Le offerte non sono in sitemap:** attivare il tipo di contenuto "Offerte".

---

## Settimana 2 · 19–23 ottobre (servono le risposte del proprietario)

> **Priorità:** le 4 pagine che Semrush rileva come fonti delle AI sono **Home, Pet friendly, Spa e Contatti** (confermate il 9 ott). Si correggono per prime, in tutte e tre le lingue: check-in e garage in Home e Contatti; meta e regole nella pagina Pet; prezzo e orari nella pagina Spa.

### 6. Carta d'identità definitiva
Aggiornare `CARTA_IDENTITA_HOTEL.md` con le risposte: check-in, supplemento cani, dog-sitter, Spa (prezzo, orari, capienza, apertura agli esterni), colazione, cuccia e ciotole.

### 7. Correzioni sulle pagine in italiano

| Dove | Problema | Correzione |
|---|---|---|
| Home (FAQ) vs `/contatti` (FAQ), in tutte e 3 le lingue | check-in 14–19 vs 15–22 | un solo orario, quello confermato |
| `/camere`, meta description | "Wi-Fi, colazione alpina e **piccola spa inclusi**"; nomi delle camere sbagliati (Matrimoniale Economy, Junior Suite, Matrimoniale Deluxe) | togliere la Spa; usare i nomi reali |
| `/servizi`, meta description | "**Tutto incluso!**" | togliere |
| **Garage**: FAQ della home IT ("un garage **gratuito** previa disponibilità") e FR ("garage couvert **gratuit**"); `/offerte` ("Wi-Fi e parcheggio inclusi", non dice quale) | il parcheggio **scoperto è gratuito**, il **garage coperto è a pagamento** (Nicolò, 9 ott) | togliere "gratuito" dal garage; nelle offerte scrivere "parcheggio scoperto incluso". Tariffa del garage dopo la conferma del proprietario. La meta "parcheggio gratuito" della home va bene (si riferisce allo scoperto) |
| `/camere/family-junior-suite`, meta IT/FR/EN | **copiata dalla Superior**: "33 m², letto king, vasca, camera deluxe" | 38 m², 4 ospiti, matrimoniale + soppalco con futon per 2 bambini, terrazza coperta |
| `/camere/matrimoniale-deluxe` | in IT si chiama "Matrimoniale Deluxe" (title, H1, URL), altrove "Superior con terrazza" | rinominare in "Superior con terrazza". Se si cambia lo slug, aggiungere il redirect |
| `/servizi/pet-friendly`, meta | "Cani ammessi **fino senza** limitazioni di taglia, ciotole e cuccia su richiesta" | correggere la frase; ciotole e cuccia solo se confermate. Nel testo mancano il massimo di 2 cani e il dog-sitter |
| `/servizi/colazione-alpina` | refuso "miele **fi** fiori" | "miele di fiori" |
| `/servizi/spa` | mancano prezzo, orari, capienza, apertura agli esterni | aggiungere dopo la conferma |
| `/offerte` | "Offerte Last Minute **Primavera/Estate 2026**" ancora online a ottobre; "a partire da 490" senza € | aggiornare o nascondere; aggiungere € |
| `/noi-siamo.html` | "il **legno antico** che scricchiola" (la struttura è nuova); "croissant" (la colazione punta sulle torte fatte in casa) | riscrivere |
| Articolo Skyway | "3462 metri" (la pagina inverno dice 3.466) | 3.466 m |
| `/dintorni/morgex`, `/courmayeur`, `/la-thuile` | **due H1** ("Scopri le altre località vicine") e nessun H2 | il secondo H1 diventa H2 |
| Tutto il sito | circa 75% delle immagini senza testo alternativo (home 23 su 31) | aggiungere un alt descrittivo |

### 8. Misurazione
- **GTM:** aggiungere un trigger "Clic link, URL contiene `tel:`" che invia l'evento GA4 `click_telefono` (solo GA4: in Ads esiste già `Chiamate Organiche`, non duplicarla). Oggi GTM traccia già wa.me, i clic verso Beddy e tutto il funnel Beddy (view_item → add_to_cart → begin_checkout → purchase), con il cross-domain attivo.
- **GA4 vs Beddy:** confrontare le prenotazioni (purchase) di GA4 con il report di Beddy, luglio–settembre 2026. GA4 riporta 13.622,22 € in "Entrate totali": verificare.
- **Consent mode:** il default è `analytics_storage: denied`. Capire se è base o avanzato (spiega una parte di Direct/Unassigned).

---

## Settimane 3–4 · 26 ottobre – 6 novembre

### 9. Francese e inglese ⚠️ (sono le pagine che gli LLM citano)

| Dove | Problema |
|---|---|
| `/fr` (home) | **meta description interamente in italiano**; H2 "Tra cime, vallate e borghi autentici" in italiano |
| `/fr/services/spa`, meta e H2 | "Sauna, **hammam**… **Accès gratuit pour les clients**" (l'hammam non c'è e la Spa è a pagamento) |
| `/en/services/spa`, meta | "Wooden sauna, **Turkish bath**… **Free access for guests**" |
| `/en/services/spa`, testo | "Finnish wood-fired tubs heated to **room temperature**" (traduzione sbagliata) |
| `/fr` e `/en/services/pet-friendly` | "**sans supplément / no extra charge**" (in IT non è scritto: verificare); Lago d'Arpy, Val Veny e Val Ferret "**depuis l'hôtel / right from the hotel**" (in IT servono pochi minuti d'auto) |
| Schede camere FR/EN | "2 **persone**", "4 **persone**" in italiano; "**mq**" invece di m² |
| Offerte FR/EN | slug numerici `/fr/offres/3078`, `/en/offers/3049`, `/en/offers/3095`; **nessuna meta description**; resti in italiano ("Cosa include", "Fuga relax Monte Bianco", "Torna a tutte le promozioni"); `/fr/offres/soggiorno-relax-deluxe` |
| Esperienze EN | slug in italiano: `/en/experiences/ciaspole`, `/en/experiences/skyway-monte-bianco-in-estate` |
| FR in generale | si passa dal tu al voi tra una pagina e l'altra ("Découvre / Réserve" vs "Réservez / Contactez-nous"); `/fr/contacts`: "Contactez-nous et **accédez-nous**", "le **project** reCAPTCHA" |

Ogni volta che si cambia uno slug, aggiungere il redirect dal vecchio.

### 10. Dati strutturati (schema): procedura passo passo
**Oggi (home):**
- "Bieffepi Srl" registrata come `Person` + `Organization`;
- la home è un `Article` scritto da "digival", con `sameAs …/NEW`;
- **l'hotel non c'è.**

**Obiettivo:** mostrare **Hotel Les Montagnards** come `Hotel`, con **Bieffepi Srl (holding proprietaria) come ragione sociale**. Tempo: circa 1,5 ore.
Le etichette di Rank Math possono essere in italiano o in inglese: le indico entrambe.

**Passo 1 · Identità (Rank Math, ~15 min)**
1. Rank Math SEO → Dashboard → Moduli: controlla che **SEO locale / Local SEO** e **Schema** siano attivi.
2. Rank Math SEO → **Titoli e meta → SEO locale** (Titles & Meta → Local SEO) e compila:

| Campo | Valore |
|---|---|
| Persona o azienda | **Azienda** (Company) |
| Nome del sito | Hotel Les Montagnards |
| Nome della persona o organizzazione | **Hotel Les Montagnards** |
| Tipo di attività (Business Type) | **Hotel** |
| Logo | logo quadrato, almeno 112×112 px |
| URL | https://www.hotelmontagnards.com |
| Email · Telefono | info@hotelmontagnards.com · +39 0165 1710000 |
| Indirizzo | Viale della Rimembranza 26/30, 11017 Morgex (AO), IT |
| Coordinate geografiche | 45.7554244, 7.0390777 |
| Pagina Chi siamo · Contatti | /noi-siamo.html · /contatti |

Se un campo non c'è nella tua versione, saltalo: lo copre il passo 4.
3. **Titoli e meta → Social Meta:** URL della pagina Facebook, e nei **profili aggiuntivi** l'Instagram. Diventano il `sameAs`.

**Passo 2 · La home non è un "articolo" (~10 min)**
1. **Titoli e meta → Pagine** (Pages): tipo di schema predefinito da Article a **Nessuno** (None).
2. Apri la **home** in modifica → barra di Rank Math → scheda **Schema**: se c'è ancora "Article", eliminalo.
3. Fai lo stesso controllo su **Contatti**, **Servizi** e **Offerte**.

**Passo 3 · Autore "digival" (~2 min)**
1. Utenti → digival → **svuota il campo "Sito web"**: genera il `sameAs …/NEW`.
2. Rank Math → Titoli e meta → **Autori**: archivi autore disattivati.

**Passo 4 · La scheda completa dell'hotel (~30 min)**
Rank Math gratuito non ha il tipo Hotel tra gli schemi personalizzati, quindi usa una di queste tre strade:
- **(a)** Rank Math **Pro** → Schema → Generatore → **Schema personalizzato**: incolla il codice qui sotto e applicalo **solo alla home**;
- **(b)** plugin gratuito **WPCode** → nuovo snippet HTML in `<head>`, mostrato **solo sulla home**;
- **(c)** **Oxygen** → template della home → elemento **Code Block** con il codice.

Lo stesso `@id` di Rank Math (`#organization`) fa sì che Google unisca questa scheda a quella del passo 1, invece di vederne due.

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Hotel",
  "@id": "https://www.hotelmontagnards.com/#organization",
  "name": "Hotel Les Montagnards",
  "legalName": "Bieffepi Srl",
  "vatID": "IT01259560074",
  "url": "https://www.hotelmontagnards.com/",
  "telephone": "+39 0165 1710000",
  "email": "info@hotelmontagnards.com",
  "address": {"@type": "PostalAddress", "streetAddress": "Viale della Rimembranza 26/30",
    "postalCode": "11017", "addressLocality": "Morgex", "addressRegion": "AO", "addressCountry": "IT"},
  "geo": {"@type": "GeoCoordinates", "latitude": 45.7554244, "longitude": 7.0390777},
  "starRating": {"@type": "Rating", "ratingValue": "3"},
  "numberOfRooms": 12,
  "petsAllowed": true,
  "checkoutTime": "10:30",
  "amenityFeature": [
    {"@type": "LocationFeatureSpecification", "name": "Parcheggio scoperto privato gratuito", "value": true},
    {"@type": "LocationFeatureSpecification", "name": "Garage coperto a pagamento (secondo disponibilità)", "value": true},
    {"@type": "LocationFeatureSpecification", "name": "Ricarica auto elettriche", "value": true},
    {"@type": "LocationFeatureSpecification", "name": "Sauna", "value": true},
    {"@type": "LocationFeatureSpecification", "name": "Tinozze finlandesi riscaldate a legna", "value": true},
    {"@type": "LocationFeatureSpecification", "name": "Idromassaggio esterno", "value": true},
    {"@type": "LocationFeatureSpecification", "name": "Wi-Fi gratuito", "value": true},
    {"@type": "LocationFeatureSpecification", "name": "Ascensore", "value": true},
    {"@type": "LocationFeatureSpecification", "name": "Ristorante", "value": false}
  ],
  "sameAs": ["https://www.facebook.com/hotelmontagnardsmorgex", "https://www.instagram.com/hotel.les.montagnards/"]
}
</script>
```

**Da aggiungere dopo le risposte del proprietario:**
- `"checkinTime": "…"`, con l'orario confermato;
- i limiti sui cani nella descrizione (se esistono).

**Non** mettere `aggregateRating` con le recensioni Google o Booking: le stelle in Google non escono comunque per l'hotel che valuta se stesso, e rischia di essere considerato markup scorretto.

**Passo 5 · Verifica (~10 min)**
1. Svuota la cache di LiteSpeed.
2. Apri il [Test dei risultati multimediali](https://search.google.com/test/rich-results?url=https%3A%2F%2Fwww.hotelmontagnards.com%2F) e [validator.schema.org](https://validator.schema.org/) sulla home. Deve comparire **Hotel – Hotel Les Montagnards** con indirizzo e servizi, e **non** devono comparire più `Person` né `Article`.
3. Controlla anche `/fr` e `/en`: le impostazioni di Rank Math valgono per tutte le lingue, ma con WPML verifica che lo snippet sia attivo anche lì.

**Dopo (con calma):** `HotelRoom` nelle schede camera e `FAQPage` dove ci sono FAQ, in tutte e tre le lingue.

### 11. Fonti esterne
- **Scheda Google:**
  - categoria principale Hotel;
  - attributi: animali ammessi, parcheggio gratuito, sauna/idromassaggio, ricarica EV, Wi-Fi;
  - check-in e check-out (dopo conferma);
  - descrizione allineata alla carta d'identità;
  - foto della Spa;
  - risposte alle recensioni.
- **Booking ed Expedia:** descrizione della **nuova** Spa (alcune schede parlano di "docce aromatiche"); attributi animali.
- **lovevda.it**, il portale ufficiale regionale (scheda 9004983): non cita né cani né Spa. Verificare come aggiornarla (ufficio turistico regionale). Dati presenti: 25 posti letto, 16 bagni, 922 m, listino 2025-26.
- **yesalps.com** chiama l'hotel "B&B-Hotel".
- **Expedia e Hotels.com** (dai risultati di ricerca, pagine bloccate ai controlli automatici): **cani "fino a 10 kg"** e "gratis". Va confrontato con la risposta del proprietario: se non c'è limite di peso, è l'errore più dannoso, perché esclude i cani di media e grande taglia. Ciotole "disponibili".
- **Travelocity**: indica un **ristorante**, che non c'è, e il "parcheggio a pagamento" (vero solo per il garage: lo scoperto è gratuito).
- **Omonimia**: esiste un "Hotel Les Montagnards" a **Morteau (Francia)**, sito hotel-les-montagnards.com. Nelle schede e nei testi usare sempre "Hotel Les Montagnards **Morgex**".
- **Bing Places**; facoltativo Apple Business Connect.
- **Beddy:** chiedere del collegamento a **Google Hotel Center / free booking links**, per avere il prezzo del sito ufficiale accanto a Booking su Google Hotels e AI Mode.

### 12. Punto di partenza GEO (da rifare ogni mese)
Le stesse 20 domande su **ChatGPT** e **Gemini** (meglio anche Google AI Mode e Perplexity), in navigazione anonima. Per ognuna annotare:
- se l'hotel compare (sì/no);
- in che posizione;
- quali fonti cita;
- quali concorrenti compaiono.

| # | Domanda |
|---|---|
| 1 | Hotel consigliati a Morgex |
| 2 | Dove dormire vicino a Courmayeur con il cane |
| 3 | Hotel pet friendly in Valle d'Aosta senza limiti di taglia per il cane |
| 4 | Hotel vicino a Courmayeur con spa o sauna |
| 5 | Dove dormire per sciare a Courmayeur e La Thuile spendendo meno |
| 6 | Hotel tranquillo vicino al Monte Bianco per un weekend romantico |
| 7 | Hotel a Morgex con parcheggio gratuito |
| 8 | Dove dormire vicino allo Skyway Monte Bianco |
| 9 | Hotel in Valle d'Aosta con colazione fatta in casa |
| 10 | Hotel per famiglie vicino a Courmayeur |
| 11 | Hotel vicino alle Terme di Pré-Saint-Didier |
| 12 | Spa a ore con tinozze finlandesi in Valdigne |
| 13 | Hôtel acceptant les chiens près de Courmayeur |
| 14 | Où dormir près de Courmayeur pour skier |
| 15 | Hôtel avec spa près du Mont-Blanc côté italien |
| 16 | Hôtel à Morgex |
| 17 | Dog-friendly hotel near Courmayeur |
| 18 | Where to stay near Courmayeur for skiing on a budget |
| 19 | Small hotel with spa near Mont Blanc, Italy |
| 20 | Hotel in Morgex, Aosta Valley |

---

## Novembre e dicembre · pagine da arricchire

Oggi le pagine hanno circa 300 parole e poche informazioni concrete. Obiettivo: rispondere alle domande che i clienti fanno (e fanno alle AI).

- **Courmayeur e La Thuile** (entro fine novembre):
  - km e minuti dall'hotel (10 km/10 min, 15 km/20 min);
  - dove si parcheggia agli impianti;
  - **niente skibus, si va in auto**;
  - km di piste;
  - collegamenti a camere e offerte;
  - FAQ.
- **Cani:**
  - regole complete: nessun limite di taglia, massimo 2, non in sala colazione durante il servizio, non in Spa;
  - supplemento e dog-sitter con i prezzi;
  - sentieri dall'hotel vs in auto (Arpy, Val Veny, Val Ferret);
  - veterinario più vicino;
  - FAQ.
- **Spa:**
  - prezzo, orari, capienza;
  - aperta agli esterni;
  - cosa portare, cosa si noleggia;
  - massaggi;
  - FAQ.
- **Morgex:**
  - distanze;
  - servizi in paese;
  - Blanc de Morgex;
  - sci nordico (19 km di piste ad Arpy, fonte lovevda);
  - FAQ.

Il calendario degli articoli è nella slide 6 di `REPORT_7_slide_claude_design.md`.
