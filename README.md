# Clear Path · Clearwater

A free map of downtown Clearwater, Florida that shows which properties are owned by the Church of Scientology or by companies that public records and news reporting tie to it. It is meant for anyone who wants to visit, shop or eat downtown without that money going to the church or its members' companies.

## How to view it

**Just open this link on your phone or computer:**

### 👉 https://mrkiwisir.github.io/Clear-Path-Clearwater/

Nothing to install and no account needed. On a phone, use your browser's **Add to Home screen** to keep it like an app.

You can also open the **research summary** (tables of every flagged property, with sources):
https://mrkiwisir.github.io/Clear-Path-Clearwater/research.html

### Using the map

| What you see | What it means |
|---|---|
| 🟥 Red shading | The owner of record is a Church of Scientology entity. |
| 🟧 Orange shading | Owned by an LLC whose state filings name a person or company that news reporting identifies as a Scientology parishioner buyer. |
| 🟨 Yellow shading *(hidden by default)* | An unverified lead: the owner shares only a mailing address or manager with a linked company. Turn these on in **Key & data**. They may be wrong. |
| 🟣 Purple dot | A public comment about a place (unvetted; hide with 💬). |
| 🟢 Green dot | A business whose building has **no ownership link found** in these sources. See the note below. |
| 🟠 / 🔴 dot | A business whose landlord is in an orange or red group. |
| ⚪ Gray dot | A business on an unverified (yellow) lead parcel. |

- **Tap** any shaded property or dot to see the owner and the evidence, with links to the sources.
- **Clean picks** tab: nearby businesses with no link found, closest first. Filter by type.
- **Route** tab: walking directions. With *Avoid walking past flagged property* on, the route goes around flagged buildings. The shortest route is shown dashed for comparison.
- **📍 Me** centers the map on you. **Scan area** loads businesses wherever the map is currently showing.
- **Mark OK / Mark avoid** on a business saves your own note **on your device only**.

## Why the green dots look random

Green dots are **not hand-picked recommendations**. They are every business that volunteers have added to [OpenStreetMap](https://www.openstreetmap.org) in the area shown, where the building's owner has no link in the data below. OpenStreetMap coverage in downtown Clearwater is patchy. Some blocks are mapped in detail and others not at all, so the green set looks uneven, and many real storefronts don't appear.

"No link found" is **not proof** that a business or its landlord is independent. It only means nothing in these sources connects them.

**Help fill the gaps:** add missing businesses to OpenStreetMap (for example with the free [StreetComplete](https://streetcomplete.app) or [Every Door](https://every-door.app) apps). They appear in Clear Path automatically, usually within a day.

## Share what you know

Anyone can add what they know about a building or business, and it shows up on the map **right away**.

1. On the map, tap a property or business and choose **✍️ Add info**. A short form opens with the address and location already filled in. You can also [post a comment directly](https://github.com/MrKiwiSir/Clear-Path-Clearwater/issues/new?template=ownership-tip.yml). You need a free GitHub account.
2. Say what you know. A source is optional, and word of mouth is welcome. Just say how you know.
3. Your comment appears on the map immediately, inside that property's popup or as a **purple dot**, and on the [comments page](https://github.com/MrKiwiSir/Clear-Path-Clearwater/issues?q=is%3Aopen+label%3Atip), where anyone can read it and reply.

Public comments are **unvetted**. Map users can hide them with the **💬 On/Off** button at the top of the map.

Please leave out private details like home addresses and phone numbers. The maintainer removes spam or comments like that by adding the `hidden` label.

## Where the information comes from

- **Property ownership:** loaded **live** each time the map opens from the [Pinellas County Property Appraiser](https://www.pcpao.gov) public parcel service. Sales and ownership changes show up without anyone updating the app.
- **Who runs each LLC:** [Florida Division of Corporations (Sunbiz)](https://search.sunbiz.org) public filings. Florida records managers and agents, not the true owners.
- **Which people and companies are linked:** published reporting, mainly the Tampa Bay Times investigation [*Clear Takeover* (2019)](https://projects.tampabay.com/projects/2019/investigations/scientology-clearwater-real-estate/) and follow-ups from 2018, 2020, 2021 and 2024, plus WUSF (2026). Each group in the app links to its sources.
- **Businesses and streets:** © OpenStreetMap contributors, used under the [ODbL](https://opendatacommons.org/licenses/odbl/).

The rules that decide what gets flagged are listed in plain text near the top of `index.html` (the `GROUPS` list). Anyone can read or check them.

## Accuracy and limits

- This is an independent, unofficial project. It is not affiliated with the Tampa Bay Times, Pinellas County or anyone named in the data.
- Every flag rests on public records and published reporting, and the sources are linked. Ownership changes, LLCs hide their real owners, and records can be wrong. **Check before relying on any single entry.**
- Walking past a building costs nothing. The routing option is there for people who simply prefer not to.
- Found an error? Tap **✍️ Add info** on the map, or [post a comment](https://github.com/MrKiwiSir/Clear-Path-Clearwater/issues/new?template=ownership-tip.yml).

## Files

| File | What it is |
|---|---|
| `index.html` | The map app (one self-contained page) |
| `research.html` | Research summary from November 2026: every flagged parcel, ownership groups and evidence |
| `data/flagged_parcels_2026-11.csv` | Snapshot of flagged parcels (tier, group, owner of record, address, parcel ID, coordinates) |
| `data/businesses_2026-11.csv` | Snapshot of OpenStreetMap businesses matched to their landlord's tier (ODbL) |
| `.github/ISSUE_TEMPLATE/` | The public comment form |

The CSV files are a dated snapshot. The live map is always more current.

## License

- **Code and research** (`index.html`, `research.html`, this README): [PolyForm Noncommercial 1.0.0](LICENSE.md). Free for personal, research, educational and nonprofit use. **Commercial use requires permission**; ask by opening an issue.
- **`data/businesses_2026-11.csv`** comes from OpenStreetMap and is under the [Open Database License](https://opendatacommons.org/licenses/odbl/1-0/). See [`data/README.md`](data/README.md).
- **Parcel ownership data** is public record from the Pinellas County Property Appraiser.
- Map tiles and business data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright).
