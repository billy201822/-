# Ducted (吊隱式) whole-floor dehumidifier in a Taiwan townhouse 2F: sizing, ducting, ERV (Lossnay LGH-35RVX3-E) + split-AC integration, drainage, maintenance

Context: 2F only, living ~30 m² + master bedroom ~22 m² (= 52 m² = about 15.7 坪 at 3.3058 m²/坪). Laundry and bathroom are at the far rear and have their own exhaust. Preferred plant location is an under-stair storage room with no ceiling, with drainage from a former toilet. The fallback is the laundry ceiling near the partition.

Limitation for the report writer: `www.medole.com.tw` and `www.100.com.tw` could not be fetched directly because those hosts are blocked by this session's network policy. All Medole and 100室內設計 data below comes from search-engine extracts of those pages, which quote the pages but could not be checked line by line. Mitsubishi and US code data also comes from search extracts of the PDFs and pages linked.

## 1. Medole 米多力 MD-70LBD: specs, sizing (L/day vs area), duct tolerance and number of supply branches

### Takeaway
The MD-70LBD is rated 70 L/day at 30°C/80% RH, with 420 CMH, 540 W, a 3/4" gravity drain and E.F. 2.70 L/kWh. Its external static pressure, duct-collar size and noise in dB are not published on the pages I could reach. Medole's own accessories (a 4-way supply box with 4" collars for 40 L/70 L units, and a φ6" 420 CMH / 300 Pa inline booster fan) point to a design of one 6" trunk feeding about 4 × 4" branches. A 70 L/day-rated unit is generously sized for about 16 坪, but its real capacity at room conditions is probably about half the nameplate figure.

