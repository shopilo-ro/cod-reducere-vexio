# Cod reducere Vexio — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Vexio** de pe [shopilo.ro](https://shopilo.ro/magazin/vexio.ro). Returneaza **cupoane Vexio** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-vexio](https://shopilo-ro.github.io/cod-reducere-vexio/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-vexio
cd cod-reducere-vexio
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Vexio",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la accesorii si gadgeturi",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/vexio.ro"
  }
]
```

## Cupoane Vexio disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la accesorii si gadgeturi | [shopilo.ro](https://shopilo.ro/magazin/vexio.ro) |

Codurile active: **[shopilo.ro/magazin/vexio.ro](https://shopilo.ro/magazin/vexio.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Vexio?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/vexio.ro), adauga produsele in cos pe Vexio, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Vexio?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Vexio?
Pagina [shopilo.ro/magazin/vexio.ro](https://shopilo.ro/magazin/vexio.ro) este actualizata zilnic cu cele mai noi cod reducere Vexio, voucher Vexio si cupon promotional Vexio.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Vexio

Vexio este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/vexio.ro) cele mai bune cod reducere Vexio, cupoane Vexio verificate si voucher Vexio active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-vexio
```

```javascript
const { fetchCoupons } = require('cod-reducere-vexio');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
