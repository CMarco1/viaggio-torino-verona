# CLAUDE.md

Sito statico dell'itinerario di un viaggio Torino → Langhe → Verona: HTML a
mano, nessun build, nessun framework. Si modifica a mano e si guarda aprendo
i file. Il centro del viaggio è **il cibo e il vino**, insieme alle cose da
vedere.

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
  costi**.
- Il **Giorno 6** ha due impegni serali fissi (degustazione con Virginia +
  **Carmina Burana** all'Arena): orari, prezzi e link stanno in
  `giorno-06.html` e `prenotazioni.html`, non qui — non duplicare qui gli
  orari, cambiano più spesso di quanto sembri.

## Decisioni già prese

- ✅ **Giorno 4 (11 agosto) — ascensore della Mole al posto del Palazzo
  Reale**: il tempo reale a Torino fra Giorno 1 e Giorno 4 è poco (circa
  un'ora di visita vera, tolti cibo e spostamenti), non abbastanza per il
  Palazzo Reale con gli interni (1h+). L'ascensore della Mole si fa in
  30-40 minuti e dà comunque il momento panoramico: il Palazzo Reale è
  trattato come il Museo Egizio, un buon motivo per tornare a Torino con più
  tempo. Se qualcosa slitta, si taglia il bicerin da Baratti & Milano, non la
  Mole.
- ✅ **9 agosto — Langhe**: pranzo e degustazione con la sorella e il suo
  ragazzo in una cantina di Langa (nome esatto da confermare con lei quando
  lo sa).
- ✅ **10 agosto — Alba di mattina, La Morra e Barolo di pomeriggio**: centro
  storico e botteghe di cioccolato/nocciola ad Alba, poi il belvedere di La Morra
  e il castello di Barolo in auto (15-20 minuti, non c'è treno) — **auto della
  sorella, già confermata**, nessun taxi da organizzare. Cambiato da
  una prima versione "solo Alba, nessuno spostamento": il centro da solo si
  esaurisce in poche ore, e tornare a Torino avrebbe significato una terza
  mezza giornata nella stessa città (dopo l'8 e l'11) per il costo di un
  treno di ~2h30 andata/ritorno. Restare in Langa con un'aggiunta breve in
  auto è il compromesso scelto.
- ✅ **12 agosto — tutto Verona**: Arena, centro storico, Casa di Giulietta,
  Ponte Pietra, Castelvecchio, giardino Giusti.
- ✅ **13 agosto — Verona con calma, poi degustazione e Carmina Burana**: la
  gita in giornata in Valpolicella è stata **tolta e sostituita** dalla
  degustazione con Virginia, trovata già pronta e prenotabile: copre Amarone e
  Valpolicella senza bisogno di auto, cantina da scegliere o una giornata
  intera fuori città. La sera si chiude con il **Carmina Burana** all'Arena,
  trovato disponibile per la stessa data: non un'aggiunta "se capita", ma il
  secondo impegno fisso della giornata insieme alla degustazione (anticipata
  apposta per lasciare margine). Il resto della giornata (mattina e primo
  pomeriggio) resta deliberatamente leggero — riposo, eventualmente
  Castelvecchio o il Giardino Giusti. Orari correnti in `giorno-06.html`.
- ✅ **Cena del Giorno 1: salsiccia di Bra e patate ripiene a Torino**, non ad
  Alba. Salsiccia di Bra da **Crostone.it** (Piazza Castello 72) e patate
  ripiene da **Poormanger** (Piazza Palazzo di Città), entrambe a due passi
  l'una dall'altra: è una richiesta esplicita, non un'opzione fra altre. Il
  bicerin che questo ha spostato fuori dal Giorno 1 è finito al mattino del
  Giorno 4, seconda volta a Torino.
- ✅ **Giorno 2, ordine invertito: pranzo prima, degustazione nel tardo
  pomeriggio**, non subito a ridosso l'uno dell'altra. La sorella ha
  confermato che la degustazione vera e propria sarà più tardi, non a ridosso
  del pranzo: il tempo fra i due è margine reale (i pranzi di Langa durano),
  non un buco da riempire.

## ⛔ Veti

- **Tartufo — abolito, in qualunque forma.** Niente tajarin al tartufo, niente
  tartufo grattugiato, niente prodotti conservati (creme, olio tartufato),
  niente tappe pensate intorno al tartufo (botteghe a tema, ecc.). Non è una
  questione di stagione: è fuori a prescindere. Se un locale è consigliato per
  *altro*, va bene lo stesso; se è consigliato *per* il tartufo, si sostituisce.

## Cosa piace

**Da mangiare e bere — è il centro del viaggio, non un contorno**, insieme ai
posti dove farlo: ogni giorno, dove possibile, ha un ristorante o locale
concreto consigliato, non solo il nome del piatto.
Piemonte: tajarin (al sugo d'arrosto o al ragù), agnolotti del plin, vitello
tonnato, brasato al Barolo, bicerin, cioccolato e nocciola (gianduia), vini di
Langa (Barolo, Barbaresco, Dolcetto, Nebbiolo).
Veneto: risotto all'Amarone, bigoli, tortellini di Valeggio, Amarone, Recioto,
Soave, spritz. A parte il tartufo (vedi Veti), nessun altro piatto è bandito —
l'obiettivo resta trovare i posti giusti.

**Da vedere:** Torino (Piazza San Carlo, Mole Antonelliana, Via Po), i colli
delle Langhe (La Morra, Barolo), il centro di Alba, l'Arena e il centro
storico di Verona. Nessun tema "nerd" in questo viaggio.

## Come si scrive sul sito

Registro fisso su tutte le pagine: **seconda persona plurale ("fate",
"arrivateci"), motivo concreto per ogni scelta, un fatto verificabile per
tappa, nessun entusiasmo generico**. Ogni giornata spiega la *logica* di sé
stessa in "Note e dritte".

Struttura di `giorno-NN.html` (non inventarne una nuova, vale per tutti i
sette giorni):

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

Questo viaggio **non ha foto proprie**: tutte le immagini in `images/` sono
state scaricate da fonti libere da riuso (Wikimedia Commons) e sono
accreditate in `images/CREDITS.md`. Se in futuro arrivano foto vere del
viaggio, sostituiscono i placeholder mantenendo lo stesso nome file, e la riga
corrispondente va tolta da `CREDITS.md`.

## Debito noto

- Nome esatto della cantina del pranzo/degustazione del 9 agosto: da
  confermare con la sorella.
- Orario esatto del treno regionale Alba→Torino della mattina del Giorno 4:
  la linea ha corse pressoché orarie, ma va verificato vicino alla data per
  avere margine sul treno Italo delle 13:00 da Torino.
- Prenotazione su Airbnb della degustazione del Giorno 6: decisa, ma va
  ancora completata online — solo 4 posti per slot.
- Biglietti del Carmina Burana del Giorno 6: scelto lo spettacolo, va ancora
  scelto il settore e completato l'acquisto sul sito ufficiale dell'Arena
  Opera Festival.
