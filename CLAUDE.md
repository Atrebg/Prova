# CLAUDE.md

Regole per lavorare su questo repository. Valgono per ogni sessione, anche da telefono.

## Lingua
- Rispondi in italiano.
- Codice, nomi di variabili, commit e commenti tecnici in inglese.

## Prima di scrivere codice
- Leggi il codice esistente e segui le convenzioni già presenti (stile, naming, struttura cartelle).
- Se il progetto ha un README o una documentazione, leggila prima.
- Se la richiesta è ambigua, scegli l'interpretazione più probabile e dichiarala a fine lavoro.
- Non aggiungere dipendenze senza motivo; se servono, spiega perché.

## Qualità del codice
- Funzioni piccole, con una sola responsabilità e nomi chiari.
- Niente codice morto, commenti ovvi o duplicazioni: riusa ciò che esiste.
- Gestisci gli errori in modo esplicito. Non ingoiare eccezioni e non lasciare `TODO` senza motivo.
- Valida l'input ai confini del sistema (utente, rete, file); all'interno fidati dei tipi.
- Mai segreti, token o password nel codice o nei commit.
- Sicurezza: attenzione a injection, XSS, path traversal e dati sensibili nei log.

## Test
- Ogni funzionalità nuova o bug fix ha un test. Per un bug, scrivi prima il test che lo riproduce.
- Esegui i test e il linter prima di dichiarare il lavoro finito.
- Se non riesci a eseguire i test, dillo chiaramente invece di affermare che funziona.

## Git
- Lavora sul branch indicato per la sessione; non fare push su altri branch.
- Commit piccoli e focalizzati, con messaggio chiaro (`tipo: descrizione breve`, es. `fix: handle empty input`).
- Non creare pull request se non richiesto esplicitamente.
- Non riscrivere la storia di branch già pubblicati.

## Review prima di chiudere
Prima di consegnare, rileggi il diff e controlla:
1. Fa solo ciò che era stato chiesto?
2. Casi limite e errori gestiti?
3. Test e linter passano?
4. Niente file temporanei o di debug rimasti?

## Comunicazione
- A fine lavoro riassumi cosa hai cambiato, cosa hai verificato e cosa resta aperto.
- Se qualcosa è bloccato o fallisce, dillo per primo, con l'output dell'errore.

## Specifiche del progetto
<!-- Compila quando il progetto prende forma -->
- Linguaggio / framework:
- Comando per installare le dipendenze:
- Comando per i test:
- Comando per il linter:
- Comando per avviare l'app:
