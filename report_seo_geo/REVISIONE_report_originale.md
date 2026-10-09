# Revisione del report "SEO & GEO Analysis – Ottobre 2026" (35 slide)

**Data:** 9 ottobre 2026
**Oggetto:** il deck Canva "WEB ANALYSIS" (`DAHW9nvdnTA`), sostituito dal report a 7 slide (`REPORT_7_slide_claude_design.md`).
**Metodo:**
- lettura del PDF slide per slide;
- HTML grezzo di 38 pagine del sito in IT/FR/EN;
- sitemap;
- container GTM;
- storico del vecchio sito su Wayback Machine (128 vecchie URL testate);
- schede esterne (lovevda.it, OTA).

## Verdetto
La **direzione strategica era giusta**: Morgex come posizionamento, pet friendly come asset principale, Spa e colazione come differenziatori, coerenza dei fatti, schema da sistemare.
La **base di evidenza era debole**: dati letti male, alcune definizioni tecniche sbagliate. Mancava il problema più grosso, la migrazione del sito senza redirect. Era anche troppo lungo e tecnico per il proprietario.

## Cosa reggeva (verificato)
- **Lo schema dichiara l'hotel come `Person`** "Bieffepi Srl", e le pagine come `Article`.
- **Check-in incoerente:** 14–19 in home, 15–22 in Contatti, in tutte e tre le lingue.
- **"Tutto incluso!"** nella meta description di `/servizi`.
- **Contaminazioni linguistiche FR/EN.** In realtà sono molte di più di quelle citate: vedi la checklist.
- **Pagine commerciali povere di testo.**

## Errori del report originale

| Slide | Il report diceva | Cosa risulta |
|---|---|---|
| 4, 8, 24 | "Sito complessivamente sano", "la SEO tecnica non è il collo di bottiglia", "assenza di criticità informatiche" | 108 vecchie URL su 128 sono in 404 dopo la migrazione (ottobre 2025); telefono sbagliato nel menu; Search Console assente |
| 5 | "Parametri in miglioramento" | **Organico: -62,8%** (da 1.287 a 479 sessioni). Il **totale** 2025, ricavato dalla quota del Direct (32,45%), è di circa 4.600 sessioni contro 2.603 (**-44%**). Utenti Italia: -44%. Cresce solo il Direct, che passa dal 32% al 71% del totale: segnale di attribuzione persa, non di salute. "Unassigned", con 0% di coinvolgimento, era segnato in verde. Gli eventi chiave e le entrate a zero nel 2025 dicono solo che il tracciamento non c'era. **Luglio–settembre 2025 = vecchio sito, luglio–settembre 2026 = sito nuovo.** |
| 6 | "+4% Francia / +3% Svizzera" | Sono punti di quota, non crescita. In assoluto +39% (da 84 a 117 e da 69 a 96 utenti), e la quota sale soprattutto perché crolla l'Italia |
| 7 | "AI Health = quante volte il sito compare negli LLM"; "Lighthouse misura la facilità di indicizzazione" | L'AI Search Health di Semrush misura la predisposizione tecnica (crawler AI non bloccati, dati strutturati, link interni), non le menzioni. Lighthouse è un audit di laboratorio (performance, accessibilità, best practice) |
| 9 | "Il robots.txt comprende feed e comment feed" | Il robots.txt è di 4 righe e non contiene feed. Le offerte con ID numerico non sono nemmeno in sitemap: il problema reale è che nessuna offerta è in sitemap e le FR/EN non hanno slug tradotto né meta description |
| 11 | "Family Junior Suite: 40 m² nella sitemap" | "40 m²" non esiste da nessuna parte. L'errore vero: la meta della FJS è **copiata dalla Superior** ("33 m², letto king, vasca") in tutte e 3 le lingue |
| 15 | "Google Rich Results analizza le informazioni che il sito passa agli LLM" | Il Rich Results Test verifica l'idoneità ai risultati arricchiti di Google, non riguarda gli LLM |
| 18 | Carta d'identità con check-in 14–19 | È uno dei due valori in conflitto, scelto senza conferma. Mancavano le cose che l'hotel non offre (ristorante, skibus, piscina, hammam, Spa inclusa) e alcune distanze erano vaghe ("pochi minuti") |
| 19 | Obiettivo: "incrementare il tempo di permanenza" | Non è un KPI per un hotel. I KPI sono i contatti diretti, le ricerche del brand e la presenza nelle risposte AI |
| 20 | "Morgex: circa 12% di conversione, circa 5 €"; "il brand è più forte" | Numeri dell'analisi Ads con il segnale di conversione inquinato: valgono solo come rapporto tra cluster. E non è il brand: è domanda locale generica |
| 31 | Mock-up | La Spa del mock-up è una piscina interna che l'hotel non ha. Le camere sono 4 categorie generiche contro le 5 reali (manca la Comfort vista Monte Bianco) |
| 33-35 | 60 titoli di blog | Irrealistico: il blog ha 6 articoli fermi a ottobre 2025 e il ritmo possibile è 1 al mese. Almeno 6 titoli "dove dormire… perché Morgex" si cannibalizzano; molti duplicano le 18 pagine esperienze esistenti; tutti in italiano |
| Forma | | Numerazione dell'indice (01–06) diversa da quella delle slide (03–07); "CORRETTAENTE"; "IDENTITA" senza accento; "IA/AI Health"; "Interesse contenuti" senza metrica né periodo |

## Cosa mancava
1. **La migrazione senza redirect.** È la causa più probabile del -63% organico. Vedi `redirect_vecchie_url.csv`.
2. **Le informazioni false in FR/EN** (Spa gratuita con hammam, cani senza supplemento, sentieri "dall'hotel"): sono quelle che gli LLM leggono.
3. **Il telefono sbagliato nel menu** (`tel:+3910651710000`) e l'assenza del tasto "Chiama" su mobile, quando il telefono è il canale di vendita principale.
4. **Le fonti esterne:** scheda Google (la fonte di Gemini, AI Mode e Maps), Google Hotel Center e Beddy, Bing (per ChatGPT), lovevda.it (non cita cani né Spa), OTA con la vecchia spa.
5. **Search Console:** non esiste, quindi mancano query, posizioni e il report degli errori 404.
6. **Un metodo per misurare la GEO:** un prompt per motore non è riproducibile. Serve un set fisso di 20 domande ripetuto ogni mese (vedi la checklist).
7. **La Spa come prodotto a sé:** aperta anche agli esterni a 35 €/h, è una domanda locale nuova. In più è senza recensioni: serve una campagna recensioni su Spa e cani.
8. **Le pagine che esistono già:** le pagine territorio (Morgex, Courmayeur, La Thuile), le 18 esperienze, Spa e Cani vanno **potenziate** (oggi circa 300 parole, doppio H1), non ricreate.

## Fonti verificate
- [Semrush KB: AI Search Health](https://it.semrush.com/kb/1601-ai-search-health-audit)
- [lovevda.it: scheda Hotel Les Montagnards](https://www.lovevda.it/it/banca-dati/22/alberghi-3-stelle/morgex/hotel-les-montagnards/9004983)
- [yesalps: "B&B-Hotel Les Montagnards"](https://www.yesalps.com/en/bnb/aosta-valley/lesmontagnards-73cd60b5f84.html)

## Copie Canva create durante la revisione
- `DAHXgnhk-RU`: copia completa del deck (35 pagine)
- `DAHXgnaZCHc`: 3 slide modello

Non servono più (il report si rifà in Claude Design): si possono cancellare da Canva.
