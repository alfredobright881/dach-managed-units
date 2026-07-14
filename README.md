# How many professionally-managed homes are there in DACH?

A bottom-up, fully-sourced estimate of professionally-managed (third-party-administered) dwellings in
Germany, Austria and Switzerland, plus a separate lower-confidence commercial layer.

**Answer: ~15 million professionally-managed residential dwellings (central case), in a defensible
range of ~11M to ~19M, on a hard ~11.4M floor that needs no assumptions at all.**

Everything here is built from public statistics: Zensus 2022 / Destatis, GdW/vdw, Statistik Austria
and the GBV Verbandsstatistik, and the Swiss BFS. Every figure carries its source URL. Every
assumption is stated as an assumption.

I built this because I needed the number for my own work and could not find an honest version of it.
The figure most often repeated in this market is ~20M. When I sourced it properly, the number came out
lower, so this is the lower number, with the workings. The uncertainty section at the bottom says
plainly which single assumption drives most of the error, and it is not a small one.

Corrections and better sources are welcome. Open an issue.

*Compiled 2026-07-10, commercial layer added 2026-07-11. Richard Dolmetsch.*
*Licensed CC BY 4.0. Cite it, fork it, correct it.*

---

*Residential is the census-anchored core. Commercial was added as a separate, lower-confidence modeled
layer, see "Commercial Hauptobjekte" below.*

**Bottom line: ~15 million professionally-managed residential dwellings in DACH (central case),
in a defensible range of ~11M (low) to ~19M (high).** The ~20M figure commonly cited in this market
sits at or above the *top* of the independently-sourced range, not at the centre.

**Commercial adds a separate, lower-confidence ~1.5M (range ~1.0–2.5M)**, see the *Commercial
Hauptobjekte* section below. It is *modeled*, not census-grade, and materially larger by value than by
unit count. Residential + commercial → **~16.5M DACH Hauptobjekte central (range ~12–21M).**

Every unit below counts **dwellings (Wohnungen)**: apartments and (where noted) commercial Lokale.
Dwellings are already the primary lettable unit, so they map to **residential Hauptobjekte**.
Parking bays and storage (Nebenobjekte) are *not* in any dwelling count. Where a source lets us see
the split, it confirms this: Austria's GBV reports 1,006,700 **Wohnungen** separately from 483,030
**Garagen**. We count the former, drop the latter.

"Professionally managed" here = administered by a professional management operation (Hausverwaltung,
Bewirtschafter, Wohnungsunternehmen, Genossenschaft, municipal housing company), whether the manager
owns the asset or runs it for a third party. It **excludes** the private owner who self-administers a
handful of units. That exclusion is the whole exercise; total dwellings (52.9M across DACH) is the
easy number and the wrong one.

---

## Summary table

| Country | Total dwellings | Rental dwellings | Professionally managed (central) | Prof.-managed range | Confidence | Key sources (year) |
|---|---|---|---|---|---|---|
| **Germany** | ~43.1M *(dwellings)* | ~23–25M *(rental dwellings)* | **~12M** | ~9.1–15M | Med (floor High; private-outsourcing share Low) | Zensus 2022 / Destatis; GdW/vdw *Wohnungswirtschaftliche Daten u. Trends 2024/25*; Haus & Grund *Wohnen in Zahlen 2025/26*; IW Köln 2025 |
| **Austria** | ~4.91M *(dwellings, GWZ 2021)* | ~1.77M *(main-residence rental, 2023)* | **~1.3M** | ~1.0–1.6M | Med-High (GBV floor is hard-sourced) | Statistik Austria GWZ 2021 & *Wohnen 2023*; GBV Verbandsstatistik 2024 (data 2023) |
| **Switzerland** | ~4.84M *(dwellings, 2024)* | ~2.4M *(rental dwellings)* | **~1.7M** | ~1.3–1.9M | Med-High (managed share of rental is high & well-attested) | BFS Gebäude- u. Wohnungsstatistik 2024; BFS Mieter/Eigentümer & Mietwohnungen (2019–2024) |
| **DACH total** | **~52.9M** | **~27M** | **~15M** | **~11–19M** | — | — |

