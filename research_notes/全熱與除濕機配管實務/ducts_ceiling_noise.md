# Duct layout for a residential ERV (全熱交換器) and ducted dehumidifier (吊隱式除濕機): ceiling drop, beams, insulation, static pressure, noise and vibration

Context: Taiwan townhouse, 2F, living room plus master bedroom (~52 m²). Mitsubishi LGH-35RVX3-E (874×888×331 mm, Ø150 ports, max 350 m³/h) and Medole MD-70LBD (845×485×310 mm, 420 CMH, 3/4" drain). Both units sit in an under-stair storage room with no ceiling, and supply goes through walls. Target living-room ceiling is ≥2600 mm, with the slab at ~2800–2850 mm (not yet measured), so the plenum is only ~200–250 mm, before any beam.

Method note: WebFetch could not reach mitsubishielectric.com.au or library.mitsubishielectric.co.uk, because the session's network allowlist blocked those hosts. The remaining findings come from search-engine extracts of the cited pages, not from full reads of the PDFs. Figures marked "computed" are my own arithmetic (Darcy–Weisbach and the ASHRAE/Huebscher equal-friction formula), not published values.

---

## 1. Duct diameters, air velocities and flat/oval equivalents, and how much ceiling depth each needs

### Takeaway
Keeping ducts quiet means keeping velocity low. Aim for ≤3 m/s in the main runs next to the unit and ≤2 m/s in branches near rooms, which is the Passivhaus/CIBSE "low-velocity" practice. Taiwanese installer blogs are looser: mains at 5–8 m/s, outlets at 2–3 m/s. A Ø150 duct stays ≤3 m/s only up to ~190 m³/h, and a Ø200 only up to ~340 m³/h. At 350 m³/h a Ø150 runs at 5.5 m/s, and the 420 CMH dehumidifier runs a Ø200 at 3.7 m/s. For the same friction, a flat duct needs more cross-sectional area than the round duct it replaces, and the penalty grows as the duct gets flatter. A Ø150 equivalent at 80 mm high is ~255×80. A Ø200 equivalent at 100 mm high is ~370×100.

### Cited Findings
**Velocity criteria (spec-level and guidance sources)**
- Passivhaus Trust *How to Build* Ch.8: the MVHR system is designed for low velocity and low pressure, with velocities **<2 m/s, up to 3 m/s for the main ducts at the MVHR unit and its connections to outside**. Design ventilation noise in living rooms and bedrooms is **<25 dB(A)** — [Passivhaus Trust, How to Build Ch.8](https://passivhaustrust.org.uk/UserFiles/File/Technical%20Papers/How%20to%20Build%202023/HowToBuild-Ch8.pdf)
- Passivhaus Trust MVHR Good Practice Guide: "High velocity air generates noise, and therefore air speed limits are recognised for ducts in different locations to minimise noise problems" — [PHT MVHR Good Practice Guide 2018](https://www.passivhaustrust.org.uk/UserFiles/File/Technical%20Papers/2018%20MVHR%20Good%20Practice%20Guide%20rev%201.1.pdf)
- CIBSE Guide B2 describes a low-velocity system as having AHU face velocity typically <2 m/s and main duct velocity <3 m/s. It says ductwork must be sized correctly for velocity, "particularly to avoid noise". I saw this only through a Scribd copy; the CIBSE tables 2.16/2.17 themselves were not visible — [CIBSE Guide B2 (Scribd copy)](https://www.scribd.com/document/688287828/CIBSE-Guide-B2-2016-Ventilation-Ductwork)
- A UK installer guide gives 2–3 m/s in distribution branches and ≤4 m/s in main spines. This is looser than Passivhaus — [APM MVHR guide](https://apmi.uk/blogs/news/mvhr-mechanical-ventilation-heat-recovery-design-installation-part-f)
- A vendor calculator gives residential mains at 600–900 fpm (3.0–4.6 m/s) and branches at 400–600 fpm (2.0–3.0 m/s). These are ASHRAE/SMACNA-style comfort-HVAC numbers, not low-noise MVHR numbers — [Anglian PHE duct velocity calculator](https://anglianphe.co.uk/duct-velocity-calculator/)

**Taiwan practice (rules of thumb; the sources disagree)**
- FENNEY (Taiwan installer): main runs **5–8 m/s**, branches **3–5 m/s**, outlet ends **2–3 m/s**. Air above ~**5 m/s** in a too-small duct causes noise and vibration. Round duct has ~10–15% less resistance than square. Keep contractions ≤15° and expansions ≤7° — [FENNEY 全熱交換器安裝全攻略](https://fenney.tw/blog/total-heat-exchanger-installation/)
- Vortexfresh (Taiwan ERV vendor) calculator: outlet (風口) velocity 2–5 m/s, with **2.0–4.0 m/s as the "standard" range** — [沃特奇 風速計算與風口建議](https://vortexfresh.com.tw/airventcalculator/)
- 王本楷裝修研究室 (Taiwan designer): comfort air speeds of ~0.5 m/s in living/dining, ~0.3 m/s in bedrooms and ~0.2 m/s for sensitive sleepers. These look like occupied-zone/draught speeds rather than grille face velocities. The same source recommends a larger duct diameter near the unit and smaller at the ends, sized to each room's occupancy — [vwdesign 13項全熱交換器設計安裝重點](https://vwdesign.pixnet.net/blog/post/122230445)
- Mobile01 owners: whole-house runs are commonly >10 m, in 6" and 4" sizes. Galvanised spiral duct and PVC pipe have lower loss than nylon flex — [Mobile01 全熱交換器的管路配法](https://www.mobile01.com/topicdetail.php?f=168&t=4744507); [Mobile01 全熱交換器風管材質分享](https://www.mobile01.com/topicdetail.php?f=168&t=5559830)
- Taiwanese "全熱系統扁管" products are as thin as **50 mm** and connect to 3" round PE pipe. These are small-bore, high-velocity systems, not Ø150 class — [hocom 全熱系統扁管](https://web.hocom.tw/h/newsinfo?key=900250758929&cont=254881)

**Flat-duct equivalence**
- UK sellers market 204×60 mm flat channel as "equivalent" to Ø125 round. The areas are 12,240 mm² vs 12,272 mm², so this is an equal-**area** match — [tradecalculator duct sizing tables](https://tradecalculator.co.uk/reference/duct-sizing-tables/); [efans 204×60 ducting](https://www.efans.co.uk/collections/204mm-x-60mm-rectangular-ducting)
- The equivalent diameter for **equal friction**, which is the right basis for fan and noise purposes, is De = 1.30·(a·b)^0.625/(a+b)^0.25 (Huebscher/ASHRAE) — [Engineering Toolbox, equivalent diameter](https://www.engineeringtoolbox.com/equivalent-diameter-d_443.html)

**Unit/plenum heights (for context)**
- In Taiwan a ceiling-hung ERV usually needs **35–40 cm** of ceiling reserve. One measured install (a Delta unit plus 角材 framing) took the ceiling down a total of ~30–31 cm — [安心整合 過樑方式風量測試](https://t0955255777.pixnet.net/blog/post/34006952)
- A ducted dehumidifier typically needs **35–45 cm** of reserved height, depending on brand and model. Access panels are typically ~10–15 cm larger than the unit body and sit directly under it — [PRO360 老屋除濕機指南](https://www.pro360.com.tw/guide/old_house_reno_dehumidifier)

### Inferences
**Computed velocities for round duct (v = Q / area):**

| Airflow | Ø100 | Ø125 | Ø150 | Ø160 | Ø180 | Ø200 | Ø250 |
|---|---|---|---|---|---|---|---|
| 75 m³/h (one room) | 2.65 | 1.70 | 1.18 | 1.04 | 0.82 | 0.66 | 0.42 |
| 100 m³/h | 3.54 | 2.26 | 1.57 | 1.38 | 1.09 | 0.88 | 0.57 |
| 150 m³/h | 5.31 | 3.40 | 2.36 | 2.07 | 1.64 | 1.33 | 0.85 |
| 175 m³/h (LGH-35 speed 2) | 6.19 | 3.96 | 2.75 | 2.42 | 1.91 | 1.55 | 0.99 |
| 263 m³/h (speed 3) | — | 5.95 | 4.13 | 3.63 | 2.87 | 2.33 | 1.49 |
| 350 m³/h (speed 4) | — | 7.92 | 5.50 | 4.84 | 3.82 | 3.09 | 1.98 |
| 420 m³/h (MD-70LBD) | — | 9.51 | 6.60 | 5.80 | 4.58 | 3.71 | 2.38 |
| **Max flow at 3 m/s** | 85 | 133 | **191** | 217 | 275 | **339** | 530 |

**What this means for this house (computed):**
- **ERV:** for ~52 m² and 2–4 occupants, realistic continuous flow is ~100–175 m³/h, so speed 1–2. A single Ø150 main then runs at ≤2.75 m/s, which meets the 3 m/s "quiet main" rule. Splitting into two rooms gives two branches of ~75–90 m³/h each. A Ø125 branch at 75–90 m³/h runs at ~1.7–2.0 m/s and meets the ≤2 m/s branch rule. A Ø100 branch runs at 2.65–3.2 m/s, which is only acceptable for a short final stub. Running speed 4 (350 m³/h) through Ø150 gives 5.5 m/s, above even the Taiwanese 5 m/s noise threshold.
- **Dehumidifier at 420 CMH:** a single Ø200 runs at 3.7 m/s. Options that get to ≤3 m/s: a Ø250 main (2.4 m/s); a 400×100 flat duct (2.9 m/s); or splitting at the unit into two Ø150/Ø160 branches of ~210 m³/h each (3.3 / 2.9 m/s), or two Ø180 branches (2.3 m/s). In practice the dehumidifier will often run at lower fan speed. Check the Medole low/high fan airflow, which is not found (see Gaps).

**Computed flat-duct sizes for equal friction (De by Huebscher formula), with velocities:**

| Flat duct (W×H, mm) | Equal-friction De | Equal-area De | v @175 | v @350 | v @420 |
|---|---|---|---|---|---|
| 204×60 | **116** (not 125) | 125 | 3.97 | 7.94 | — |
| 220×90 | 150 | 159 | 2.46 | 4.91 | 5.89 |
| 250×80 | 149 | 160 | 2.43 | 4.86 | 5.83 |
| 300×80 | 161 | 175 | 2.03 | 4.05 | 4.86 |
| 400×60 | 153 | 175 | 2.03 | 4.05 | 4.86 |
| 300×100 | 183 | 195 | 1.62 | 3.24 | 3.89 |
| 400×80 | 182 | 202 | 1.52 | 3.04 | 3.65 |
| 500×80 | 199 | 226 | 1.22 | 2.43 | 2.92 |
| 400×100 | 207 | 226 | 1.22 | 2.43 | 2.92 |

- Minimum width for a given height (equal friction, computed):
  - Ø150 equivalent: H=50 → W≈496; H=60 → W≈379; H=80 → W≈255; H=100 → W≈194.
  - Ø200 equivalent: H=60 → W≈777; H=80 → W≈505; H=100 → W≈370; H=120 → W≈293.
  - Below ~60 mm height the flat duct needs 30–65% more cross-section than the round duct it replaces. **Practical sweet spot:** use ≥80 mm height for an ERV flat section and ≥100 mm for the dehumidifier.
- Flat oval (computed, ASHRAE flat-oval De): 300×80 oval ≈ Ø159; 300×100 ≈ Ø180; 400×100 ≈ Ø205.
- **Ceiling depth per duct type.** This is an estimate, unsourced. It assumes Taiwanese 角材 framing of ~30–36 mm plus 6–9 mm 矽酸鈣板, and ~10–20 mm for hanger strap or clearance:
  - Bare Ø150 round: ~200–215 mm below slab/beam.
  - Ø150 with 25 mm insulation (OD ≈ 200): ~250–265 mm.
  - Bare Ø200: ~250–265 mm.
  - Insulated Ø200 (OD ≈ 250): ~300–315 mm.
  - 80 mm-high flat: ~130–145 mm. 100 mm-high flat: ~150–165 mm. Add ~25 mm per side if the flat duct is insulated.
- **With slab 2800–2850 and a 2600 ceiling (200–250 mm plenum):** a bare Ø150 just fits under the slab, but nothing round fits under a beam. Insulated OA/EA ducts and any Ø200 should therefore stay in the storage room, a wall chase or a 假樑/包樑 bulkhead. Only short, uninsulated SA/RA branches, preferably 80–100 mm flat, should run in the living-room ceiling plenum.
- **Supply grille face velocity:** use ≤2 m/s through the free area for bedrooms (Passivhaus <2 m/s; FENNEY 2–3 m/s at outlets). This is a rule of thumb, not a spec. For example, 90 m³/h at 2 m/s needs 0.0125 m² free area, i.e. ~250 cm² gross at 50% free-area ratio, roughly a 250×100 grille (computed).

### Gaps
- I found no Taiwanese standard or manufacturer table of 扁管 sizes (e.g. PVC flat duct in 60/80/100 mm heights) matched to Ø150/Ø200. Equivalents above are computed. Installers should state the actual product (supplier, W×H) and its friction data.
- A search extract said a UK retailer lists 220×90 mm as the Ø150 equivalent, but it did not name which retailer, so I could not cite it. By equal friction 220×90 computes to De ≈ 150 mm, which is consistent.
- I found no MD-70LBD fan-speed table (low/medium/high airflow).

---

## 2. Crossing or avoiding beams (繞梁 / 過梁), and when (if ever) a beam may be penetrated

### Takeaway
Taiwanese contractors are unanimous: **do not core-drill (洗洞) structural beams** for ERV ducts. The accepted options are:
- Route parallel to beams within the beam bays.
- Pass under the beam with a thin flattened section (壓扁管) or a purpose-made 過樑器 (~3 cm thick), accepting extra airflow loss.
- Use only the sleeves (套管) the builder cast in, which are typically only 10–12 cm.

Any new beam penetration needs a structural engineer (結構技師). I found no formal published rule for sleeve size or position in residential practice; forum numbers are unofficial.

### Cited Findings
- "萬~萬~不可洗洞" (never core-drill a beam) for supply ducts, for structural safety. The same source says passing **under a beam with 3" duct drops the ceiling ~9 cm, and with 6" duct ~18 cm**, whereas a **過樑器 is ~3 cm thick** — [安心整合 3種過樑方式風量測試](https://t0955255777.pixnet.net/blog/post/34006952); [YouTube 安心整合 lintel-duct](https://www.youtube.com/watch?v=0W9SKz565zo)
- Measured airflow loss over a **10 m supply run** (Delta VEB250AT3, 7 cm outlet, 20 m/s at source): **~28% without a 過樑器 vs ~34% with one**. These are single, uncontrolled measurements on a small-bore high-velocity system — [安心整合](https://t0955255777.pixnet.net/blog/post/34006952)
- A second write-up of the same Delta-250 test gives 28% vs 34%, and says a **flattened duct (壓扁) costs ~4% airflow** but adds resistance and noise — [Home Type 家居 過樑器實測](https://type.tw/article/765)
- Mobile01 posters report 過樑器 losses of **20–40%**. Others claim professionally installed systems lose only ~5% overall. These are anecdotal — [Mobile01 全熱交換器風管風量損失](https://www.mobile01.com/topicdetail.php?f=731&t=6106914)
- Builder-preset sleeves through beams are typically only **~10–12 cm**, while installers use standard 5" ducts, which forces reducers and destabilises airflow. Forum posters suggest holes should be **~27 cm above the bottom of a main beam and ~24 cm for a secondary beam**. This is a netizen rule of thumb, not a code. Another poster notes that steel beams may not allow even preset holes — [Mobile01 全熱交換機預留穿樑問題](https://www.mobile01.com/topicdetail.php?f=360&t=2942943)
- Common advice: use rigid PVC for long runs, 斜T (Y-branches) at turns, and squashed PP duct for the beam-crossing segment. Put the beam crossing on the small end branches rather than the main — search extract covering [Mobile01 天花板討論](https://www.mobile01.com/topicdetail.php?f=360&t=6554529) and [vwdesign 嚴公館案例](https://vwdesign.pixnet.net/blog/posts/7119969145)
- Keep the route short with few bends, and use 45° 斜T/斜彎 instead of 90° elbows and straight tees — [udn 全熱交換器的規劃要領](https://blog.udn.com/42d2f647/153239451); [vwdesign 13項重點](https://vwdesign.pixnet.net/blog/post/122230445)

### Inferences
- **For this house:** the units are in an under-stair room with no ceiling and supply goes through walls, so the cheapest beam strategy is to **avoid crossing beams in the living-room ceiling altogether**:
  - Penetrate partition walls **below** the beam soffit and enter each room as a high-wall supply (高壁出風).
  - Or run ducts along the beam line inside a narrow 包樑/假樑 bulkhead. That drops only a strip, not the whole ceiling.
  - Walls under beams in townhouses are often brick or RC. An opening in an RC wall, or a large opening in a load-bearing brick wall, should also go to a structural engineer. Small openings in a non-load-bearing brick partition normally need only a lintel/frame. This is a general construction inference, not sourced.
- If a crossing is unavoidable, use a flat section of ≥80 mm height. A Ø150 equivalent is ~255×80 by equal friction. Its added resistance is small at ERV speed-2 airflow. Avoid 30–50 mm "ultra-flat" transitions on the main, because their equivalent diameter collapses and velocity and noise rise.
- The 28%/34% loss figures come from a small-bore 7 cm, ~20 m/s system. They should not be read across directly to a Ø150 system at 2–3 m/s, where pressure loss scales with roughly velocity² (computed reasoning).

### Gaps
- I found no published Taiwanese code clause or structural-engineer guideline on post-construction beam penetrations for residential ducts (sleeve diameter vs beam depth, distance from support, reinforcement). The forum rule (27/24 cm from beam bottom) is unverified.
- I found no measurements of 過樑器 loss on Ø150 low-velocity systems.

---

## 3. Which ducts must be insulated, how thick, the resulting outer diameter, and condensation risk

### Takeaway
Mitsubishi's RVX3 manual requires the **two outdoor-side ducts (OA and EA) to be insulated** and **sloped ≥1/30 down toward the outside**. Without that insulation, condensation and water dripping from the unit can occur. Taiwanese installers agree that OA and EA ducts must be insulated. Opinions on SA vary, and RA is generally left bare. I found no Taiwan-specific thickness standard for ERV ducts. Thickness should be picked so the outer surface stays above the dew point, and Taiwan's humidity means international minimums may be insufficient.

### Cited Findings
- LGH-15–200RVX3-E installation manual: "The two outdoor ducts must be covered with heat-insulating material in order to prevent condensation from forming". "Without additional insulation, it could cause condensation and water drop from the unit". "The duct should have a slope of 1/30 toward the outdoors". The manual lists minimum outdoor-side duct lengths of ~**1.0 m for LGH-15 to 65**, 2.5 m for LGH-80/100 and 3 m for LGH-160/200. The extract was garbled, so verify against the PDF — [Mitsubishi IM LGH-15–200RVX3-E](https://www.mitsubishi-electric.co.nz/materials/ventilation/manuals/lossnay/lgh-rvx3-e/2_installation/im_lgh-15-200rvx3-e.pdf)
- LGH-50RVX3-E specification: "The outdoor side duct (OA and EA) shall decline by 1/30 or more downward to outdoor" — [Mitsubishi SPC LGH-50RVX3-E](https://www.mitsubishi-electric.co.nz/materials/PRODUCT/Ventilation/LGH-RVX3-E/01_Specifications/SPC_LGH-50RVX3-E.pdf)
- 瑞翔風管工程 (Taiwan duct contractor):
  - The **OA (外氣入口)** duct needs insulation because of the indoor–outdoor temperature difference.
  - The **supply duct** can also see condensation and is insulated in their practice.
  - The **EA duct** needs insulation where it runs near walls in contact with warm indoor air.
  - The **RA (回風)** duct does not.
  - The article also compares 保溫棉 (wrap) and 保溫板 (board) — [瑞翔 全熱交換器吊裝](https://rayhsiang.com.tw/%E5%85%A8%E7%86%B1%E4%BA%A4%E6%8F%9B%E5%99%A8%E5%90%8A%E8%A3%9D/)
- Mobile01: the outdoor-side intake and exhaust ducts need insulation. **Metal spiral duct conducts heat quickly** and drips if uninsulated when the inside–outside temperature difference is large — [Mobile01 風管材質分享](https://www.mobile01.com/topicdetail.php?f=168&t=5559830)
- CKY (Taiwan HVAC insulation guide): insulation must be thick enough to keep the outer surface above ambient dew point. In Taiwan's high humidity, international minimum thicknesses may be inadequate and a condensation check is needed. Its thickness tables cover chilled-water pipes, not ERV ducts — [CKY 空調管路保溫工程設計指南](https://www.cky.com.tw/insights/hvac-pipe-insulation-design)

### Inferences
- **Condensation mechanisms in Taiwan.** This is psychrometric reasoning, not a sourced figure:
  - **Summer:** OA at ~33 °C and 70% RH has a dew point of ~26–27 °C. If the OA duct passes through an air-conditioned 26 °C space, the duct wall can sit at or below the OA dew point, so condensation forms **inside** the OA duct. The 1/30 fall to outside lets that water drain out rather than into the unit. EA after the core is still warm and humid, and the same applies.
  - **Winter:** OA at ~10–15 °C cools the duct below indoor dew point (~12–14 °C), so condensation forms **on the outside** of the OA duct.
  - Both are reasons to insulate OA and EA over their full indoor length with a **vapour-tight** jacket: closed-cell PE/NBR, or fibreglass with sealed foil.
- **SA/RA in this layout:** ERV SA after the core is close to room temperature. Dehumidifier SA is warm and dry, since the compressor reheats it. So SA/RA insulation is mainly optional for condensation. It can still help with noise, or where ducts touch AC supply ducts or run in unconditioned spaces. RA can stay bare.
- **Thickness and outer diameter.** This is a typical-practice estimate, unsourced. 20–25 mm insulation turns Ø150 into an OD of ~190–200 mm and Ø200 into ~240–250 mm. That is why OA/EA should be kept in the storage room and exterior wall rather than in the low living-room plenum. With a short OA/EA run, the insulated length is minimal.
- Because the units sit in the storage room, put the OA/EA wall penetrations on the storage-room exterior wall, so the insulated outdoor ducts are short. The manual's ~1 m minimum outdoor-duct length for LGH-15–65 still applies (verify the figure). Separate the OA intake from the EA discharge and from AC condensers and any kitchen/toilet exhaust.

### Gaps
- I found no published Taiwan thickness spec for ERV OA/EA duct insulation, and could not reach the Mitsubishi manual text that may specify the insulation material or thickness. The installer should state the material (PE/NBR/glass wool), thickness and vapour barrier.
- I found no Medole guidance on insulating dehumidifier supply ducts.

---

## 4. Flexible duct limits and external static pressure: Mitsubishi LGH-35RVX3-E airflow vs ESP, and how much duct it can handle

### Takeaway
Mitsubishi rates the LGH-35RVX3-E at **88 / 175 / 263 / 350 m³/h at 10 / 40 / 90 / 160 Pa** ESP for speeds 1–4 (15 / 29 / 61 / 120 W). These four points lie on one quadratic system curve, so the rating effectively describes a duct system with **160 Pa resistance at 350 m³/h**. A well-built Ø150 rigid system of ~8–10 m per airstream with 3–4 bends, hood and grille uses well under that, leaving margin.

Flex duct is the main way to waste the budget. Rules:
- Pull it fully extended (≤4% compression).
- Support it every ≤1.2 m with ≤42 mm/m sag.
- Count each 90° flex bend as ~6 m (20 ft) of duct.
- Keep flex as short connectors (~0.4 m) rather than long runs.

### Cited Findings
**LGH-35RVX3-E fan/ESP data (manufacturer)**
- Mitsubishi NZ: fan speeds 1–4 give ESP **10, 40, 90, 160 Pa** at **24, 49, 73, 97 L/s** (~88/175/263/350 m³/h). Input power is 15–29–61–120 W — [Mitsubishi Electric NZ LGH-35RVX3-E](https://www.mitsubishi-electric.co.nz/ventilation/i/685105/lossnay-fresh-air-energy-recovery-ventilation)
- Mitsubishi HK RVX3 series table: LGH-35RVX3 at **88/175/263/350 m³/h** and **10/40/90/160 Pa**, power 15/29/61/120 W — [Mitsubishi Electric HK RVX3 Series](https://www.mitsubishielectric.com.hk/en/products/details/RVX3-Series)
- The Mitsubishi publication gives 350 m³/h at 160 Pa for 100% speed. Airflow, ESP and SFP are tested to BS EN 13053:2019, and the heat-exchange data to ISO 16494-1 — [Mitsubishi NZ Lossnay LGH-RVX3 publication](https://www.mitsubishi-electric.co.nz/publications/ventilation/Lossnay-LGH-RVX3-Energy-Recovery-Ventilation/)
- Retailers agree: "External Static Pressure 160 Pa" at maximum speed, "100% (Default speed 4) … 160 Pa" — [ShopClima LGH-35RVX3-E](https://www.shopclima.it/en/mitsubishi-electric-lgh-35rvx3-e-lossnay-enthalpic-heat-recovery-unit-for-horizontal-or-vertical-installation-350-m3-h.html); [airconditioning-online.com.au](https://www.airconditioning-online.com.au/product/mitsubishi-electric-lossnay-heat-recovery-ventilation-lgh-35rvx3-e/)
- **Conflict:** BPC Ventilation lists "350 m³/hr @ 100 Pa", which the manufacturer data I found does not support — [BPC Ventilation](https://bpcventilation.com/products/mitsubishi-lossnay-lgh-35rvx3-e). The NZ range brochure gives an airflow range of 24–97 L/s, consistent with the above — [Mitsubishi NZ LGH-RVX3 range brochure](https://www.mitsubishi-electric.co.nz/materials/PRODUCT/Ventilation/LGH-RVX3-E/00_Publications/02_Brochure/LGH-RVX3_Range.pdf)
- **Unverified:** a search extract of the Australian flyer mentioned ~104 L/s at 85 Pa at a "75%" setting and 19 dB(A) at lowest speed. This conflicts with the 97 L/s maximum elsewhere, could not be fetched, and is probably a garbled table read — [Mitsubishi AU Lossnay RVX3 flyer 2024-11](https://mitsubishielectric.com.au/wp-content/uploads/2024/12/Flyer_Lossnay-RVX3-E-2024-11.pdf)

**Flex duct rules (US ADC/industry guidance)**
- Install flex fully extended. Fully extended means **≤4% longitudinal compression**, and compression raises friction roughly proportionally. For sizing, **each 90° bend adds ~20 equivalent feet (~6 m)** — [Royal Metal Products, flex duct installation per ADC](https://royalmetalproducts.com/wp-content/uploads/904-Flex-Duct-Black-Installation-Instructions.pdf)
- Support at **≤4 ft (1.2 m)** intervals, with maximum sag **½ in per ft (42 mm per m)**. Vertical runs need straps every ≤6 ft (1.8 m) — [Royal Metal Products](https://royalmetalproducts.com/wp-content/uploads/904-Flex-Duct-Black-Installation-Instructions.pdf); [PNNL BASC, support intervals for flex ducts](https://basc.pnnl.gov/resource-guides/support-intervals-flex-ducts)
- Excess flex material in a run should be **<5%**, because extra material raises friction — [ASHI home inspectors' guide to flex duct](https://www.homeinspector.org/reporter-articles/a-home-inspectors-guide-to-flexible-hvac-duct-installation/)
- ERV/HRV makers use flex only as a **short connector**. One example is a ~**16 in (~0.4 m)** flex between the unit and the rigid duct "for noise dampening". Another guide requires flex connections between the HRV/ERV and the rigid duct — [Honeywell/TrueFRESH ERV/HRV install guide](https://api.ferguson.com/dar-step-service/Query?ASSET_ID=4289745&USE_TYPE=INSTALLATION&PRODUCT_ID=4425300); [Imperial Air Solace HRV/ERV guide](https://www.gasexperts.ca/wp-content/uploads/2016/06/Solace-Installation-Guide.pdf)
- Taiwan: nylon flex has an internal steel wire and corrugated inner face, so it has higher resistance than rigid duct — [Mobile01 風管材質分享](https://www.mobile01.com/topicdetail.php?f=168&t=5559830). Flex sags, which causes uneven airflow and under-delivery, so rigid duct is preferred — [100室內設計 全熱交換機眉角](https://www.100.com.tw/article/1365)
- Duct, grilles and distribution boxes all add pressure loss and must be pre-budgeted. One Taiwanese designer estimates the airflow loss at ~10% with good design and **>50% when not calculated** — [vwdesign 2023 全熱交換器品管關鍵](https://vwdesign.pixnet.net/blog/posts/7119111332)

### Inferences
- **Reading the ESP table (computed check):** K = 160/350² = 0.001306 Pa/(m³/h)². That gives 175² × K = 40 Pa, 263² × K = 90 Pa and 88² × K = 10 Pa. So the four ratings are points on **one system curve**, not four independent fan limits. Practical meaning: if the owner's duct system loses ≤40 Pa at 175 m³/h (equivalently ≤160 Pa at 350 m³/h), each speed will deliver at least its catalogue airflow. A system with more resistance will deliver less at every speed. The full fan curve, i.e. the maximum ESP available at each speed, could not be retrieved (see Gaps).
- **The ESP budget applies to each airstream separately.** OA duct + hood + SA duct + grilles must fit within it, and so must RA grille + RA duct + EA duct + hood. The unit's own filters and core are presumably inside the rating, but confirm this.
- **Computed friction for galvanised/PVC smooth duct (Darcy–Weisbach, ε = 0.09 mm):**
  - Ø150 at 175 m³/h: 0.76 Pa/m. At 263: 1.6 Pa/m. At 350: 2.7 Pa/m.
  - Ø125 at 90 m³/h: ~0.55 Pa/m. Ø125 at 175: 1.85 Pa/m.
  - Ø200 at 420 m³/h: 0.92 Pa/m. Ø250 at 420: 0.31 Pa/m.
  - Velocity pressure for Ø150 at 175 / 350 m³/h is 4.5 / 18.2 Pa, so each smooth 90° elbow (K≈0.3–0.4) costs ~1.5 / ~6–7 Pa.
- **Example path (computed):** 8 m rigid Ø150 + 4 elbows ≈ **12 Pa at 175 m³/h, 27 Pa at 263, 47 Pa at 350**. This excludes the wall hood, grille, branch box and any flex. Hood and grille might add ~10–30 Pa at speed 4 (unsourced estimate). Result: a short Ø150 rigid layout like this house's (unit in the under-stair room, ~3–8 m per run) comfortably fits the 40 Pa / 160 Pa budgets. Long flex runs, compressed flex, 90° tees, or squeezing to Ø100/flat 60 mm can quickly consume it.
- **Practical limits to give the installer.** These are rules of thumb synthesised from the above:
  - Flex only as ≤0.5–1 m connectors at the unit (for vibration) and at grilles. Pull it taut, support it ≤1.2 m apart, and use no flex for 90° turns (use rigid long-radius elbows or two 45°s).
  - ≤4 elbows per airstream.
  - Use 45° Y-branches (斜T) for splits.
  - Keep the total equivalent length per airstream ≤~15–20 m at speed 2–3.
- **Dehumidifier:** a 420 CMH Ø200 path of 6 m + 3 elbows computes to ~14 Pa (Ø250: ~5 Pa), excluding grilles. Whether that fits depends on Medole's unpublished ESP.

### Gaps
- I could not retrieve the LGH-35RVX3-E full fan characteristic curve (ESP vs airflow per speed, beyond the rated points) or Mitsubishi's duct-resistance charts for Ø150. Both are in the Mitsubishi technical data book (library.mitsubishielectric.co.uk / AU flyer, blocked here). Also unconfirmed: whether the RVX3 has constant-airflow control or a fan-speed fine-adjust setting.
- **The MD-70LBD external static pressure is not published** on any page found ([Medole MD-70LBD](https://www.medole.com.tw/md-70lbd.html); [dealer page](https://htx4379.waca.ec/product/detail/1777408)). The manual may be on the [Medole 說明書下載](https://www.medole.com.tw/cate-282067.htm) page. One ducted-dehumidifier dealer says that for ≤25 坪 with well-controlled duct length and **≤4 outlets**, a 70 L unit still performs well. That is dealer experience, not a spec — [仁裕 風管式除濕機容量](https://www.renyuac.com/post/%E3%80%90%E7%A7%91%E6%99%AE%E4%B8%80%E4%B8%8B%E3%80%91%E9%A2%A8%E7%AE%A1%E5%BC%8F%E9%99%A4%E6%BF%95%E6%A9%9F%EF%BC%8C%E5%AE%B9%E9%87%8F%E5%A4%A7%E5%B0%8F%E5%88%B0%E5%BA%95%E6%80%8E%E9%BA%BC%E9%81%B8%EF%BC%9F)
- I found no published maximum total flex-duct length for ERVs. US guidance limits compression and sag, not absolute length.

---

## 5. Noise and vibration: silencers, acoustic flex, anti-vibration hangers, grille face velocity, unit placement

### Takeaway
The levers are, in order:
1. Keep the unit out of bedrooms and living rooms, which this house already does with the under-stair room.
2. Keep duct velocity low (≤3 m/s mains, ≤2 m/s near rooms) and run the fan at a low speed. Oversizing ducts so that speed 2 delivers the needed airflow is the quietest strategy.
3. Decouple the unit from the structure with anti-vibration hangers or pads and a short flexible connector.
4. Add an acoustic flex or a silencer section on the SA (and RA) side before the first room.

The design target is <25 dB(A) in living rooms and bedrooms (Passivhaus).

### Cited Findings
- Passivhaus design noise from ventilation in living rooms and bedrooms is <25 dB(A), with low-velocity ducts (<2 m/s; ≤3 m/s mains) — [Passivhaus Trust How to Build Ch.8](https://passivhaustrust.org.uk/UserFiles/File/Technical%20Papers/How%20to%20Build%202023/HowToBuild-Ch8.pdf)
- Taiwan: do not place the main unit in bedrooms or studies. If an outdoor unit is against a bedroom wall, soundproof it, because low-frequency noise disturbs sleep. Owners report the unit noise is noticeably harsh at night — [100室內設計](https://www.100.com.tw/article/1365); [Mobile01 為什麼有裝全熱交換器但不使用](https://www.mobile01.com/topicdetail.php?f=731&t=5289747&p=3)
- Labelled noise is often ~30 dB, while outlet noise is said to be 40–50 dB. One owner reported 65–70 dB measured at an outlet. That figure is anecdotal and methodology unknown. Turning the fan to maximum to make up for poor airflow raises noise — [100室內設計](https://www.100.com.tw/article/1365); [LINE Today 全熱交換機懶人包](https://today.line.me/tw/v3/article/8nlWZxz)
- An owner reported that a long (20 m) nylon flex run was much quieter (less 風切聲) at the same airflow. This is anecdotal, and flex attenuates noise at the cost of pressure loss — search extract from [Mobile01 不使用討論](https://www.mobile01.com/topicdetail.php?f=731&t=5289747&p=3)
- Supply ducts are under positive pressure and can resonate and make noise, so they need anti-vibration hanging — [vwdesign 嚴公館案例](https://vwdesign.pixnet.net/blog/posts/7119969145)
- Above-ceiling anti-vibration frames (防震架台) and silencer accessories are sold for ERVs and concealed fan units. The vendor claims ≥90% reduction in vibration transmitted to the building. That is a single-vendor claim, not independently verified — [和泰 HOTAI 型錄 PCW2023-2](https://www.hotaidev.com.tw/catalog/PCW2023-2/47/)
- A ~0.4 m flex between unit and rigid duct is used "for noise dampening" — [Honeywell/TrueFRESH install guide](https://api.ferguson.com/dar-step-service/Query?ASSET_ID=4289745&USE_TYPE=INSTALLATION&PRODUCT_ID=4425300)
- A too-small duct (>~5 m/s) generates noise and vibration — [FENNEY](https://fenney.tw/blog/total-heat-exchanger-installation/)
- Separate the OA intake and EA outlet as far as possible, ideally on different sides of the house — [100室內設計](https://www.100.com.tw/article/1365)
- A ducted dehumidifier needs an access panel ~10–15 cm larger than the unit, directly below it, and a planned condensate drain route — [PRO360 除濕機指南](https://www.pro360.com.tw/guide/old_house_reno_dehumidifier)

### Inferences
**Installer checklist: rules of thumb synthesised from the sources above; cite as guidance, not spec**
- **Unit mounting:**
  - Hang the LGH-35RVX3-E (and the MD-70LBD) from the under-stair structure on rubber or spring anti-vibration hangers, or set it on an isolated shelf with rubber pads.
  - Do not bolt it rigidly to a wall shared with a bedroom.
  - Keep both units level, and the dehumidifier drain at a positive fall with a trap.
  - Line the storage-room door and walls with absorptive material if they adjoin the living room. Unsourced.
- **Connections:** fit a 0.3–1 m flexible or acoustic-flex connector at every unit spigot, pulled taut, to break structure-borne vibration.
- **Attenuation:** before the first room on SA and RA, use a ~1 m section of acoustic (perforated-liner) flex or a short circular silencer. Insulated SA/RA ducts also add some attenuation. I could not find a Mitsubishi- or Taiwan-sourced spec length for this.
- **Velocity:**
  - Mains ≤3 m/s: Ø150 up to ~190 m³/h, Ø200 up to ~340, Ø250 up to ~530.
  - Branches ≤2 m/s: Ø125 up to ~88 m³/h, Ø150 up to ~127.
  - Grille free-area face velocity ≤~2 m/s in bedrooms.
  - Use long-radius elbows or 2×45°, and keep reducers ≤15° and expanders ≤7°.
- **Crosstalk:** a single trunk that feeds both bedroom and living room can carry speech and TV sound between rooms. Give each room its own branch from a distribution point inside the storage room, with a length of acoustic flex on each branch. This is general MVHR practice, not sourced here.
- **Operation:** size ducts so the needed airflow (~100–175 m³/h) comes at speed 1–2 (10–40 Pa rating points). Avoid relying on speed 4, which is 120 W and much louder, at 5.5 m/s in Ø150.
- **Dehumidifier:** at 420 CMH, use a ≥Ø250 or flat 400×100 main, or split immediately into two branches, to stay near 3 m/s. Put the supply grilles away from the beds. The compressor's vibration makes isolated mounting more important than for the ERV.
- **Commissioning:** measure the airflow at each grille with an anemometer or flow hood after installation and compare it with the rated airflow. This is recommended in Taiwanese sources ([安心整合](https://t0955255777.pixnet.net/blog/post/34006952); [vwdesign 2023](https://vwdesign.pixnet.net/blog/posts/7119111332)). Also measure dB(A) in the bedroom at night at the intended speed.

### Gaps
- No Mitsubishi LGH-35RVX3-E sound data per speed (dB(A) at 1.5 m) was retrieved, except an unverified 19 dB(A) at lowest speed from the AU flyer extract.
- I found no MD-70LBD noise rating.
- I found no independent test data on acoustic-flex or silencer insertion loss for Ø150 residential ducts in a Taiwanese context.
- Whether the brick or RC wall between the storage room and bedroom gives enough sound isolation is site-specific and was not researched.
