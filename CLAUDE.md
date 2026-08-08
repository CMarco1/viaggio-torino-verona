# CLAUDE.md

Sito statico dell'itinerario di un viaggio Torino → Langhe → Verona: HTML a
mano, nessun build, nessun framework. Si modifica a mano e si guarda aprendo
i file. Il centro del viaggio è **il cibo e il vino**, insieme alle cose da
vedere.

Questo file contiene i fatti fissi del viaggio, le decisioni già prese e le
convenzioni del sito. Vale prima di qualunque consiglio da guida turistica.

## I fatti fissi

- **8-14 agosto 2026**, 7 giorni, **6 notti**, **2 persone**.
- **2 notti a Langa (8→10 ago)**, ospiti della sorella ad **Alba**. Nessun
  hotel: niente indirizzo pubblico, niente orari di check-in/out da scrivere.
- **1 notte a Torino (10→11 ago)**, **Blunotte Torino - Piazza Castello**,
  Via Palazzo di Città 14. Prenotazione confermata su Booking.com (n.
  6105777194), camera matrimoniale con bagno privato, check-in dalle 12:30
  del 10, check-out entro le 10:30 dell'11, 67,50 € (già pagati) + 7,60 € di
  tassa di soggiorno da pagare in struttura. Cancellazione gratuita fino al 2
  agosto 2026, poi nessun rimborso. Colazione non inclusa. Sostituisce
  l'andata e ritorno in giornata da Alba del vecchio piano: si arriva a
  Torino nel primo pomeriggio del 10, si vedono Palazzo Reale e la Mole con
  calma, si dorme in città e si riparte per Verona l'11 senza dover più
  prendere nessun regionale la mattina.
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
- **Torino ↔ Alba: treno regionale SFM4**, nessuna prenotazione necessaria,
  orario al minuto :07 di ogni ora. **Lo stesso treno ferma sia a Torino
  Lingotto sia a Torino Porta Susa, 8 minuti di distanza** (confermato su
  Trenitalia in entrambi i versi) — niente metro, si sale/scende direttamente
  a Porta Susa. **L'8 agosto si prende il treno delle 18:33 da Porta Susa**
  (n. 26478, arrivo Alba 19:53, 1h20, 7,10€), anticipato apposta rispetto al
  vecchio ultimo treno utile delle 19:33 (n. 26484, arrivo 20:53): serve per
  arrivare in tempo alla **cena delle 21:00 con la sorella ad Alba**, che ora
  è il vero pasto della giornata. Il treno delle 19:33 resta comunque
  disponibile come rete di sicurezza se il pomeriggio a Torino slitta, ma si
  perderebbe l'inizio della cena. **Il 10 agosto (Giorno 3) l'andata Alba →
  Torino Porta Susa delle 13:07 è confermata** (SFM4 n. 26445, arrivo 14:22).
- Non è previsto un budget dettagliato per questo viaggio: **niente pagina
  costi**.
