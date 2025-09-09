# EUR/GBP → USD with historical rates (my first Jupyter)

I took a small purchases dataset in **EUR** and **GBP** and converted everything to **USD** using **historical** FX from VATComply.  
I left the notebook **intentionally messy** so you can see where I broke things and how I fixed them—false starts, comments, and all.

## What I did
- Loaded purchases into pandas (`amount`, `currency`).
- Pulled **historical** FX for a specific date from **VATComply**.
- Added `exchange_rate` and computed `amount_usd`.
- Exported two files:
  - `output.csv` — first pass  
  - `rates_converted.csv` — same data, but with fixed decimals for readability

## What went wrong & how I fixed it
- Tried looping rows → hit a `TypeError` indexing strings; switched to **vectorized** pandas (`.loc` / `.map`).
- Decimal formatting looked messy → added fixed precision in the final export.

