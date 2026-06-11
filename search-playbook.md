# Sales Navigator Search Playbook

Search recipes for the four priority segments, in mining order. Each recipe pairs an **account search** (find qualifying companies) with a **lead search** (find target personas at those companies). Run the account search first, save qualifying companies to an account list, then run the lead search against that list — this keeps revenue validation upstream of persona hunting.

## Shared parameters (all segments)

**Lead filters:**
- Seniority: CXO, VP
- Function: Purchasing, Supply Chain, Finance, Operations
- Geography: United States

**Title boolean (paste into Title field):**

```
("Chief Procurement Officer" OR "Chief Supply Chain Officer" OR "Chief Financial Officer" OR CFO OR CPO OR "VP Procurement" OR "Vice President Procurement" OR "VP Strategic Sourcing" OR "Vice President Strategic Sourcing" OR "VP Supply Chain" OR "Vice President Supply Chain" OR "SVP Supply Chain" OR "VP Finance" OR "Vice President Finance" OR "VP Operations" OR "Head of Procurement")
```

**Account filters:**
- Headcount: 201–500, 501–1,000, 1,001–5,000, 5,001–10,000, 10,001+ (headcount is a revenue proxy only — validate $100M+ separately before scoring)
- Headquarters: United States

**Revenue/ownership verification sources (all segments):** Food Processing Top 100, company press releases and newsrooms, 10-K/10-Q filings for public companies, PE firm portfolio pages, trade press cited per segment below.

---

## 1. Baking & Snacks

**Account search:**
- Industry: Food and Beverage Manufacturing; Baked Goods Manufacturing
- Keyword boolean:

```
(bakery OR baking OR "baked goods" OR bread OR buns OR rolls OR tortilla OR cookies OR crackers OR biscuits OR snacks OR chips OR pretzels OR popcorn OR "snack foods")
```

**Segment-specific verification sources:** Baking & Snack magazine, SOSLAND Baking Top 100, American Bakers Association membership, SNAC International membership.

**Watch for:** commodity exposure to wheat/flour, oils, and packaging — earnings or trade-press commentary on input-cost inflation is a strong cost-pressure signal. Heavy PE activity in this segment (tortilla, cookie/cracker, and in-store bakery roll-ups) — check ownership before scoring.

---

## 2. Confectionery

**Account search:**
- Industry: Food and Beverage Manufacturing
- Keyword boolean:

```
(confectionery OR confections OR candy OR chocolate OR chocolatier OR gummies OR gum OR licorice OR mints OR "sugar confection")
```

**Segment-specific verification sources:** Candy Industry Global Top 100, National Confectioners Association membership, Sweets & Snacks Expo exhibitor lists.

**Watch for:** cocoa and sugar price volatility — both have produced repeated margin-pressure commentary; an exec on record about input costs is a 5-score signal. Many mid-size family-owned confectioners sit right at the $100M line — verify revenue carefully.

---

## 3. Prepared Foods & Meat

**Account search:**
- Industry: Food and Beverage Manufacturing; Meat Products Manufacturing
- Keyword boolean:

```
("prepared foods" OR "prepared meals" OR "ready meals" OR "frozen entrees" OR "frozen foods" OR meat OR poultry OR pork OR beef OR protein OR sausage OR bacon OR deli OR "further processing" OR "value-added protein")
```

**Segment-specific verification sources:** The National Provisioner Top 100 Meat & Poultry Processors, Refrigerated & Frozen Foods Top 150, North American Meat Institute membership.

**Watch for:** this segment skews large — many processors clear $100M easily, so prioritize persona quality over company hunting. Protein input volatility and labor costs drive frequent cost-reduction initiatives. Significant co-man/private-label activity — both are in-scope.

---

## 4. Beverages

**Account search:**
- Industry: Beverage Manufacturing; Food and Beverage Manufacturing
- Keyword boolean:

```
(beverage OR beverages OR drinks OR soda OR "soft drinks" OR juice OR water OR "energy drink" OR "sports drink" OR coffee OR tea OR kombucha OR brewery OR distillery OR winery OR "beverage co-packer" OR "contract beverage")
```

**Segment-specific verification sources:** Beverage Industry Top 100, Beverage World, Brewers Association production rankings (for craft at scale).

**Watch for:** aluminum/PET packaging and freight are the dominant input-cost stories — packaging-cost commentary is a strong hook. Beverage co-packers (contract manufacturers) are explicitly in-scope and often under-prospected. High-growth better-for-you brands may be sub-$100M but PE-backed with roll-up theses — score 2–3 and note the sponsor.

---

## PE overlay (run after each segment)

- Industry: Venture Capital & Private Equity
- Title boolean:

```
("Managing Partner" OR "Managing Director" OR "Operating Partner" OR Partner)
```

- Keyword: food OR beverage OR consumer
- Validate F&B portfolio exposure on the firm's portfolio page before adding; capture portfolio company names in the notes field. A confirmed-F&B-portfolio PE contact scores 2 by rubric.
