# Ismailia Fresh — Cold Storage Inventory (Demo)

نسخة تجريبية من نظام مخزون تلاجات التخزين لمصنع **عين إسماعيلية فريش**.
A demo of a cold-storage inventory system for the Ismailia Fresh juice factory.

> ⚠️ **Demo only.** Data is fake and saved in each visitor's browser (localStorage). The production version will use a real database, hosting, domain, and secure user accounts.

## Demo accounts

| User | Password | Role |
|---|---|---|
| `admin` | `1234` | Admin — full access, settings, activity log |
| `ahmed` | `1234` | Storekeeper — stock in, withdraw, CSV import |
| `mahmoud` | `1234` | Field rep — view only |

## Features

- Products with sizes in **kg / liter / ton**
- Cold stores with owner, location, and allocated capacity (load bar)
- Every batch tracked separately: production code, production / entry / expiry dates
- **FEFO / FIFO** withdrawal order (setting)
- **Auto withdraw**: enter a quantity (packs or kg) and it's split across batches in the right order
- Warning + required reason when withdrawing out of order
- Expiry status colors and shelf-life progress per batch
- **Production code trace**: see where a production run is distributed
- CSV import with preview and validation; CSV export (Excel-friendly Arabic)
- Map of all cold stores (OpenStreetMap)
- Dashboard, movements log, and per-user **activity log**
- Arabic / English interface

## Run / deploy

It's a single static `index.html` — no build step.

**GitHub Pages:** Settings → Pages → Source: `Deploy from a branch` → Branch: `main` / `(root)` → Save.
The site will be at `https://<username>.github.io/<repo>/`.

To reset the demo data, sign in as `admin` and click **Reset demo data**.

---
Developed by **Omar Semida**
