# Codice sconto Itabus, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Itabus** da [shopilo.it](https://shopilo.it/negozi/itabus.it). Restituisce **coupon Itabus** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-itabus](https://shopilo-it.github.io/codice-sconto-itabus/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-itabus
cd codice-sconto-itabus
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Itabus",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su viaggi in autobus Italia",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/itabus.it"
  }
]
```

## Coupon Itabus disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su viaggi in autobus Italia | [shopilo.it](https://shopilo.it/negozi/itabus.it) |

Codici attivi: **[shopilo.it/negozi/itabus.it](https://shopilo.it/negozi/itabus.it)**

## Domande frequenti

### Come utilizzo un codice sconto Itabus?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/itabus.it), aggiungi i prodotti al carrello su Itabus e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Itabus?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Itabus piu recenti?
La pagina [shopilo.it/negozi/itabus.it](https://shopilo.it/negozi/itabus.it) viene aggiornata quotidianamente con i codici sconto Itabus, voucher Itabus e coupon promozionali Itabus piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Itabus

Itabus e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/itabus.it) trovi i migliori codici sconto Itabus, coupon Itabus verificati e voucher Itabus attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-itabus
```

```javascript
const { fetchCoupons } = require('codice-sconto-itabus');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
