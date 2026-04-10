# Codice sconto Trainline, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Trainline** da [shopilo.it](https://shopilo.it/negozi/thetrainline.com). Restituisce **coupon Trainline** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-trainline](https://shopilo-it.github.io/codice-sconto-trainline/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-trainline
cd codice-sconto-trainline
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Trainline",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su biglietti treno e bus",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/thetrainline.com"
  }
]
```

## Coupon Trainline disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su biglietti treno e bus | [shopilo.it](https://shopilo.it/negozi/thetrainline.com) |

Codici attivi: **[shopilo.it/negozi/thetrainline.com](https://shopilo.it/negozi/thetrainline.com)**

## Domande frequenti

### Come utilizzo un codice sconto Trainline?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/thetrainline.com), aggiungi i prodotti al carrello su Trainline e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Trainline?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Trainline piu recenti?
La pagina [shopilo.it/negozi/thetrainline.com](https://shopilo.it/negozi/thetrainline.com) viene aggiornata quotidianamente con i codici sconto Trainline, voucher Trainline e coupon promozionali Trainline piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Trainline

Trainline e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/thetrainline.com) trovi i migliori codici sconto Trainline, coupon Trainline verificati e voucher Trainline attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-trainline
```

```javascript
const { fetchCoupons } = require('codice-sconto-trainline');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