---

## Low / central / high (professionally-managed residential dwellings)

| Case | Germany | Austria | Switzerland | **DACH total** |
|---|---|---|---|---|
| **Low** | ~9.1M | ~1.0M | ~1.3M | **~11.4M** |
| **Central** | ~12M | ~1.3M | ~1.7M | **~15M** |
| **High** | ~15M | ~1.6M | ~1.9M | **~18.5M** |

**Headline: ~15M central, ~11–19M range.** (A parallel automated research pass put the
central band slightly wider at ~13–18M and a broad-case high at ~24M. The difference is entirely
whether condominium/WEG *building* administration is counted; see the uncertainty note.)

---

## Germany — the swing factor

- **Total dwellings ~43.1M** (Zensus 2022, reference date 15.05.2022; ≈ stock update 31.12.2021 of
  43.08M). Source: Statistisches Bundesamt, Zensus 2022 —
  https://www.destatis.de/DE/Themen/Gesellschaft-Umwelt/Bevoelkerung/Zensus2022/_inhalt.html ;
  vacancy PM (4.3% leer, confirms ~1.9M vacant of ~43M) —
  https://www.destatis.de/DE/Presse/Pressemitteilungen/Zensus2022-Pressemitteilungen/PM_zenus2022_46.html
- **Rental dwellings ~23M** (Zensus 2022: "rund 23 Millionen Wohnungen von verschiedenen
  Eigentümertypen vermietet"; some derivations put it at ~25.0M when a wider rental definition is
  used). This counts **rental dwellings**.
- **Ownership of the rental stock** (Zensus 2022, via Haus & Grund *Wohnen in Zahlen 2025/2026*):
  - Privatpersonen (private small landlords): **63.5%** (~14.6M) — https://www.hausundgrund.de/sites/default/files/downloads/250320hausgrundbroschuerewohneninzahlenweb.pdf
  - Privatwirtschaft (private commercial housing companies): **14.33%** (~3.3M)
  - Genossenschaften (cooperatives): **11.66%** (~2.7M)
  - Kommune/Bund/Land (municipal/state/federal): **9.03%** (~2.1M)
  - Organisation ohne Erwerbszweck (non-profit): **1.49%** (~0.34M)
