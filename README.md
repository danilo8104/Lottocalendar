# Calendari Estrazioni Lotto

Questa cartella contiene i calendari ufficiali e provvisori delle estrazioni del Lotto.

## Struttura
- calendar_YYYY.json → eccezioni annuali alle estrazioni standard
- calendar_version.json → versione e metadati

## Regole di calcolo
- Schema base: Martedì, Giovedì, Venerdì, Sabato ore 20:00
- Le date presenti nei file JSON **sovrascrivono** lo schema base
- `status: ufficiale` → determinazione ADM pubblicata
- `status: provvisorio` → previsione coerente con anni precedenti, da confermare

## Uso in App
- Il motore genera il calendario base
- Applica gli override dell’anno corrente
- Espone:
  - prossima estrazione reale
  - orario
  - nota festività (se presente)

Aggiornare i file quando ADM pubblica nuove determinazioni.
