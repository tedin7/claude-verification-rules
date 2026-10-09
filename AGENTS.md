# Istruzioni per gli agenti

## Chiarezza delle risposte — adattamento ASD-STE100

Applica questi criteri alle risposte, anche in italiano. Sono un adattamento
conversazionale di ASD-STE100 Issue 9, non una dichiarazione di conformità al
vocabolario inglese controllato. Conserva identificatori tecnici e dettagli necessari.

- Presenta prima il risultato e il limite che ne cambia il significato, poi le
  prove e il passo successivo (6.1–6.2). Un risultato parziale va dichiarato subito.
- Usa nomi semplici e coerenti. Spiega sigle e termini interni al primo uso
  pertinente; conserva il nome tecnico per identificarli (1.9–1.11, 9.4).
- Preferisci soggetto esplicito, forma attiva e verbi concreti. Indica chi ha
  fatto cosa; sostituisci formule vaghe con la causa osservata (3.6–3.7).
- Scrivi frasi brevi: punta a 20 parole nelle istruzioni e 25 nelle spiegazioni
  (4.1, 5.1, 6.3). Non troncare comandi, nomi o condizioni per rispettare il numero.
- Mantieni un argomento per paragrafo. Separa risultato, prove e blocchi quando
  mescolarli rende difficile capire lo stato (6.4–6.6).
- Nelle procedure, indica prima le condizioni e poi un'azione per frase.
  Usa l'imperativo per le azioni richieste all'utente (5.2–5.4).
- Usa elenchi per passi o casi distinti e connettivi per causa e conseguenza
  (4.3–4.4). Non comprimere tutto in una frase con molte clausole.
- Rileggi dal punto di vista dell'utente: chiarisci riferimenti ambigui senza
  eliminare informazioni necessarie. Se serve, riscrivi la frase (4.2, 9.1).

Fonte: [ASD-STE100, Issue 9](https://www.asd-ste100.org/assets/files/ASD-STE100_ISSUE9.pdf).
Criteri selezionati su 10 sessioni interattive campionate il 2 ottobre 2026.

## Falsificazione prima del rilascio (regola costante)

Ordine dell'operatore del 2026-10-09. Prima di mettere online un cambiamento di
comportamento, un agente o una sessione **diversa da chi l'ha scritto** prova a
farlo sbagliare: casi di bordo, raffiche e carico, dati malformati o privati,
versioni e formati simili, strumenti e chiamanti esistenti, ripristino e
riavvio, permessi. Lavora su copie o in isolamento, mai sulla produzione, e
riporta per ogni punto "passa" o "fallisce" con la prova.

- I test verdi e le prove dell'autore non bastano: controllano solo ciò che
  l'autore ha pensato.
- Si rilascia solo con i difetti gravi corretti, ognuno con un test che
  fallisce prima e passa dopo, e con la falsificazione ripetuta su quella
  versione.
- Una modifica senza effetto sul comportamento (testo, documentazione) è
  esclusa.
- Nel resoconto distingui "provato dall'autore" da "falsificazione
  indipendente superata".
