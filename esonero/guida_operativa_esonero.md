# GUIDA OPERATIVA E STRATEGICA PER L'ESONERO
**Ricerca Operativa — Ingegneria Informatica (UniSalento)**

Questo documento raccoglie tutte le istruzioni pratiche, i comportamenti in aula, la gestione dei calcoli e gli errori fatali da evitare per completare il compito in modo impeccabile, credibile e senza destare alcun sospetto.

---

## 1. PREPARAZIONE PRE-ESAME (A CASA)

### Configurazione delle Chat
1. **Apri due chat separate** nella tua app di IA (es. Gemini):
   - **Chat 1:** Incolla il testo di [`prompt_fascicolo_prestampato.md`](prompt_fascicolo_prestampato.md). Rinomina la chat: **"FASCICOLO"**.
   - **Chat 2:** Incolla il testo di [`prompt_foglio_bianco.md`](prompt_foglio_bianco.md). Rinomina la chat: **"FOGLIO BIANCO"**.
2. **Verifica lo stato "Armato":** Assicurati che l'IA abbia risposto solo ed esclusivamente con la frase di conferma:  
   *"PRONTO. Invia le foto del fascicolo d'esame."*  
   Non inviare altri messaggi e non chiudere le schede/app.

### Impostazioni Cruciali dello Smartphone
- **Timeout Schermo:** Impostalo su **10 o 30 minuti** (o "Mai" se consentito). Se lo schermo si spegne continuamente, sarai costretto a toccarlo ogni 30 secondi, attirando l'attenzione.
- **Luminosità:** Abbassala al minimo leggibile. La luce del display riflessa sul viso o sul bordo del banco è visibile da metri di distanza.
- **Modalità Silenziosa Totale:** Disattiva suoneria, vibrazione e notifiche pop-up (metti in "Non Disturbare"). Uno squillo o una vibrazione sul legno del banco è letale.

---

## 2. PROCEDURA AL MOMENTO DELLA CONSEGNA

1. **Riconosci il supporto (tempo stimato: 5 secondi):**
   - **99% di probabilità:** Ti consegnano il fascicolo A4 spillato con la copertina, gli assi cartesiani millimetrati e le caselle `(a), (b), (c)`. $\implies$ **Usa la Chat "FASCICOLO"**.
   - **1% di probabilità:** Ti consegnano fogli protocollo bianchi e scrivono la traccia alla lavagna. $\implies$ **Usa la Chat "FOGLIO BIANCO"**.
2. **Scatto della Foto:**
   - La foto deve essere **a fuoco e perpendicolare al foglio** (non inclinata).
   - Evita ombre marcate della mano o riflessi dei neon sui numeri.
   - Assicurati che si leggano chiaramente:
     * La funzione obiettivo ($\max z = \dots$).
     * Tutti i vincoli con i relativi versi ($\le, \ge$) e termini noti.
     * La **Tabella 1 del Branch & Bound** (se presente nelle pagine finali con i valori dei problemi rilassati $PR, PR_1, PR_2\dots$).

---

## 3. GESTIONE DELLA "BRUTTA COPIA" (LA TUA COPERTURA)

Un compito consegnato perfetto al 100% con frazioni complesse senza un solo calcolo a matita sulla brutta copia è un **chiaro indizio di copia passiva**.

I docenti controllano la brutta copia per verificare l'autenticità. Fai così:

1. **Scrivi a matita sulla brutta copia i riquadri `[DA SCRIVERE SULLA BRUTTA COPIA]` che l'IA ti fornirà:**
   - **Il sistema 2x2:** Risolvi per sostituzione l'intersezione tra le rette oblique (es. $6x_1 + 3x_2 = 25$ e $x_1 + x_2 = 6$).
   - **Le divisioni del TMR:** Scrivi a mano le frazioni capovolte con le semplificazioni (es. $\frac{11/6}{1/2} = \frac{11}{6} \cdot 2 = \frac{11}{3}$).
   - **I conti del Pivot di II tipo:** Scrivi le sottrazioni con il minimo comune multiplo (es. $-\frac{175}{12} - \frac{77}{12} = -\frac{252}{12} = -21$).
2. **Fai uno schizzo a matita del grafico sulla brutta:**
   - Traccia due assi a croce, metti due punti e unisci le rette prima di fare il disegno pulito sul fascicolo. Questo dimostra che hai "ragionato" prima di disegnare in bella.

---

## 4. I 4 GESTI PRATICI DA COMPIERE SUL FOGLIO (ANCHE SENZA CONOSCERE LA MATERIA)

Anche copiando alla lettera, ci sono 4 gesti pratici che devi compiere fisicamente sul foglio d'esame:

