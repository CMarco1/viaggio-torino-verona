# CLAUDE.md

Sito statico dell'itinerario di un viaggio Torino → Langhe → Verona: HTML a
mano, nessun build, nessun framework. Si modifica a mano e si guarda aprendo
i file. Stessa impostazione di `viaggio-giappone-2`, riadattata a un viaggio
più corto e senza tema nerd: qui il centro è **il cibo e il vino**, insieme
alle cose da vedere.

Questo file contiene i fatti fissi del viaggio, le decisioni già prese e le
convenzioni del sito. Vale prima di qualunque consiglio da guida turistica.

## I fatti fissi

- **8-14 agosto 2026**, 7 giorni, **6 notti**, **2 persone**.
- **3 notti a Langa (8→11 ago)**, ospiti della sorella ad **Alba**. Nessun
  hotel: niente indirizzo pubblico, niente orari di check-in/out da scrivere.
- **3 notti a Verona (11→14 ago)**, **Hotel Leopardi**, Via Leopardi 16.
  Prenotazione confermata (n. 2515228984), doppia economy, 238,07 € + 28,85 €
  di tassa di soggiorno da pagare in struttura.
- **Rientro la sera del 14**: si parte da Verona P.N. alle 18:22 e si arriva a
  Roma Termini alle 22:13. Nessuna notte extra, si rientra a casa in giornata.
- **Treni Italo, tutti confermati** (4 tratte, contatto prenotazione Marco
  Coccia):
  | Giorno | Data | Tratta | Treno | Orario | Ambiente |
  |---|---|---|---|---|---|
  | G1 | sab 8/8 | Roma Termini → Torino P.S. | 9924 | 10:40 → 15:20 | Smart |
  | G4 | mar 11/8 | Torino P.S. → Milano Centrale | 8143 | 13:00 → 14:00 | Smart |
  | G4 | mar 11/8 | Milano Centrale → Verona P.N. | 8989 | 15:35 → 16:55 | Smart |
  | G7 | ven 14/8 | Verona P.N. → Roma Termini | 8967 | 18:22 → 22:13 | Prima Business |

  I codici di prenotazione e i numeri dei biglietti **non vanno scritti sul
  sito** (è pubblico): restano nei PDF dentro `biglietti/`, che è ignorata da
  git.
- **Torino ↔ Alba: treno regionale**, nessuna prenotazione necessaria,
  servizio pressoché orario (~1h15-1h25). **Vincolo duro: l'8 agosto l'ultimo
  treno utile da Torino ad Alba parte alle 19:41.** Il pomeriggio a Torino del
  Giorno 1 va scritto per finire in tempo per quel treno, con margine per
  arrivare in stazione.
- Non è previsto un budget dettagliato per questo viaggio: **niente pagina
  costi**, a differenza del sito Giappone.

## Decisioni già prese

- ✅ **9 agosto — Langhe**: pranzo e degustazione con la sorella e il suo
  ragazzo in una cantina di Langa (nome esatto da confermare con lei quando
  lo sa).
- ✅ **10 agosto — giornata ad Alba**: centro storico, mercato, botteghe di
  tartufo e nocciola, nessuno spostamento. Scelto esplicitamente invece di un
  giro dei borghi (Barolo/La Morra) o di una giornata di puro relax: è
  l'opzione a ritmo tranquillo ma con qualcosa da vedere.
- ✅ **12 agosto — tutto Verona**: Arena, centro storico, Casa di Giulietta,
  Ponte Pietra, Castelvecchio, giardino Giusti.
- ✅ **13 agosto — gita in Valpolicella**: cantine Amarone/Recioto, borghi
  (Fumane, Sant'Ambrogio, San Pietro in Cariano). È uno scambio rispetto a un
  secondo giorno di sola Verona: la giornata del 12 copre già la città.
- ✅ **Cena del Giorno 1**: ad Alba/Langa, dopo il trasferimento serale — non
  a Torino prima di partire.

## Cosa piace

**Da mangiare e bere — è il centro del viaggio, non un contorno:**
Piemonte: tajarin al tartufo, agnolotti del plin, vitello tonnato, brasato al
Barolo, bicerin, vini di Langa (Barolo, Barbaresco, Dolcetto, Nebbiolo).
Veneto: risotto all'Amarone, bigoli, tortellini di Valeggio, Amarone, Recioto,
Soave, spritz. Nessun veto esplicito: a differenza del viaggio in Giappone,
qui non ci sono piatti banditi — l'obiettivo è trovare i posti giusti, non
evitarne.

**Da vedere:** Torino (Piazza San Carlo, Mole Antonelliana, Via Po), i colli
delle Langhe, il centro di Alba, l'Arena e il centro storico di Verona,
le cantine della Valpolicella. Nessun tema "nerd" in questo viaggio.

## Come si scrive sul sito

Stesso registro del sito Giappone: **seconda persona plurale ("fate",
"arrivateci"), motivo concreto per ogni scelta, un fatto verificabile per
tappa, nessun entusiasmo generico**. Ogni giornata spiega la *logica* di sé
stessa in "Note e dritte".

Struttura di `giorno-NN.html` (non inventarne una nuova — identica a
`viaggio-giappone-2`):

- `.dayhero` + `.chips` — i chip devono coincidere con il teaser della card in
  `index.html`.
- `.card.accent.a-sintesi` → `ul.synth`, tre righe.
- `.card.a-itin` → `ol.timeline`, `<li><span class="t">HH:MM</span><div>…</div></li>`.
  Le tappe facoltative hanno `class="opt"` sul `<li>`.
- `.card.a-mappa` → iframe Google Maps + link `.maplink`. Se cambi le tappe,
  **aggiorna anche saddr/daddr**.
- `.card.a-mangiare` → `ul.eat` con `<span class="when">Pranzo</span>`.
- `.card.a-note.prose` → paragrafi che aprono con `<strong>`.
- Navigazione in fondo: `.dayfoot` prev/home/next.
- Priorità: `<span class="prio prio-high|prio-med|prio-low">`.

Toccando un giorno, controlla sempre gli effetti su: `index.html` (teaser e
immagine), `prenotazioni.html` (se nasce o muore una prenotazione),
`mangiare.html` (se il consiglio è generale e non di giornata).

## Immagini

A differenza di `viaggio-giappone-2`, questo viaggio **non ha foto proprie**:
tutte le immagini in `images/` sono state scaricate da fonti libere da riuso
(Wikimedia Commons) e sono accreditate in `images/CREDITS.md`. Se in futuro
arrivano foto vere del viaggio, sostituiscono i placeholder mantenendo lo
stesso nome file, e la riga corrispondente va tolta da `CREDITS.md`.

## Debito noto

- Nome esatto della cantina del pranzo/degustazione del 9 agosto: da
  confermare con la sorella.
- Orario esatto del treno regionale Alba→Torino della mattina del Giorno 4:
  la linea ha corse pressoché orarie, ma va verificato vicino alla data per
  avere margine sul treno Italo delle 13:00 da Torino.
- Cantina da prenotare per la gita in Valpolicella del Giorno 6.
