# Code promo Micromania, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Micromania** depuis [shopilo.fr](https://shopilo.fr/reductions/micromania.fr). Renvoie les **coupons Micromania** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-micromania](https://shopilo-fr.github.io/code-promo-micromania/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-micromania
cd code-promo-micromania
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Micromania",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur les jeux video et consoles",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/micromania.fr"
  }
]
```

## Coupons Micromania disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur les jeux video et consoles | [shopilo.fr](https://shopilo.fr/reductions/micromania.fr) |

Codes actifs : **[shopilo.fr/reductions/micromania.fr](https://shopilo.fr/reductions/micromania.fr)**

## Questions frequentes

### Comment utiliser un code promo Micromania ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/micromania.fr), ajoutez les produits a votre panier sur Micromania et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Micromania ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Micromania les plus recents ?
La page [shopilo.fr/reductions/micromania.fr](https://shopilo.fr/reductions/micromania.fr) est mise a jour quotidiennement avec les codes promo Micromania, bons de reduction Micromania et coupons promotionnels Micromania les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Micromania

Micromania est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/micromania.fr), retrouvez les meilleurs codes promo Micromania, coupons Micromania verifies et bons de reduction Micromania actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-micromania
```

```javascript
const { fetchCoupons } = require('code-promo-micromania');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
