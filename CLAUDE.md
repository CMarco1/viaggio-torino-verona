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
- **Torino ↔ Alba: treno regionale SFM4**, nessuna prenotazione necessaria,
  orario al minuto :07 di ogni ora. **Lo stesso treno ferma sia a Torino
  Lingotto sia a Torino Porta Susa, 8 minuti di distanza** (confermato su
  Trenitalia in entrambi i versi) — niente metro, si sale/scende direttamente
  a Porta Susa. **Vincolo duro: l'8 agosto l'ultimo treno utile da Torino ad
  Alba parte alle 19:33 da Porta Susa** (19:41 a Lingotto). Il pomeriggio a
  Torino del Giorno 1 va scritto per finire in tempo per quel treno, con
  margine per arrivare in stazione.
- Non è previsto un budget dettagliato per questo viaggio: **niente pagina
  costi**.
- Il **Giorno 6** ha due impegni serali fissi (degustazione con Virginia +
  **Carmina Burana** all'Arena): orari, prezzi e link stanno in
  `giorno-06.html` e `prenotazioni.html`, non qui — non duplicare qui gli
  orari, cambiano più spesso di quanto sembri.

## Decisioni già prese

- ✅ **9 agosto — Langhe, con orari confermati dalla sorella**: partenza verso
  le 11:00, tappa a **Neive**, **pranzo alle 13:00** in cantina (già
  prenotato, nome ancora da confermare), **degustazione guidata alle 16:30**.
  Dopo la degustazione, **La Morra ed eventualmente il castello di Barolo**
  entrano come tappa **facoltativa** in auto (quella della sorella): lei ha
  segnalato che il posto della degustazione non è lontano da La Morra, quindi
  probabilmente ci si passa, ma non è un piano fisso — dipende dal tempo sul
  posto.
- ✅ **Giorno 3 (10 agosto) — giornata intera a Torino, andata e ritorno in
  treno da Alba**: sostituisce il vecchio piano "Alba di mattina, La Morra e
  Barolo di pomeriggio" (quel giro in auto è ora facoltativo nel Giorno 2, non
  più un piano fisso del 10 agosto). Con una giornata intera dedicata solo a
  Torino, il **Palazzo Reale** finalmente ci sta (prima, fra Giorno 1 e il
  vecchio Giorno 4, restava sì e no un'ora di visita vera): entra nel piano
  insieme all'**ascensore della Mole**, spostato qui dal vecchio Giorno 4. Il
  Museo Egizio diventa una tappa facoltativa a bassa priorità, non più "da
  rimandare a un altro viaggio". Nessun bagaglio da portare: è una gita in
  giornata, si dorme ancora ad Alba quella sera.
- ✅ **Giorno 4 (11 agosto) — mattina ad Alba, Torino solo di passaggio**:
  dato che Torino è già stata vista con calma il giorno prima, oggi non c'è
  più bisogno di tornarci per visitare qualcosa. La mattina resta ad Alba
  (Duomo, corso, torri, un'ultima tappa da Bodrato), poi si prende il
  regionale verso Torino Porta Susa solo per la coincidenza con l'Italo delle
  13:00 — nessuna visita, nessun deposito bagagli (la sosta è troppo breve
  per averne senso).
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

- Nome esatto della cantina del pranzo/degustazione del 9 agosto (Neive): da
  confermare con la sorella.
- Se il giro del 9 agosto tocca davvero La Morra e/o Barolo dopo la
  degustazione: probabile ma non fissato, dipende dal tempo sul posto.
- Orari dei regionali Alba↔Torino del **Giorno 3** (andata e ritorno, 10
  agosto) e della mattina del **Giorno 4** (11 agosto): nessuno di questi è
  la stessa corsa già confermata su Trenitalia (quelle confermate restano
  solo le due dell'8 agosto sera e della vecchia mattina dell'11). Vanno
  riverificati più vicino alla data, in particolare il ritorno delle 19:33 il
  10 agosto: quel giorno è un lunedì, non un sabato come l'8 agosto.
- Prenotazione su Airbnb della degustazione del Giorno 6: decisa, ma va
  ancora completata online — solo 4 posti per slot.
- Biglietti del Carmina Burana del Giorno 6: scelto lo spettacolo, va ancora
  scelto il settore e completato l'acquisto sul sito ufficiale dell'Arena
  Opera Festival.
