# Handoff

Stato al 2026-11-01. Branch di lavoro: `claude/skills-plugins-coding-hru1gv` (repo `Atrebg/Prova`).

## Obiettivo dell'utente
Lavorare ai propri progetti **solo dal telefono** (sessioni Claude Code nel cloud), con buone pratiche di codice, e fare pulizia dei repository GitHub vecchi.

## Fatto
- Aggiunto `CLAUDE.md` (regole di qualità: lingua, test, git, review finale) e pubblicato sul branch. Nessuna PR aperta.
- Cercato skill e plugin: nessuna skill di coding era già attiva e `ListPlugins` risultava vuoto.
- Plugin proposti tramite card di installazione (l'utente **non ha visto il pulsante** dal telefono, quindi non risultano attivati):
  - Engineering (Anthropic)
  - code-review (Anthropic)
  - coding-agent-skills (community)
  - coding-skills (community)
- Esaminati i 58 repo visibili sull'account. `lezione1` controllato: modello JavaFX del Politecnico, un solo commit del 2020 ("inutile").
- Controllato Remote Control: nessun computer collegato (`list_computer_folders` vuoto).

## Bloccato / non fattibile da questa sessione
- **Eliminare repository**: nessuno strumento disponibile. Va fatto dall'utente su github.com (repo, Settings, Danger Zone, Delete) o con `gh repo delete` da un Mac autenticato.
- **Attivare i plugin**: avviene fuori dalla sessione (card nell'app o catalogo dell'account, forse serve un amministratore). Il comando `/plugin` esiste solo nel terminale locale.
- **Mac**: l'utente dice di averlo configurato, ma non risulta collegato. Possibili cause: spento, app chiusa, altro account, cartella non condivisa.

## Decisioni dell'utente sulla pulizia
Da **eliminare (43)**:
- Università (35): `lezione1` e i 34 fork Java: `Lab01`–`Lab11`, `2017-06-07`, `2017-06-07-simulazione_SerieA_JDK11`, `2018-01-22_SerieA_JDK11`, `2019-01-24_ExtFlightDelays_JDK11`, `2019-06-05-simulazione-JDK11`, `2019-06-27-A-JDK11`, `2019-06-27-C-JDK11`, `2019-07-12-A-JDK11`, `2019-07-12_FoodPyramidMod_JDK11`, `2019-09-03-JDK11`, `2020-01-20-JDK11`, `2020-06-03-simulazione`, `2020-06-10-simulazione`, `Emergency`, `GestioneMigrazioni`, `GestoreCorsi`, `EsempioSQL`, `IndovinaNumero`, `LibrettoVoti`, `MetroParis`, `NoleggioAuto`, `VotiNobel`, `babs`.
- Fork di tutorial (8): `Flask-Web-App-Tutorial`, `microblog`, `carmanager`, `NFT-Marketplace-Tutorial`, `marketplace-v1`, `polito-projects-TeamPicks`, `Edesia-Project-InformationSystem`, `sito_pwr_2019`.

Tutti sotto `github.com/Atrebg/<nome>`.

**Da tenere (account Atrebg)**: `Prova`, `prenotazioni_olimpo`, `mida_mens_saloon`, `the-flow-event-finance`, `block_puzzle_rl`, `NFTMarketplace`, `marketplace`, `marketplace-clever`, `clash_royale_RL`, `SmartC`, `unitask`, `pythonProject1`.

**Di altri account, non toccare**: `gabrielee5/bot`, `Michele2399/the-flow-event-finance`. Per `emanuelaallocca/dintorni_new` l'utente può solo togliersi dai collaboratori (Settings, Collaborators).

Nota: "NFT Marketplace" è stato interpretato come `NFTMarketplace` (tenuto), non `NFT-Marketplace-Tutorial` (da eliminare). Da confermare.

## Prossimi passi
1. Opzionale: checklist con link diretti ai 43 repo da eliminare dal browser del telefono.
2. Riprovare ad attivare i plugin, poi `ListPlugins` per verificare.
3. Compilare la sezione "Specifiche del progetto" di `CLAUDE.md` quando lo stack è scelto, e copiarlo nei repo delle due app (`prenotazioni_olimpo`, `mida_mens_saloon`).
4. Se il Mac risulta collegato: `list_computer_folders` e `request_computer_folder`.