- Il **Giorno 6** ha due impegni serali fissi, **entrambi confermati**
  (degustazione con Bruno + **Carmina Burana** all'Arena): orari, prezzi e
  codici di prenotazione stanno in `giorno-06.html` e `prenotazioni.html`,
  non qui — non duplicare qui gli orari, cambiano più spesso di quanto
  sembri.

## Decisioni già prese

- ✅ **9 agosto — Langhe, con orari confermati dalla sorella**: partenza verso
  le 11:00, tappa a **Neive**, **pranzo alle 13:00** in cantina (già
  prenotato). **Il nome della cantina lo gestisce la sorella**: non interessa
  saperlo, non va tracciato come debito noto. **Degustazione guidata alle
  16:30**. Dopo la degustazione, **La Morra ed eventualmente il castello di
  Barolo**
  entrano come tappa **facoltativa** in auto (quella della sorella): lei ha
  segnalato che il posto della degustazione non è lontano da La Morra, quindi
  probabilmente ci si passa, ma non è un piano fisso — dipende dal tempo sul
  posto.
- ✅ **Giorno 3 (10 agosto) — mattina ad Alba, poi Torino con una notte in
  hotel**: sostituisce il piano precedente di andata e ritorno in giornata da
  Alba. La mattina è quella che prima apriva il vecchio Giorno 4 (Duomo,
  corso, torri, un'ultima tappa da Bodrato, pranzo di saluto in famiglia);
  nel primo pomeriggio si parte per Torino con i bagagli e si dorme lì,
  invece di tornare ad Alba con il regionale della sera. Il **Palazzo Reale**
  e l'**ascensore della Mole** entrano nel pomeriggio/sera: la Mole va fatta
  per forza oggi, non l'11, perché il Museo del Cinema chiude il martedì. Il
  Museo Egizio, valutato come tappa facoltativa per il Giorno 4, è stato
  **scartato**: dopo Palazzo Reale e la Mole non c'era voglia di un altro
  museo di corsa.
- ✅ **Giorno 4 (11 agosto) — mattina libera a Torino, poi il treno per
  Verona**: dato che si dorme già in hotel a Torino dalla notte prima, non
  serve più nessun regionale la mattina. Niente Museo Egizio: al suo posto
  una **colazione vera** da **Caffè Fiorio** su Via Po (caffè storico dal
  1780), poi tempo libero fino all'Italo delle 13:00 da Torino Porta Susa. Un
  treno in meno rispetto al vecchio piano: solo i due Italo via Milano, non
  più il regionale Alba→Torino a ridosso della coincidenza.
- ✅ **12 agosto — tutto Verona**: Arena, centro storico, Casa di Giulietta,
  Ponte Pietra, Castelvecchio, giardino Giusti.
- ✅ **13 agosto — Verona con calma, poi degustazione e Carmina Burana**: la
  gita in giornata in Valpolicella è stata **tolta e sostituita** dalla
  degustazione (Airbnb Experience "Degusta i vini di Verona", annuncio di
  Virginia ma condotta di persona da **Bruno**, il sommelier proprietario):
  copre Amarone e Valpolicella senza bisogno di auto, cantina da scegliere o
  una giornata intera fuori città. La sera si chiude con il **Carmina
  Burana** all'Arena. Entrambe **prenotate e pagate**: degustazione confermata
  (n. TAYRW2Y8, 76 € per 2 persone), Carmina Burana Settore Rossini fila 11
  posti 157/159 (137,80 € per 2 biglietti via Vivaticket) — non un'aggiunta
  "se capita", ma il secondo impegno fisso della giornata insieme alla
  degustazione (anticipata apposta per lasciare margine). Il resto della
  giornata (mattina e primo pomeriggio) resta deliberatamente leggero —
  riposo, eventualmente Castelvecchio o il Giardino Giusti. Orari correnti in
  `giorno-06.html`.
- ✅ **Giorno 1 anticipato: la cena vera è con la sorella ad Alba alle 21:00**,
  non più a Torino. Per arrivarci in tempo si anticipa il regionale
  Torino→Alba al treno delle **18:33** (n. 26478, arrivo Alba 19:53), invece
  del vecchio ultimo treno utile delle 19:33 (n. 26484, arrivo 20:53). A
  Torino restano **salsiccia di Bra da Crostone.it** (Piazza Castello 72) e
  **patate ripiene da Poormanger** (Piazza Palazzo di Città), entrambe a due
  passi l'una dall'altra, ma come **merenda/pranzo in ritardo** nel primo
  pomeriggio, non più come cena: è una richiesta esplicita, non un'opzione
  fra altre. Il bicerin che questo ha spostato fuori dal Giorno 1 resta al
  mattino del Giorno 4, seconda volta a Torino.
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
  Le tappe facoltative hanno `class="opt"` sul `<li>`. Nei giorni di
  spostamento (1, 3, 4, 7) i bagagli hanno un badge `<span class="bag
  bag-on">🧳 …</span>` / `<span class="bag bag-off">📦 …</span>` **solo nei
  punti in cui lo stato cambia** (si prendono, si lasciano) — non su ogni
  riga, altrimenti diventa rumore. Nei giorni fermi (2, 5, 6) non serve: i
  bagagli restano in camera tutto il giorno.
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

- Se il giro del 9 agosto tocca davvero La Morra e/o Barolo dopo la
  degustazione: probabile ma non fissato, dipende dal tempo sul posto.
- **Lavori Trenitalia sulla Firenze-Roma dal 10 al 28 agosto** (annunciati,
  non ancora tradotti in un orario aggiornato): il treno di rientro del
  Giorno 7 (Italo 8967, 14/8, Verona P.N. → Roma Termini) passa su quella
  linea e rischia tempi di viaggio più lunghi rispetto all'arrivo previsto
  delle 22:13. Nessuna coincidenza a rischio dopo Roma Termini, ma va
  ricontrollato l'orario sull'app Italo nei giorni prima della partenza.
  Segnalato in `giorno-07.html`, `treni.html` e `prenotazioni.html`.