- **Hard floor — a directly-cited *management* figure, not an ownership residual: 9.1M dwellings.**
  GdW/vdw (*Wohnungswirtschaftliche Daten und Trends 2024/25*): *"Professionell-gewerbliche Anbieter
  bewirtschaften in Deutschland 9,1 Mio. Wohnungen … 36 % des Mietwohnungsbestandes."* i.e. housing
  companies, cooperatives, municipal and listed providers **actively manage 9.1M dwellings = 36% of
  the rental stock.** Source: https://www.vdwbayern.de/wp-content/uploads/2024/12/Wohnungswirtschaftliche-Daten-und-Trends-20242025.pdf
  — This is the strongest single German number: it says *bewirtschaften* (manage), not just *own*.
  Cross-checks: the ~36.5% professional/institutional *ownership* residual from the Vermietergruppen
  split ≈ ~8.4M (consistent); GdW's own member companies alone manage 6.0M ≈ 30% of rental
  (https://www.gdw.de/die-wohnungswirtschaft/), sitting inside the 9.1M.
- **The swing above the floor:** how much of the **16.1M** privately-owned rental stock (IW Köln 2025,
  *Private Vermieter in Deutschland*; 5.2M private landlords, avg ~3 units each) is run by a
  third-party Hausverwaltung rather than self-managed —
  https://www.iwkoeln.de/fileadmin/user_upload/Studien/Gutachten/PDF/2025/Gutachten-Private-Vermieter-in-Deutschland.pdf
  German small landlords predominantly self-manage (the IW study frames many as *not* professionally
  organised), but ~40% of their units are condos inside a WEG (professionally administered *building*),
  and a minority outsource letting. Assumed third-party-managed share **15–35% → +2.4–5.6M**, net of
  overlap. (These privately-owned units are *not* inside the 9.1M, so adding them does not double-count.)
- **Context on the management industry:** Destatis counted **24,066** property-management firms (2018;
  >30,000 by 2023) with €11B+ turnover —
  https://www.destatis.de/DE/Presse/Pressemitteilungen/2019/09/PD19_370_31.html . Germany also has
  ~9.3M condominium dwellings in WEG, most with a professional Verwalter, an *adjacent* pool
  (building administration, not letting) that overlaps both owner-occupied and rented stock and is
  **deliberately not added in**. A parallel research pass tried to map that ~9.28M WEG bucket to
  "always professionally administered" and it was **adversarially refuted (0–3 vote)** on
  buildings-vs-units and self-management grounds, which is exactly why counting WEG would inflate
  the total toward/past 20M on a double-count, and why the high case here stops at ~15M for Germany.
- **Germany professionally-managed rental dwellings: Low ~9.1M · Central ~12M · High ~15M.**

## Austria — GBV gives a hard floor

- **Total dwellings ~4.91M** (Gebäude- u. Wohnungszählung, register census 31.10.2021, published
  Sept 2023); ~4.02M are main-residence dwellings. Source: Statistik Austria —
  https://www.statistik.at/statistiken/bevoelkerung-und-soziales/wohnen/wohnungsbestand ;
  GWZ 2021 — https://www.statistik.at/fileadmin/announcement/2023/09/20230919GWZ2021.pdf
- **Main-residence rental dwellings ~1.77M** (2023). Source: Statistik Austria, *Wohnen 2023* —
  https://www.statistik.at/fileadmin/user_upload/Wohnen-2023_Web-barrierefrei.pdf
- **GBV (gemeinnützige Bauvereinigungen) managed = hard floor.** At end-2023 the 182 GBVs managed
  **1,520,600 units**, of which **1,006,700 Wohnungen** (dwellings) + **15,070 Lokale** (commercial)
  + 483,030 Garagen (parking, *excluded* as Nebenobjekte) + 15,780 other. Source: GBV
  Verbandsstatistik 2024 (data year 2023) —
  https://cms.gbv.at/DE/repos/files/GBV/Intranet_downloads/PDF/Verbandsstatistik/GBV%20Verbandsstatistik24.pdf
  (secondary: https://de.wikipedia.org/wiki/Gemeinn%C3%BCtzige_Bauvereinigungen_in_%C3%96sterreich )
  — This ~1.0M dwelling figure is the single cleanest "professionally-managed Hauptobjekte" number in
  all of DACH, because GBV itself already reports a *Verwaltungsbestand* (units under management) and
  splits Wohnungen from Garagen. The prior-year figure (GBV Verbandsstatistik 2023, Stand 31.12.2022)
  is the same shape: 1,492,500 units → 997,590 Wohnungen + 14,660 Lokale (= 1,012,250 Hauptobjekte)
  vs 464,910 Garagen + 15,300 sonstige (Nebenobjekte, excluded).
  https://cms.gbv.at/DE/repos/files/GBV/Intranet_downloads/Intranet_data/Statistik/STAT23%20Publikation.pdf
- **Composition of the GBV-managed dwellings** (end-2022): ~66% the GBV's own rental/cooperative stock,
  ~30% Eigentumswohnungen / WEG condominium administration, ~4% rental owned by others but managed by
  a GBV (pure third-party). So even on the strictest "third-party only" reading, ~34% of the ~1.0M is
  external administration; the rest is a non-profit professionally managing its own stock (still in
  scope per the definition above, which includes cooperatives).
- **Above the GBV floor:** municipal housing, **~276,100 Gemeindewohnungen** (16% of Austrian rental;
  Wiener Wohnen dominates with ~202,500 in Vienna), plus private rental via commercial
  Hausverwaltungen. GBV (40% of rental, ~681,800) + municipal (~276,100) ≈ **958,000 institutionally
  managed rental dwellings** as a social-housing floor. Sources: GBV market analysis + Statistik
  Austria *Wohnen 2023*.
- **Austria professionally-managed dwellings: Low ~1.0M (GBV Verwaltungsbestand) · Central ~1.3M · High ~1.6M.**

## Switzerland — high managed share, small stock

- **Total dwellings 4.84M** (BFS Gebäude- und Wohnungsstatistik 2024) —
  https://www.bfs.admin.ch/news/de/2025-0428
- **Rental dwellings ~2.4M.** BFS (end-2024): **2.5M households rent** vs 1.4M own; tenure split
  **~58% rental / 36% owner-occupied / ~3% cooperative** of households. Source: BFS Mieter/Eigentümer —
  https://www.bfs.admin.ch/bfs/de/home/statistiken/bau-wohnungswesen/wohnungen/wohnverhaeltnisse/mieter-eigentuemer.html
- **Ownership of rental (BFS 2019–2021):** private persons **47%**, institutional investors
  (insurance/pension funds/real-estate funds) **~33%**, other corporations/cooperatives/public **~20%**.
  BFS explicitly notes that **many privately-owned rentals are run by a professional Bewirtschafter**:
  tenants often don't know the owner is a private person because they only ever deal with the manager.
  Sources: BFS Mietwohnungen; SRF —
  https://www.srf.ch/news/schweiz/bfs-wohnungsstatistik-ein-drittel-der-wohnungen-gehoert-institutionellen-anlegern ;
  https://www.watson.ch/schweiz/wirtschaft/297119550-die-haelfte-der-schweizer-mietwohnung-gehoert-einer-privatperson
- **Managed share of rental is high:** institutional (33%) + other corporate/coop/public (~20%) =
  ~53% that is essentially always professionally managed, plus a large slice of the private 47% via
  Bewirtschafter → **~70–80% of rental**. On ~2.4M rental that is ~1.7–1.9M. Independent corroboration
  of the high delegation level: the BWO/pom+ study *Die volkswirtschaftliche Bedeutung der
  Immobilienwirtschaft der Schweiz* reports an **Outsourcinggrad of ~70%** of the Bewirtschaftung
  market (revised to ~74% in later editions), but note this is measured by **CHF value across the
  whole building stock (2014)**, not a residential-dwelling count, so it corroborates the *direction*
  rather than pinning the number.
  https://www.bwo.admin.ch/dam/bwo/de/dokumente/01_Wohnungsmarkt/15_Studien_und_Publikationen/Forschungsberichte/die_volkswirtschaftlichebedeutungderimmobilienwirtschaftderschwe.pdf.download.pdf/die_volkswirtschaftlichebedeutungderimmobilienwirtschaftderschwe.pdf
- **Switzerland professionally-managed rental dwellings: Low ~1.3M (~55%) · Central ~1.7M (~70%) ·
  High ~1.9M (~80%).** (Switzerland is the thinnest-sourced leg. No source gives a CH
  professionally-managed dwelling *count*; a broad reading that most of the ~2.4M rental is managed
  would push the high toward ~2.0M+.)
- **Sanity check ✓** SVIT Online-Wohnungsindex: **~393,900 rental objects advertised Apr 2025–Mar 2026**.
  Against a rental stock of ~2.4M that is a **~16% annual listing rate**, consistent with normal
  Swiss re-letting churn. The Swiss stock figure here is *not* wildly off this benchmark.

---

## Commercial Hauptobjekte — a separate, LOWER-confidence layer (~1.5M DACH)

Everything above is **residential**. Commercial lettable units (offices, shops, gastronomy, practices,
light-industrial/logistics) are a genuinely different measurement problem, and the number below is
**modeled, not census-grade**. Treat it as order-of-magnitude, confidence **LOW**.

**Why it can't be counted like dwellings:** no statistical office counts "lettable commercial units."
Commercial real estate is measured in **floor area (m²)** or **assets-under-management (€)**, and the
nearest unit-like proxy, business establishments (*Arbeitsstätten*), over-counts (home offices, no
premises) and mixes owner-occupied with let. So a Hauptobjekt count must be triangulated, with visible
assumptions, from two directions:

**Method A — floor area ÷ average unit size.** Germany's office stock alone is **382.4M m² across
323,700 office/administrative buildings** (Destatis/BBSR *Nichtwohngebäudebestand*, 2015 —
https://de.statista.com/themen/2537/bueroflaechen/ ; office split by city: 19 markets = 114.5M m² ≈ a
third of the national total). Add retail *Verkaufsfläche* (~120M m², HDE, widely cited) and
light-industrial/logistics. Of that, the **let + professionally-managed** slice (excluding owner-occupied
corporate/SME premises) is roughly ~350–500M m²; at an average commercial unit of ~350–450 m² that is
**~0.9–1.3M units in Germany.**

**Method B — establishments × let-share × managed-share.** Germany had **3.8M business establishments**
(Niederlassungen, Destatis Unternehmensregister 2024 —
https://www.destatis.de/DE/Themen/Branchen-Unternehmen/Unternehmen/Unternehmensregister/_inhalt.html ).
Assume ~45–55% are let rather than owner-occupied, and ~50–65% of those are managed by a third-party
Hausverwaltung/PM → **~0.9–1.3M units.** The two methods converge, which is the only reason I'd put a
number here at all.

| Country | Establishments (proxy) | Prof.-managed let commercial units (central) | Range | Basis |
|---|---|---|---|---|
| **Germany** | ~3.8M (Niederlassungen, 2024) | **~1.1M** | 0.7–1.8M | office 382M m² hard-sourced; let/managed shares assumed |
| **Austria** | ~700k companies / ~0.78M Arbeitsstätten (2021) | **~0.2M** | 0.13–0.30M | Statistik Austria Arbeitsstättenzählung 2021 |
| **Switzerland** | ~637k companies / ~0.7M Arbeitsstätten (2022) | **~0.25M** | 0.15–0.35M | BFS STATENT 2022; high CH management penetration |
| **DACH commercial** | — | **~1.5M** | **~1.0–2.5M** | modeled, confidence LOW |

- Sources for the establishment anchors: Statistik Austria *Arbeitsstättenzählung 2021* (~700k companies)
  https://www.statistik.at/fileadmin/announcement/2023/08/20230814Arbeitsstaettenzaehlung2021.pdf ;
  BFS *STATENT 2022* (~637k companies, ~5.6M employees)
  https://www.bfs.admin.ch/bfs/de/home/statistiken/industrie-dienstleistungen/erhebungen/statent.html
- **No double-count with residential.** The residential ~15M counts **dwellings only**. I explicitly
  dropped the commercial *Lokale* that sit inside residential portfolios (e.g. GBV's 14,660 Lokale were
  *not* added to its 1.0M Wohnungen). So this commercial layer is additive, not overlapping.
- **The count understates commercial's economic weight.** A commercial unit carries roughly 3–10× the
  rent and management fee of a dwelling, so on any per-unit revenue measure commercial is a much larger
  share than of the unit count, plausibly ~20–40% despite being ~10% of units. On a unit-count basis
  it is a ~1.5M footnote; on a revenue basis it deserves its own line.

**DACH grand total (residential + commercial): ~16.5M professionally-managed Hauptobjekte (central),
range ~12–21M**, of which commercial is ~1.5M (~10% by count, materially more by value). The
commercial layer is **LOW confidence** and should be presented as a modeled adjacency, never with the
same weight as the census-anchored residential figure.

---

## What is genuinely uncertain

0. **Commercial is the lowest-confidence part of this whole file.** The ~1.5M commercial figure is a
   model built on assumed let-shares and managed-shares and an assumed average unit size. There is no
   commercial equivalent of the Zensus. Its true range could plausibly be ~1.0–2.5M, and the biggest
   open questions are the owner-occupied-vs-let split of DACH commercial stock and the average lettable
   commercial unit size (both unmeasured here). Do not present commercial with the confidence of the
   residential figure.
1. **Germany's private-landlord outsourcing share is the dominant source of error.** It alone moves
   the German number from ~8.4M to ~15M, i.e. it swings the whole DACH total by ~±5M. No single study
   cleanly reports "share of privately-owned rental dwellings run by a third-party Hausverwaltung."
   The 8.4M **floor** (professional/institutional owners) is hard-sourced; everything above it is an
   assumption about the 16.1M private stock. If you cite one German figure, cite the floor
   with the caveat, not the central.
2. **"Managed" vs "owned by a professional."** This counts in-house management by housing companies and
   cooperatives as professional management, since they are professional operations running the same
   workflows. A purist "third-party Bewirtschafter only" definition would trim Germany and Austria
   (removing coops/municipal in-house stock) but *not* Switzerland much.
3. **WEG / condominium administration is deliberately excluded.** ~10M German condos (>1.5M WEG) and
   large Austrian/Swiss Stockwerkeigentum pools have a professional Verwalter for the *building*, not
   the letting. Including WEG administration as "managed units" would push DACH well above 20M, but it
   is a different (adjacent) market from rental operations and would double-count against the rental
   figures.
4. **Rental-base definition wobble in Germany** (~23M vs ~25M depending on whether vacant/edge cases
   are included) moves the professional-owner floor by ~0.5M. Minor next to point 1.
5. **Commercial Hauptobjekte are only partially in scope.** These counts are residential dwellings
   plus the handful of commercial Lokale that appear inside residential-management statistics (e.g.
   GBV's 15,070). A full commercial-Hauptobjekt census would add to the total but is outside this
   residential-focused brief.

**One-line takeaway:** the honest, sourced answer is **~15M professionally-managed residential
Hauptobjekte in DACH (range ~11–19M)**, with a rock-solid **~11.4M floor** (Germany's 9.1M actively
*managed* by professional-commercial providers + Austria's ~1.0M GBV Verwaltungsbestand + Switzerland's
~1.3M institutional/cooperative) that needs no heroic assumptions. The ~20M figure is reachable only at
the top of the range and only by counting generous private-landlord outsourcing and/or WEG
condominium administration, and the latter was adversarially refuted as a clean addition.

---

## Method note

The primary pass was a manual bottom-up build from national statistical sources, country by country.

It was then independently cross-checked by an automated deep-research pass (2026-07-10): 20 sources
fetched, 25 claims adversarially verified, 22 confirmed and 3 refuted. That pass reproduced every
primary figure used above against Zensus 2022, GdW/vdw, Statistik Austria + GBV, and BFS, with none
refuted. Its own assembled central band was slightly wider (~13–18M, broad-case high ~24M). The gap
is entirely its more generous treatment of WEG/condominium building administration, which its own
verification then flagged as a double-count risk (the WEG → "always managed" mapping was refuted 0–3).

Net: two independent methods agree on the ~11M floor and a mid-teens central. They differ only on
how much adjacent condo-administration to fold in, which this file excludes on purpose.

---

## License and attribution

This work is licensed **CC BY 4.0** (see `LICENSE`). Share it, adapt it, use it commercially, just
give credit. `CITATION.cff` has a machine-readable citation, or use:

> Dolmetsch, R. (2026). *Professionally-managed dwellings in DACH: a sourced bottom-up estimate.*
> https://github.com/richdolm/dach-managed-units

The underlying statistics belong to their respective publishers: Statistisches Bundesamt, GdW/vdw,
Haus & Grund, IW Köln, Statistik Austria, GBV, Bundesamt für Statistik, BWO and SVIT. What is
licensed here is the compilation, the derivation and the commentary, not the source data.
