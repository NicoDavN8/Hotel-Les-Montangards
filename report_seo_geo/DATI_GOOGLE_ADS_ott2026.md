# Dati Google Ads per l'incontro del 10 ottobre 2026

**Fonte:** API Google Ads, account `4130469299`, estrazione del 9 ottobre 2026.
**Uso:** la slide "Google Ads" (2b nel file del report) e le risposte se il proprietario chiede numeri. È un documento interno.

---

## 1. Cosa misura davvero ogni conversione (verificato per tipo)

| Azione | Tipo in Google Ads | Cosa conta | Lug–set 2026 |
|---|---|---|---|
| Chiamate da ADS \| Click-to-call | GOOGLE_HOSTED (azione locale) | **tocchi sul tasto "Chiama"** dell'annuncio | 51 |
| Chiamate Organiche | WEBPAGE (tag sul sito) | **tocchi sul numero di telefono del sito** | 102 |
| MSG WhatsApp da ADS | (asset messaggio) | clic su WhatsApp nell'annuncio | 30 |
| Whatsapp Organico | WEBPAGE | clic su WhatsApp nel sito | 147 |
| Acquisto | WEBPAGE (Beddy) | prenotazioni online completate | 2 (766 €) |

⚠️ Le due azioni "chiamate" hanno il campo "durata minima 60 s", ma **su questi tipi non si applica**. Sono **richieste di chiamata**, non telefonate verificate.
Tutte le conversioni Ads sono di persone che hanno avuto un'interazione con un annuncio: "Organico" vuol dire "partito dal sito", non "traffico non pubblicitario".

## 2. Luglio–settembre 2026

| | Luglio | Agosto | Settembre | Totale |
|---|---|---|---|---|
| Spesa | 456,40 € | 456,57 € | 456,53 € | **1.369,50 €** |
| Clic | 6.802 | 3.186 | 862 | 10.850 |
| Richieste di chiamata (ADS + sito) | 56 | 59 | 38 | **153** |
| Clic WhatsApp (ADS + sito) | 81 | 58 | 38 | **177** |
| Prenotazioni online | 0 | 0 | 2 | **2** (766 €) |
| **Contatti totali** | 137 | 117 | 78 | **332**, circa **4 €** l'uno |
| Clic per contatto | 50 | 27 | 11 | |

- **Il totale mensile scende** (137, 117, 78): probabilmente stagionalità. **Non mostrare grafici mese per mese** al proprietario, solo i totali del trimestre.
- **Clic sempre più qualificati:** servivano 50 clic per un contatto a luglio, 11 a settembre e circa 8 nei primi 8 giorni di ottobre.
- **WhatsApp dall'annuncio in crescita:** 10, 20, poi 15 nei primi 8 giorni di ottobre. Le richieste di chiamata dall'annuncio calano: 20, 12, 1.
- **Il 95% dei contatti arriva da smartphone** (314 su 332).
- **Per ripagare 1.370 €:** bastano 2–3 prenotazioni da circa 620 € (media dei valori di Acquisto: 1.720,40 € per 2 a giugno, 766 € per 2 a settembre). Il calcolo è sul fatturato, non sul margine.

## 3. Gennaio–settembre 2026
- **Spesa:** 4.104 €.
- **Contatti:** circa 657, cioè circa 6 € a contatto.
- **Prenotazioni online:** 4, per 2.486 €.
- **Prima di maggio i numeri non sono confrontabili:** `Chiamate Organiche` e `Whatsapp Organico` iniziano a contare davvero da maggio–giugno.

## 4. ⚠️ Telefonate vere: 4 su 10 senza risposta
Fonte: dettaglio chiamate (`call_view`), cioè le chiamate tramite numero di inoltro dell'estensione di chiamata, con durata e stato.

| Periodo | Chiamate | Senza risposta | Con risposta | Di cui ≥ 60 s |
|---|---|---|---|---|
| 2026 (gen – 9 ott) | 138 | **55 (40%)** | 83 | 51 |
| Lug–set 2026 | 46 | 17 (37%) | 29 | 19 |
| Dal 2023 | 673 | 248 (37%) | 425 | — |

**Quando si perdono (2026):**

| Fascia | Senza risposta |
|---|---|
| 7–9 | 17% |
| 9–13 | **42%** |
| 13–15 | 17% |
| 15–19 | **45%** |
| 19–22 | 40% |
| 22–7 | **100%** (6 su 6) |

- **Weekend:** sabato 47%, domenica 50%.
- **Durata delle chiamate con risposta:** mediana 75 secondi, quindi sono conversazioni vere.
- **A luglio 2026 non c'è nessun record:** l'estensione di chiamata era forse spenta.

**Cosa proporre:**
- deviare le chiamate su un cellulare quando la reception è occupata;
- programmare l'estensione di chiamata solo negli orari coperti, e negli altri lasciare WhatsApp.

## 5. Campagne
- Attiva solo **`PMax_Hotel_Summer 26`**. Le altre 6 sono **in pausa**, a spesa zero.
- Il nome "Summer" in autunno: controllare che le immagini e i testi non siano estivi con la stagione invernale alle porte.

## 6. Cosa NON mostrare al proprietario
- **Le "244 conversioni", il CPA di 5,56 €, il CTR del 7% e il CPC di 0,07 €** (maggio–luglio): sono gonfiati dal traffico display.
- **Il ROAS calcolato solo su Acquisto** (1,27x): sembra basso perché le prenotazioni nate al telefono non sono tracciate.
- **La parola "telefonate"** per le azioni di chiamata: si dice "richieste di chiamata".