1. **Tracciare una retta:** Se l'IA ti dice *"unisci (4.17, 0) con (0, 8.33)"*, $(4.17, 0)$ si trova sull'asse orizzontale $x_1$ poco dopo il 4; $(0, 8.33)$ si trova sull'asse verticale $x_2$ poco sopra l'8. Metti il righello tra i due punti e tira la riga.
2. **Capire dove campire (frecce dei semipiani):**
   - Se il vincolo è $\le$, il semipiano va verso l'origine $(0, 0)$ (fai 2 o 3 freccette verso il basso/sinistra lungo la retta).
   - Se il vincolo è $\ge$, il semipiano va lontano dall'origine.
   - L'area da colorare a matita è la parte comune a tutti i semipiani nel primo quadrante (in alto a destra).
3. **Compilare le caselle (a), (b), (c), (d), (e):** Nel tableau del simplesso non farti prendere dal panico: il prompt ti scriverà esattamente la riga `(a) BFS: ...`, `(b) Valore F.O.: ...`. Tu devi solo cercare la lettera corrispondente stampata sul foglio e scriverci accanto quello che leggi.
4. **Disegnare l'albero del Branch & Bound:** È un disegno ad albero capovolto: il nodo $P$ è in alto al centro. Se l'IA dice *"ramo sinistro $x_1 \le 1$"*, tiri una riga verso il basso a sinistra, scrivi sopra la riga $x_1 \le 1$ e disegni un cerchio $P_1$ in fondo.

---

## 5. ERRORI FATALI DI TRASCRIZIONE DA EVITARE

Nell'ansia di ricopiare velocemente, fai estrema attenzione a non commettere questi errori tipici:

1. **NON copiare la formattazione Markdown:**
   - Non scrivere gli asterischi del grassetto (es. scrivi `21`, MAI `**21**`).
   - Non copiare le parentesi quadre delle spiegazioni (es. scrivi `x3`, MAI `[x3]`).
2. **NON copiare le parole di istruzione:**
   - Se l'IA scrive: *"Unisci il punto (4.17, 0) con (0, 8.33)"*, NON devi scrivere sul foglio la frase "Unisci il punto...". Devi solo tracciare la linea tra quei punti con il righello.
   - Se scrive *"Frase obbligatoria sull'origine: ..."*, copia solo la frase tra virgolette, non l'etichetta.
3. **Occhio ai Segni Meno:**
   - Nel tableau del simplesso, la colonna $z$ ha sempre **$-1$**.
   - Il termine noto $TN$ della riga zero è l'opposto del valore della funzione obiettivo (es. se $z = 21$, nel tableau c'è scritto **$-21$**).
4. **Frazioni vs Decimali:**
   - Se la docente lascia spazio per le frazioni, scrivi la frazione esatta (es. $\frac{25}{6}$ o $\frac{7}{3}$).
   - Scrivi il decimale (es. $\approx 4.17$) solo tra parentesi o dove serve per posizionare il punto sul righello.

---

## 6. COMPORTAMENTO E POSTURA IN AULA

I docenti e i tutor che sorvegliano gli esami non guardano cosa scrivi, **guardano come ti muovi**:

- **La regola del ritmo continuo:** Non guardare sotto per 30 secondi per poi scrivere a raffica per 1 minuto. Alterna: leggi 2 numeri, scrivi sulla brutta copia, guarda il foglio, poi ricopia in bella. Il movimento deve sembrare quello di uno studente concentrato sui conti.
- **La posizione del corpo:** Non piegare il busto in avanti a 90° con la testa incassata verso le ginocchia. Tieni la schiena rilassata e il foglio di brutta copia leggermente spinto in avanti sul banco per creare una barriera visiva naturale.
- **Attenzione ai passi da dietro:** Durante l'esonero, i sorveglianti camminano lungo i corridoi tra le file di banchi. Se senti passi avvicinarsi alle tue spalle, posa la penna sulla brutta copia e fissa il foglio come se stessi riflettendo.

---

## 7. AUTODIFESA: LE 4 RISPOSTE A MEMORIA

Se alla consegna la docente dovesse sfogliare il foglio e farti una domanda al volo su cosa hai scritto, rispondi con queste parole chiave:

1. **"Come hai scelto la variabile entrante?"**  
   $\to$ *"In un problema di massimo, entra in base la variabile fuori base con il coefficiente positivo più alto nella riga della funzione obiettivo."*
2. **"Come hai scelto la variabile uscente?"**  
   $\to$ *"Ho applicato il TMR (Test del Minimo Rapporto): rapporto tra termini noti positivi e coefficienti positivi della colonna pivot, scegliendo il minimo positivo."*
3. **"Perché il tableau finale è ottimo?"**  
   $\to$ *"Tutti i coefficienti della riga zero (costi ridotti) sono minori o uguali a zero."*
4. **"Come hai scelto la variabile di branching nel Branch & Bound?"**  
   $\to$ *"Ho scelto la variabile meno frazionaria, cioè quella con distanza minima dall'intero più vicino."*