### Cited Findings
- MD-70LBD manufacturer specs:
  - 除濕能力 70 L/日 at DB30°C / RH80%; 能源因數值 (E.F.) 2.70 L/kWh.
  - 220 V / 1φ / 60 Hz; 消耗電功率 540 W; 風量 420 CMH; refrigerant R-410A.
  - Drain: gravity, through a 3/4" pipe. Has a full-water auto-stop warning.
  - Operating range 5–40°C; humidity set-point range RH 20–90%.
  - Dimensions 845 × 485 × 310 mm.
  - Comes with a two-sided filter (formaldehyde/odour). App/Wi-Fi control, an air-quality sensor and a UV sterilizer are optional.
  - Source: [Medole MD-70LBD product page](https://www.medole.com.tw/md-70lbd.html), via search extract.
- Conflicting data:
  - A reseller lists 845 × 467 × 310 and a 16 A start-up current. The manufacturer page lists 19 A. Source: [ye888 reseller listing](https://www.ye888.com.tw/ec99/rwd1295/product.asp?prodid=md-70lbd) vs [Medole](https://www.medole.com.tw/md-70lbd.html).
  - Treat the manufacturer figures as authoritative.
- Noise: the official page only claims "多層隔音、超低噪音設計". It gives no dB value. — [Medole MD-70LBD](https://www.medole.com.tw/md-70lbd.html), via search extract.
- Static pressure and duct collar size are not listed on the product page. — [Medole MD-70LBD](https://www.medole.com.tw/md-70lbd.html), via search extract.
- Medole accessories:
  - 「四孔出風箱」 (4-outlet supply plenum) fits 40 L and 70 L models and has 4" flanges. — [Medole accessory: 四孔出風箱](https://www.medole.com.tw/show-1330073.html)
  - 「斜流風機」 (mixed-flow inline booster fan) is φ6", 420 CMH, 300 Pa static pressure. — [Medole accessory: 斜流風機 φ6" 420CMH](https://www.medole.com.tw/show-1105877.html)
- A Medole 8-key control panel manual PDF exists for its ducted range but could not be read. — [Medole 吊隱式風管除濕機 8Key 控面板說明書 (PDF)](https://www.medole.com.tw/uploadfiles/982/%E5%90%8A%E9%9A%B1%E5%BC%8F%E9%A2%A8%E7%AE%A1%E9%99%A4%E6%BF%95%E6%A9%9F-8Key%E6%8E%A7%E9%9D%A2%E6%9D%BF%E8%AA%AA%E6%98%8E%E6%9B%B8.pdf)
- Price, unit only:
  - NT$53,300 list, or NT$46,900 with a promo code. — [宏騰興 reseller](https://htx4379.waca.ec/product/detail/1777408)
  - NT$42,000 without installation. — [ye888](https://www.ye888.com.tw/ec99/rwd1295/product.asp?prodid=md-70lbd)
- Area guidance is rule-of-thumb from Taiwanese sources and is inconsistent:
  - A single-zone unit suits about 8–10 坪, and one unit for whole-house dehumidification suits only about 25 坪. — [100室內設計 article 14098/9641 via search extract](https://www.100.com.tw/article/9641)
  - Another source says a whole-house unit can serve 20–30 坪. — [FENNEY 冷氣幫 guide](https://fenney.tw/blog/guide-to-concealed-dehumidifiers/)
  - The extract did not make clear which source gave which figure.
- Duct-length and static-pressure tolerance: no Medole data was found. For comparison, design limits from a US ducted-dehumidifier maker (Aprilaire, a different product, used only as an analogue):
  - Aprilaire E080 supply-side external static pressure must not exceed 0.4" w.c. (about 100 Pa); for another E-series model the limit is 0.6" w.c. (about 150 Pa). — [Aprilaire E080/E100/E100H installation guide](https://abrwholesalers.com/media/assets/product/documents/aprilaire/dehumidifier/eseries/aprilaire-e080-e100-e100h-dehumidifier-installation-guide.pdf)
  - Aprilaire 1750A maximum static pressure is 0.8" w.c., and 1770A is 1.5" w.c. — [Aprilaire 1750A/1770A guide](https://manuals.plus/aprilaire/1750a-1770a-dehumidifiers-manual)
  - "Elbows, turns, and the static pressure of the HVAC equipment will affect the airflow through the dehumidifier." — same Aprilaire 1750A/1770A guide.
- Taiwanese designer guidance on duct runs: use 45° turns and avoid 90° elbows to limit pressure loss. When sharing ducts with an ERV, put the dehumidifier close to the main duct and convenient for drainage. — [100室內設計: 除濕機搭配全熱交換器，有沒有什麼限制？](https://www.100.com.tw/v2/article/6105), via search extract.

### Inferences
- **Real capacity: about 35 L/day, not 70.**
  - 540 W × 24 h = 12.96 kWh/day. 70 L ÷ 12.96 kWh ≈ 5.4 L/kWh, which does not match the stated E.F. of 2.70 L/kWh.
  - So the E.F. and the 70 L/day figure must refer to different test conditions. Taiwan's energy-label test condition is, to my understanding, about 27°C/60% RH, but I did not verify this here.
  - If E.F. 2.70 applies at about 540 W, then 2.70 × 0.54 × 24 ≈ **35 L/day** at milder, room-like conditions.
  - The nameplate 70 L/day is a hot/very humid rating point (30°C/80%). Plan on roughly 30–40 L/day under real indoor conditions (about 26–28°C, 60–70% RH). This is still ample for about 16 坪 if the envelope is reasonably tight.
- **Air change rate.** 52 m² × about 2.8 m ≈ 146 m³. At 420 CMH that is about 2.9 recirculation air changes per hour, which is a reasonable whole-floor mixing rate.
- **Trunk size.** 420 CMH in a 6" (152 mm) duct runs at about 6.4 m/s. That is acceptable for a short trunk in a plant room but noisy if it ends near bedrooms. Medole's φ6"/420 CMH booster accessory suggests 6" is the brand's matched trunk size.
- **Branches.**
  - 4 × 4" branches at 105 CMH each run at about 3.6 m/s.
  - 2 × 4" branches at 210 CMH each would run at about 7.2 m/s, which is too fast and noisy.
  - Recommended: 3–4 branches of 4", or 2 branches of 5" (about 4.6 m/s), with a balancing damper per branch.
  - The common residential targets of ≤3–4 m/s for branches and ≤5 m/s for the trunk are unsourced rules of thumb.
- **Split by area.** Living 30 m² vs master 22 m² is roughly 58/42. That suggests 2 outlets in living and 1–2 in master (for example, 2 + 2 using the Medole 4-way box).
- **Booster fan.** Medole sells a 300 Pa booster fan, which implies that long duct runs or many fittings may exceed the main unit's own fan capability. Keep runs short (the plant room is roughly central) and keep total fittings low. Ask Medole for the rated external static pressure (ESP) and the airflow at that ESP.

### Gaps
- The MD-70LBD's ESP (Pa), fan curve, inlet/outlet collar dimensions, noise (dB(A)), weight, minimum service clearances and maximum duct length were not found. The installation manual could not be retrieved because medole.com.tw is blocked in this session. Ask Medole or the installer for the 安裝說明書.
- I could not verify whether the 70 L/day and the 2.70 L/kWh figures are at different test conditions, nor the exact CNS test condition.
- No Taiwanese source gives a recommended number of outlets per 坪 for ducted dehumidifiers.

## 2. Return and supply placement, recirculation vs fresh-air mixing, and whether to connect ERV SA into the dehumidifier return (串接)

### Takeaway
The safest and most commonly recommended arrangement is to keep the two duct systems separate. If they are combined, the airflows and static pressures have to be calculated, because the ERV and dehumidifier move different volumes and can disturb each other (turbulence, noise, imbalance). Feeding ERV fresh air into the dehumidifier's intake has a precedent: Aprilaire's ventilating dehumidifiers draw outdoor air into the dehumidifier inlet to pre-dry it. With a powered ERV, though, it should be a "loose" connection: the ERV SA ends in an open return plenum or room, not hard-ducted to the dehumidifier inlet. Do not put returns in toilets or kitchens.

### Cited Findings
- How ducted dehumidifiers work: the unit is hidden in the ceiling and connects by ducts to supply and return grilles in each room. It draws in humid indoor air, dries it, and sends it back. — [PRO360 老屋翻新除濕機指南](https://www.pro360.com.tw/guide/old_house_reno_dehumidifier)
- Return location:
  - Toilets (廁所) and kitchens are unsuitable for return grilles, because they would carry grease and odours to other rooms. — Taiwanese installation guide via search extract ([100室內設計 9641](https://www.100.com.tw/article/9641) / [LINE Today](https://today.line.me/tw/v3/article/LX3WeRM))
  - Medium and large homes suit multi-point supply/return designs, but no number was given. — same extract.
- Sharing ducts between an ERV and a dehumidifier (Taiwanese designer article):
  - Ceiling space is limited, so the two machines' ducts are often combined through a 分風箱 or dampers.
  - The ERV's airflow usually differs from the dehumidifier's, which easily causes 擾流 (turbulence), noise and lower efficiency.
  - "如果使用共管在聲音與技術上需要精準計算，如果天花配置空間有餘裕，還是建議分管較好。"
  - Source: [100室內設計: 除濕機搭配全熱交換器，有沒有什麼限制？](https://www.100.com.tw/v2/article/6105), via search extract.
- Manufacturer precedent for mixing fresh air into a dehumidifier inlet (Aprilaire, US):
  - Ventilation air comes in through a normally-closed damper and an outdoor-air duct.
  - The installer measures the negative static pressure at the point where the fresh-air duct enters the return or the dehumidifier inlet, then uses a table to estimate the ventilation CFM.
  - "a longer fresh air intake duct or lower return static pressure will increase the ventilation time required."
  - Source: [Aprilaire 1830/1850 installation instructions](https://www.achooallergy.com/user_manuals/aprilaire-1830-1850-install-manual.pdf); [Aprilaire 1870](https://esmithair.com/wp-content/uploads/2020/02/Aprilare-Dehumidifiers_1870.pdf)
- Aprilaire layout rules:
  - Preferred installation is "return-to-return": pull air from, and send dried air back to, the HVAC return.
  - For "return-to-supply", "allow adequate space before the first branch duct to ensure the warm dehumidified air is thoroughly mixed".
  - Use at least 12" of flex duct at the dehumidifier inlet and outlet to stop vibration noise reaching the ducts.
  - Use insulated duct where the dehumidifier sits in unconditioned space.
  - Source: [Aprilaire manuals via search](https://documents.alpinehomeair.com/product/Aprilaire%201700%20-%20Safety%20and%20Installation%20Instructions.pdf); [Aprilaire E080/E100](https://abrwholesalers.com/media/assets/product/documents/aprilaire/dehumidifier/eseries/aprilaire-e080-e100-e100h-dehumidifier-installation-guide.pdf)
- Building-science forum view on an inline dehumidifier on the ERV supply:
  - Dehumidifiers "can't vary their output to the demand of the ERV".
  - Running one under over- or negative pressure relative to the ERV fans "could damage the ERV".
  - The suggested workaround is an air handler that circulates the larger of the ERV or dehumidifier flow.
  - This is practitioner opinion. — [GreenBuildingAdvisor: ventilating dehumidifier vs ERV + dehumidifier](https://www.greenbuildingadvisor.com/question/ventilating-dehumidifier-vs-erv-dehumidifier-for-hot-humid-climate); [GBA: HRV/ERV with integrated dehumidifier](https://www.greenbuildingadvisor.com/question/why-nobody-makes-an-hrv-erv-with-integrated-dehumidifier)
- Lossnay LGH-35RVX3-E fan data (relevant to pressure interaction):
  - Airflow 350 / 263 / 175 / 88 m³/h across 4 speeds.
  - External static pressure SP1–SP4 = 10 / 40 / 90 / 160 Pa. Another listing says "350 m³/h @ 100 Pa", so check the datasheet.
  - Duct connection 150 mm.
  - Source: [ShopClima LGH-35RVX3-E](https://www.shopclima.it/en/mitsubishi-electric-lgh-35rvx3-e-lossnay-enthalpic-heat-recovery-unit-for-horizontal-or-vertical-installation-350-m3-h.html); [BPC Ventilation](https://bpcventilation.com/products/mitsubishi-lossnay-lgh-35rvx3-e); [Airconditioning-online AU](https://www.airconditioning-online.com.au/product/mitsubishi-electric-lossnay-heat-recovery-ventilation-lgh-35rvx3-e/)

### Inferences
- **Pros of 串接 (ERV SA → dehumidifier return side):**
  - Fresh air is dried before it is distributed, the same principle as Aprilaire's design.
  - The dehumidifier's supply ducts deliver the fresh air too, so the ERV needs fewer or no separate SA branches. The ERV SA and dehumidifier ducts both enter the same plant room.
  - It also gives the fresh air some reheat (see section 3), which can be welcome in spring and in plum-rain (梅雨) weather.
- **Cons and risks of a hard, sealed connection** (ERV SA duct bolted straight to the dehumidifier inlet):
  - **Flow mismatch.** The dehumidifier wants 420 CMH, but the ERV delivers 88–350 m³/h. A sealed connection either starves the dehumidifier or forces the ERV SA fan to supply more than intended.
  - **Pressure imbalance.** The dehumidifier's suction lowers the pressure at the ERV SA outlet. The SA fan then sees less resistance and moves more air than the EA fan, which unbalances the ERV, pressurizes the house and lowers core efficiency.
  - **Unit off, ERV on.** The ERV must push through the dehumidifier's coil and filter, adding resistance. The SA flow drops, especially at the low speeds that have only 10–40 Pa available.
  - **ERV off, unit on.** Outdoor air can be pulled backwards through the idle ERV. A motorized or back-draft damper is needed.
  - **Control.** Each unit's control assumes its own airflow. This matches the GBA warning.
- **Recommended combined design ("loose coupling"):**
  - Run the ERV SA into a return plenum, or into the storage room itself.
  - That space must also have a large open return path from the living area: a return grille or louvred door sized for at least 420 CMH at low velocity.
  - The dehumidifier then draws mostly room air plus the ERV air, and the pressure at the ERV SA outlet stays near neutral.
  - Keep the ERV's 3–4 speed settings and its EA from the living area unchanged.
  - Mixing must happen before the coil, with no direct jet of ERV air onto the coil sensor. The unit's RH sensor is typically at the return, so a jet of humid outdoor air hitting it could make the unit run constantly. This last point is my assumption.
- **Return arrangement for this floor:**
  - One central return near the stair or plant room, or the plant-room door/louvre itself acting as the return.
  - Transfer paths are needed from the master bedroom (door undercut or transfer grille), or the bedroom will pressurize and its supply flow will drop. This is a common practice rule of thumb and is unsourced.
  - Do not put a return in the bathroom (sourced above).
  - Avoid a return in the laundry: lint would clog the filter, and the room's exhaust fan would compete (inference).
- **Supply placement:**
  - Put outlets on the far sides of the living room and bedroom, away from the return, so the dried air sweeps the room.
  - Aim them away from beds and sofas, because the supply air is warm (see section 3).
  - Place a supply near the AC indoor unit's return so the AC can absorb the reheat.
- **Fallback location (laundry ceiling):** shorter drain, but the duct runs to the living room and master bedroom get longer. It also needs an access hatch (section 5) and puts the unit in a lint/humid zone with a competing exhaust fan. Inference.

### Gaps
- Mitsubishi's Lossnay technical manual has guidance on connecting Lossnay SA to air-conditioner or fan-unit returns (direct vs indirect connection), but it was not retrieved here. Look for it, since it is the manufacturer's own rule for the ERV side.
- No Medole statement was found on whether fresh air or ERV air may be ducted into the MD-70LBD inlet, or on its allowable inlet negative pressure.
- No Taiwanese contractor article with measured airflows for 全熱交換器串接除濕機 was found. The [Mobile01 user thread](https://www.mobile01.com/topicdetail.php?f=731&t=6607871) on 全室除濕 + 全熱交換 exists, but only a snippet was visible.

## 3. Expected humidity performance in Taiwan summers and plum rain; target RH; interaction with ERV enthalpy core, split-AC dry mode and reheat

### Takeaway
An ERV's enthalpy core reduces, but does not remove, the moisture brought in by ventilation. In plum rain, an ERV on high speed can add a moisture load comparable to a large share of the dehumidifier's real capacity. A split AC in dry mode removes moisture only while it is cooling. Inverter units struggle with latent load at part-load, so a dehumidifier is the main tool when it is mild and wet. A dehumidifier turns all removed latent heat, plus its own electrical input, into sensible heat. That means warm supply air: an estimated 1–1.5 kW for this unit in real use. In summer the AC must remove that heat.

### Cited Findings
- ERV and humidity:
  - Enthalpy-type (全熱) exchangers transfer both heat and moisture, so incoming air is less humid, but they do not actively dehumidify. — [Poll-tex 全熱交換機 knowledge page](https://www.poll-tex.com.tw/knowledge/energy-recovery-ventilator/)
  - "全熱交換器只能交換部分濕度，台灣梅雨季及高濕度環境仍可能需要冷氣或除濕機". — [達瑞克 2026 全熱交換器推薦](https://www.da-rank.com/blog/heat-recovery-ventilator-recommendation-2026); [100室內設計 6369](https://www.100.com.tw/article/6369)
  - One Taiwanese source warns that an ERV brings in humid outdoor air. Even with a conventional dehumidifier, "室內濕度依然不穩定". — [沃特奇 (vendor) 全熱交換器優缺點](https://vortexfresh.com.tw/advantagesanddisadvantagesoffullheatexchanger/). This is a vendor promoting an integrated product, so it may be biased.
  - In Taiwan, when the AC is dehumidifying, an ERV can exhaust humid indoor air and bring in drier fresh air, helping keep humidity steady. — [100室內設計 6105](https://www.100.com.tw/v2/article/6105), via search extract. This claim only holds when outdoor air is drier than indoor air, which is rare in Taiwan summers.
- Lossnay LGH-35RVX3-E enthalpy efficiency:
  - Cooling 82 / 78 / 73 / 71% at speeds 1→4; heating 83.5 / 78.5 / 74 / 71.5%. Efficiency falls as airflow rises.
  - Other listings give 66.5% cooling temperature (sensible) efficiency at maximum speed. That is a different metric.
  - Source: [ShopClima](https://www.shopclima.it/en/mitsubishi-electric-lgh-35rvx3-e-lossnay-enthalpic-heat-recovery-unit-for-horizontal-or-vertical-installation-350-m3-h.html); [Airconditioning-online AU](https://www.airconditioning-online.com.au/product/mitsubishi-electric-lossnay-heat-recovery-ventilation-lgh-35rvx3-e/)
- Debate on ERVs in hot-humid climates:
  - One GBA expert says there is "very little energy recovery" when the indoor-outdoor temperature difference is small.
  - Another calls ERVs in cooling-dominated climates "a silly idea".
  - Ventilating dehumidifiers are framed as suiting warm climates.
  - Source: [GBA: running ERV in humid summer](https://www.greenbuildingadvisor.com/question/running-erv-in-humid-summer); [GBA: ERV system too much humidity](https://www.greenbuildingadvisor.com/question/erv-system-too-much-humidity); [GBA: ventilating dehumidifier vs ERV](https://www.greenbuildingadvisor.com/question/ventilating-dehumidifier-instead-of-erv)
- Heat output: "A dehumidifier converts latent load into sensible heat, and this extra heat has to be rejected by the cooling system anyways." — [GBA: dehumidification and minisplits](https://www.greenbuildingadvisor.com/question/dehumidification-and-or-vs-mini-splits)
- Aprilaire's own manuals call the output "warm dehumidified air" and require mixing before the first branch. — [Aprilaire E080/E100 guide](https://abrwholesalers.com/media/assets/product/documents/aprilaire/dehumidifier/eseries/aprilaire-e080-e100-e100h-dehumidifier-installation-guide.pdf)
- Split AC dry mode:
  - The unit "still cools but the balance between latent and sensible is tipped more to latent". Efficiency drops somewhat, but this is "still more efficient than throwing ever more dehumidifier at the problem". Lowering blower speed in cooling mode also helps. — [GBA: dehumidification and minisplits](https://www.greenbuildingadvisor.com/question/dehumidification-and-or-vs-mini-splits)
  - Inverter units modulate, so they struggle with latent loads at part-load in humid climates, and oversizing makes this worse. — [HVAC Know It All: mini-split dehumidification](https://hvacknowitall.com/blog/mini-split-dehumidification-the-problem-nobody-warned-you-about)
  - Mini-splits do not dehumidify in heating mode. — [Innovative Dehumidifiers](https://www.innovativedehumidifiers.com/the-truth-behind-mini-split-systems/)
  - Contractor rule of thumb: if indoor RH stays above 60% despite a correctly sized mini-split and dry mode, add supplemental dehumidification. — [Budget Heating & AC](https://www.budgetheating.com/mini-split-humidity-control-for-year-round-comfor/)
- Target RH: a vendor of an integrated ERV-plus-desiccant unit claims it keeps supply RH at about 50–60%. This is marketing and unverified. — [沃特奇 全熱除濕一體機](https://tw-vortex.weebly.com/20840291053850028629199683963627231.html)

### Inferences
These are my calculations; the assumptions are stated.
- **ERV moisture load, plum rain.**
  - Assumptions: outdoor 25°C/95% (humidity ratio about 19.0 g/kg); indoor target 26°C/55% (about 11.6 g/kg); difference about 7.4 g/kg.
  - At ERV speed 2 (175 m³/h ≈ 205 kg/h), the moisture brought in without recovery would be about 36 L/day.
  - With 70% latent recovery, the residual is about 11 L/day. With a more conservative 50%, about 18 L/day.
  - At speed 4 (350 m³/h) the figures double: about 22–36 L/day.
  - Compare that with the MD-70LBD's estimated 30–40 L/day real capacity (section 1). In plum rain the ERV should run at low speed (speed 1–2), consistent with the required ventilation rate. Otherwise the dehumidifier spends most of its capacity on ventilation air.
  - Latent efficiency is usually lower than the quoted enthalpy efficiency, but I did not find Lossnay's latent figure.
- **Summer, 32°C/65% outdoor (about 19.6 g/kg).** The moisture difference is similar (about 8 g/kg), so the loads are similar. The ERV still adds moisture. The AC in cooling mode carries much of the latent load while it runs, and the dehumidifier tops up at night or during low-load hours.
- **Heat output.**
  - Latent heat of condensation is about 0.68 kWh per litre.
  - At about 35 L/day (1.46 L/h): about 1.0 kW latent becomes sensible, plus about 0.54 kW electrical, for about 1.5 kW total. That is roughly 0.43 RT or 1,300 kcal/h.
  - At the 70 L/day rating point: about 2.5 kW.
  - Spread over 420 CMH (about 0.137 kg/s), that implies supply air about 10 K warmer than the return air in real use, assuming all heat goes into the airstream.
  - Consequences:
    - In summer with the AC on, the AC must remove this extra 1–1.5 kW. That is a sizeable fraction of a typical 5–7 kW split serving 52 m².
    - In plum rain and spring (22–26°C), the reheat is useful. It acts like "dehumidify without overcooling", which an AC in dry mode cannot do well.
- **Operating strategy:**
  - Use the dehumidifier as the primary humidity control in plum rain, spring, autumn and mild humid days.
  - In hot summer, let the AC (cooling, low fan, or dry mode) carry the latent load. Set the dehumidifier's set-point slightly above the AC-controlled level (for example 60% RH) so it only tops up and does not fight the AC with heat.
  - A target of 50–60% RH is reasonable. Below about 50% the energy cost rises steeply; this is an unsourced rule of thumb.
- **When a supply jet is near the AC return,** the AC sees warmer return air and may run harder in cooling mode. That is acceptable, but do not let the dehumidifier supply blow directly onto the AC's thermistor or the room thermostat.

### Gaps
- No measured data was found on RH achieved by Taiwanese ducted dehumidifiers in plum rain, and no authoritative Taiwanese RH target (for example from 國健署 or 營建署). Commonly cited targets such as ≤60% RH (EPA/ASHRAE) were not verified in this research.
- The latent (moisture) efficiency of the LGH-35RVX3-E core was not found; only total enthalpy and temperature efficiencies were.
- No source was found on the MD-70LBD's actual supply-air temperature rise or its capacity at 26–27°C/60–70% RH.

## 4. Condensate drain requirements: slope, trap, air break, connecting to a former toilet or soil stack, condensate pump

### Takeaway
Medole specifies only a 3/4" gravity drain. Detailed slope and trap rules are not available from Medole, so use code-level practice. Slope at least 1/100 (1/8 in/ft), with 1/50 preferred for long runs. Discharge indirectly through an air gap or air break into a trapped, vented receptor. Never hard-connect the condensate line to a soil pipe. A former toilet's soil stub has no trap once the toilet is removed (the trap was inside the WC). So it needs a proper trap or floor-trap fitting that will not dry out, plus an air break, before the dehumidifier drain can go to it. If gravity is not possible, use a condensate relay pump (中繼排水加壓器), which Taiwanese installers commonly include.

### Cited Findings
- MD-70LBD drain: gravity drainage through a 3/4" pipe, with a full-water auto-stop. — [Medole MD-70LBD](https://www.medole.com.tw/md-70lbd.html), via search extract.
- Taiwanese practice:
  - Plan the drain slope, route and outlet before construction to avoid backflow (逆流). — [LINE Today 吊隱式除濕機 article](https://today.line.me/tw/v3/article/PGQq5jl)
  - A Costco Taiwan ducted-dehumidifier listing says basic installation includes drainage work and a 中繼排水加壓器 (relay drain pump). — [Costco TW item 112445](https://www.costco.com.tw/Exhibitions/Appliances/p/112445)
  - General drainage-pipe slope is about 1:50 to 1:100 downward. — [100室內設計 article via search extract](https://www.100.com.tw/article/11288)
- Manufacturer drain-hose guidance (Panasonic, portable units, a general principle):
  - Avoid kinks and up-down undulations in the hose, or poor drainage can cause leaks.
  - Insulate the pipe where condensation can form on it. — [Panasonic Taiwan FAQ 3016](https://pstw.panasonic.com.tw/FAQ/Article/3016)
- US model-code rules (UMC/CMC/UPC, used as a reference standard, not Taiwan code):
  - Minimum condensate slope is 1/8 in per ft, about 1% or 1/96. — [UpCodes: Condensate Waste and Control](https://up.codes/s/condensate-waste-and-control); [Riverside CA CMC handout](https://www.riversideca.gov/cedd/sites/riversideca.gov.cedd/files/pdf/building/forms/Inspections_page_handouts/CALIFORNIA%20MECHANICAL%20CODE%20RESIDENTIALCONDENSATE%20DISPOSAL%20REQUIREMENTS.pdf)
  - Some specifiers call for 1/4 in per ft (about 2%, or 1/48) on long horizontal runs for reliability. — [Anvilfield condensate field guide](https://anvilfield.com/field-guides/hvac/condensate-drain-trap-management/)
  - Condensate must discharge indirectly through an air gap or air break into a trapped, vented receptor, a dry well or a fixture tailpiece. CPC 801.2 requires at least a 1" vertical air gap above the receptor's flood rim. — [Town of Truckee condensate handout](https://townoftruckee.gov/DocumentCenter/View/106/Condensate-Waste-PDF?bidId=)
  - The receptor's P-trap must be vented so its seal isn't siphoned. The minimum drain is 3/4" and never smaller than the unit's outlet. — [HQ Plumbing & Air](https://hqplumbingandair.com/resources/faqs/air-conditioner-condensate-drain-rules)
  - The equipment's own drain trap follows the manufacturer's instructions, and a condensate pump is an allowed option. — [Riverside CA handout](https://www.riversideca.gov/cedd/sites/riversideca.gov.cedd/files/pdf/building/forms/Inspections_page_handouts/CALIFORNIA%20MECHANICAL%20CODE%20RESIDENTIALCONDENSATE%20DISPOSAL%20REQUIREMENTS.pdf)
- Traps and odour:
  - A trap's 水封 (water seal) blocks sewer odour and insects. Once the seal dries out or is siphoned, odour control fails.
  - Positive or negative pressure in the drain system can push out or pull out the seal, so drains need venting (通氣管).
  - Source: [OPEN Design: 存水彎 guide](https://www.openworld.tv/blog/plumbing-trap-guide.html); [金高電: 什麼是存水彎](https://www.gigataiwan.com.tw/news-detail/35/)

### Inferences
- **Former toilet stub:**
  - A floor-mounted WC has its trap built into the bowl, so the remaining 4" soil stub is an open, untrapped sewer opening.
  - Recommended sequence: seal the stub with a reducer to a trapped receptor (a P-trap, or a 防臭 floor-drain/落水頭 fitting). Then run the dehumidifier hose so it ends above that receptor with a visible air gap (≥25 mm, following the CPC concept) or a proprietary air-break fitting (tundish).
  - This gives odour protection (the trap seal), backflow protection (sewage cannot surcharge into the dehumidifier pan), and inspectability.
  - These are code-concept inferences; I found no Taiwanese rule specific to dehumidifiers.
- **Dry-trap risk.** Condensate flows only when the unit runs, so the trap may dry out in winter. Use a trap with a mechanical or waterless anti-odour valve (e.g. a 防臭杯 / check-valve trap), or top it up seasonally. A floor drain fed occasionally by a nearby basin would also keep it primed.
- **Avoid double trapping.** That means an unvented trap at the unit plus another trap downstream with no air break in between, which can air-lock. The air break solves this.
- **Trap at the unit.** If the MD-70LBD's fan draws air through the coil, the drain pan is under negative pressure. Without a trap, air would be sucked up the drain and water could back up or spit out. A trap, or the manufacturer's built-in arrangement, is usually needed there.
  - This is a general HVAC principle and an inference, not a Medole statement. Ask Medole whether the 3/4" outlet needs an external trap and how deep.
- **Slope target.**
  - At 1/100, a 3 m run drops 30 mm; at 1/50, it drops 60 mm.
  - With the unit at floor or shelf level in a room with no ceiling, gravity to a floor-level toilet stub may be marginal. Mounting the unit on a raised bracket or shelf gives fall; otherwise use a relay pump.
  - In the laundry-ceiling fallback, gravity to the laundry floor drain is easy.
- **Pipe material.** Use 3/4" PVC with insulation over its whole length (Panasonic's condensation warning). Add a cleanout or tee near the unit for flushing algae and slime.

### Gaps
- No Medole drain-installation details were found: required slope, external trap requirement or depth, or a pump option. The manual was inaccessible.
- No Taiwanese building or plumbing code clause (建築技術規則 / 自來水用戶用水設備標準 / 排水設備) specific to condensate drains or to connecting into soil (污水/糞管) pipes was found. A licensed plumber (水電) should confirm whether connecting into a 糞管 vs 雜排水管 is permitted locally.
- Condensate pump models, head and flow ratings, and noise were not researched in detail.

## 5. Maintenance, access, cost, noise and the no-ceiling equipment room

### Takeaway
Clean the dehumidifier filter often: every 2 weeks to 2 months in humid use, per Taiwanese manuals and articles. Clean the Lossnay filters at least yearly and its cores every 1–2 years, vacuum only and never washed. Service access needs at least a 40 × 60 cm hatch (some say 80 × 40 cm) and about 45 cm ceiling void if the unit is ceiling-hung. A no-ceiling under-stair plant room is better for access than either location. Its weak points are noise breakout (the compressor is right inside the room), drain fall, and making sure the room works as a proper return plenum.

### Cited Findings
- Ducted dehumidifier filters:
  - Taiwanese articles conflict: one says "一般2個月清1次，環境潮濕建議更勤", another says every 6 months to 1 year depending on conditions.
  - Method: vacuum, or wash with water and a neutral detergent, then dry in the shade and refit.
  - Source: [100室內設計 2050/9641 via search extract](https://www.100.com.tw/article/2050); [FENNEY 冷氣幫](https://fenney.tw/blog/guide-to-concealed-dehumidifiers/)
  - The MAXE 萬士益 LND series ducted dehumidifier manual (per search extract) recommends cleaning the filter every two weeks with warm, not hot, water. The search tool described it as not ducted-specific, but the PDF title is "LND吊隱式除濕機系列說明書". — [MAXE LND manual PDF](https://www.maxe.com.tw/Web/Maxe/package/WebSite/PublicDownload/LND%E5%90%8A%E9%9A%B1%E5%BC%8F%E9%99%A4%E6%BF%95%E6%A9%9F%E7%B3%BB%E5%88%97%E8%AA%AA%E6%98%8E%E6%9B%B8.pdf)
- Access and ceiling void:
  - Access hatch at least 80 × 40 cm per one source, or at least 40 × 60 cm so the filter can be pulled out per another. — [100室內設計 / LINE Today extracts](https://today.line.me/tw/v3/article/LX3WeRM); [100室內設計 9641](https://www.100.com.tw/article/9641)
  - Ceiling void at least about 45 cm. If space is lacking, consider a balcony or corridor location, and leave a service opening. — [LINE Today](https://today.line.me/tw/v3/article/PGQq5jl)
  - Ducted ERVs also need ducts in the ceiling plus inspection hatches, which raises up-front cost. Filters and cores need regular inspection or replacement, or efficiency drops and bacteria can grow. — [100室內設計 6105 via search extract](https://www.100.com.tw/v2/article/6105)
- Lossnay LGH-RVX3-E family maintenance (from LGH-15RVX3-E / RVX documents covering the same family):
  - "Guideline: Clean the air filters once a year."
  - "Clean the Lossnay cores once [every] two year[s]. (Clean the Lossnay cores once a year if possible.) (Frequency should be increased depending on the extent of dirt.)"
  - Cores: vacuum the exposed surfaces, soft brush only, "Do NOT wash in water."
  - The controller's maintenance-indicator interval can be set from 100 to 9,900 h.
  - Source: [Mitsubishi NZ LGH-RVX3-E installation manual](https://www.mitsubishi-electric.co.nz/materials/ventilation/manuals/lossnay/lgh-rvx3-e/2_installation/im_lgh-15-200rvx3-e.pdf); [Mitsubishi NZ how to clean filter/core LGH-RVX](https://www.mitsubishi-electric.co.nz/materials/ventilation/manuals/lossnay/lgh-rvx-e/1_operation/how-to-clean-your-filter-core-lgh-rvx.pdf); [ManualsLib Lossnay technical manual p.91](https://www.manualslib.com/manual/1571205/Mitsubishi-Electric-Lossnay-Series.html?page=91)
  - Replacement G4 filter sets for the LGH-35RVX3 are sold aftermarket. — [cleanfilter.eu](https://cleanfilter.eu/mitsubishi-lossnay-lgh-35rvx3-2xg4-filter-set-standard)
- LGH-35RVX3-E physical and noise data:
  - 888 × 874 × 331 mm, about 30 kg, 150 mm collars.
  - Noise about 17–32 dB(A) across speeds. Sources give either 30.5 or 32 dB(A) at top speed.
  - Input power about 120–140 W at maximum.
  - Source: [Airconditioning-online AU](https://www.airconditioning-online.com.au/product/mitsubishi-electric-lossnay-heat-recovery-ventilation-lgh-35rvx3-e/); [BPC Ventilation](https://bpcventilation.com/products/mitsubishi-lossnay-lgh-35rvx3-e); [ShopClima](https://www.shopclima.it/en/mitsubishi-electric-lgh-35rvx3-e-lossnay-enthalpic-heat-recovery-unit-for-horizontal-or-vertical-installation-350-m3-h.html)
- Noise:
  - Medole gives no dB figure, only "multi-layer insulation, ultra-low noise". — [Medole](https://www.medole.com.tw/md-70lbd.html)
  - Aprilaire requires at least 12" of flex duct at the inlet and outlet against vibration transmission. — [Aprilaire manuals](https://manuals.plus/m/2cf44a7a0d7b5c8198a67990737a0d74257ad842317e73778e7b3ba715d3f996)
- Cost:
  - MD-70LBD is NT$42,000–53,300 for the unit only. — [ye888](https://www.ye888.com.tw/ec99/rwd1295/product.asp?prodid=md-70lbd); [宏騰興](https://htx4379.waca.ec/product/detail/1777408)
  - A Taiwanese article on 吊隱式除濕機 price and installation cost exists, but its figures were not visible in the extracts. — [FENNEY 價格](https://fenney.tw/blog/price-of-concealed-dehumidifier/)

### Inferences
- **Maintenance schedule** (manufacturer intervals vs Taiwanese rules of thumb):
  - Dehumidifier return filter: check monthly in the humid season and clean every 2–8 weeks. Monthly checks are a sensible rule of thumb between the 2-week (MAXE manual) and 2-month (articles) figures.
  - Lossnay filters: Mitsubishi says "at least yearly"; in Taiwan's dusty and humid urban air, quarterly to half-yearly checks are prudent (inference).
  - Lossnay core: vacuum every 1–2 years (manufacturer), never wash.
  - Also check that the drain trap is primed, and flush the drain line once a year (inference).
  - If the ERV SA is fed into the dehumidifier return (串接), the dehumidifier filter also catches some outdoor dust, so it may load faster. The ERV's own SA filter should stay as the first stage.
- **No-ceiling under-stair room, pros:**
  - Full-face access for filters, ERV cores and the control board, with no hatch-size limits. The ERV's 888 × 874 mm footprint needs its core and filter panel side fully clear; check the clearance in Mitsubishi's installation manual.
  - Drain and pump are accessible.
  - The room can serve as the return plenum, using a louvred door or return grille.
- **No-ceiling under-stair room, cons:**
  - Compressor and fan noise radiate into the room. Line the room or door with acoustic material and keep the door solid with a separate return grille sized for low velocity, or use an acoustically lined return plenum.
  - Both units hanging from or on the stair structure can transmit vibration into the stair. Use anti-vibration mounts.
  - Gravity drain fall to the toilet stub may need the unit raised.
  - The MD-70LBD is designed for 吊隱 (ceiling-hung) mounting. Confirm with Medole whether shelf or floor mounting in the normal orientation is allowed, keeping the drain pan level.
- **Fallback, laundry ceiling:**
  - Needs a hatch of at least 60 × 40 cm, ideally 80 × 40 cm, on the filter/service side, plus at least 45 cm of void. The unit is 310 mm high, plus duct transitions.
  - Laundry lint means more frequent filter cleaning if the unit draws any local air.
  - The duct runs to the bedroom and living room are longer, and the higher ESP may push the unit towards needing the Medole booster fan.

### Gaps
- Medole maintenance intervals, filter specification and service clearances: the manual was inaccessible.
- The LGH-35RVX3-E specific operating manual was not read directly; the intervals come from same-family documents. Service clearance dimensions for the LGH-35RVX3-E were not found.
- Confirm that the -E (European-spec) LGH-35RVX3-E is rated for Taiwan's 220 V/60 Hz supply. I did not verify this, and the Taiwan-market model designation may differ.
- No sources were found on installed cost (labour, ducting, pump) for this combined system in Taiwan, or on measured noise of the MD-70LBD.
