# 室內 CO2 控制與新鮮外氣量：小型台灣住宅（2F 客廳 ~30 m² + 主臥 ~22 m²，Mitsubishi LGH-35RVX3-E）

> 研究方法說明：本次以 WebSearch 為主。WebFetch 在此雲端環境無法連到 pmc.ncbi.nlm.nih.gov 與 mitsubishi-electric.co.nz（DNS 不在允許網域），所以原始 PDF（Persily 2017 全文、三菱 CO2 感測器型錄、LGH-35RVX3-E 規格表）都沒有整份讀過，數字來自搜尋結果裡的原文片段與摘要。若要正式引用，建議開放這兩個網域後再核對原文。所有計算都是筆者依引用的輸入值推得，列在各節 Inferences。

---

## 1. 標準與指引：台灣室內空氣品質標準、台灣建築/住宅通風規定，與 ASHRAE 62.2、EN 16798-1、WHO 及臥室睡眠研究比較

### Takeaway
台灣法定的 CO2 限值是 **8 小時平均 1000 ppm**（室內空氣品質標準，2012），只管「公告場所」，不直接約束私人住宅。住宅端唯一的量化通風規定，是《建築技術規則建築設備編》第 102 條「設置機械通風時」臥室、起居室 **8 m³/h·m²**。這條按樓地板面積計，與人數無關，也沒定義是否必須是外氣。國際上，2025 年臥室睡眠文獻整合研究建議臥室 **≤1000 ppm、最好 ≤800 ppm**，約相當於每人 **8 L/s（≈29 m³/h）**，大約是多數住宅標準的兩倍。

### Cited Findings
**台灣：室內空氣品質標準（環保署 101.11.23 發布，現由環境部主管）**
- 二氧化碳 CO2 標準值：**8 小時值 1000 ppm**。依《室內空氣品質管理法》第 7 條第 2 項訂定。同條也列 CO、甲醛、TVOC、PM2.5 等項目 — [台北市法規附件：室內空氣品質標準 2012](https://www.laws.taipei.gov.tw/lawatt/Law/A040300030009600-20121123-2000-001.pdf)；[室內空氣品質標準表格 101.11（臺藝大）](https://portal2.ntua.edu.tw/~d09/dowmload/臺藝大法規-1011128/室內空氣品質管理法/室內空氣品質標準-表格-101.11.pdf)
- 「8 小時值」的定義：連續 8 小時各測值的算術平均，或 8 小時累計採樣的測值 — [室內空氣品質標準 2012](https://www.laws.taipei.gov.tw/lawatt/Law/A040300030009600-20121123-2000-001.pdf)
- 立法說明：1000 ppm 是參考多數國家的建議值或標準值；香港「卓越級」為 800 ppm。考量法案推動初期要減輕場所改善成本，所以採 1000 ppm — [室內空氣品質標準 2012](https://www.laws.taipei.gov.tw/lawatt/Law/A040300030009600-20121123-2000-001.pdf)
- 2005 年的建議值（舊制）：第一類（學校、醫療等有特別需求的場所）600 ppm，第二類（一般公共場所、辦公大樓）1000 ppm（依搜尋摘要，出處為下列教材/文件之一）— [文化大學環安資料](https://esh.pccu.edu.tw/var/file/19/1019/img/625/228241839.pdf)；[ISHA 資料](https://isha.org.tw/image/technology/safety/02/filedate/0620-5.pdf)
- 量測容許誤差：標準值在 1000 以下為原始數據 ±10%，1000（含）以上為 ±100 濃度單位 — [室內空氣品質標準（2022 附表修正版）](https://www.laws.taipei.gov.tw/lawatt/Law/A040300031015900-20220630-2000-001.pdf)

**台灣：建築技術規則建築設備編 第 102 條（機械通風量）**
- 「建築物供各種用途使用之空間，設置機械通風設備時，通風量不得小於左表規定」。「臥室、起居室、私人辦公室等容納人數不多者」為 **8 m³/h·m²**（兩欄皆 8）；辦公室、會客室 10；會議室、候診室等容納人數較多者 15 — [rootlaw 第102條附表 PDF](http://www.rootlaw.com.tw/Attach/L-Doc/A040040100000904-1061018-102000-001.pdf)；[LawPlayer 第102條（最新修正 111.12.29）](https://lawplayer.com/article/6438f5f0e800e5f0b933df49)
- 內政部研究報告評論：此表的通風量隨地板面積變動，與室內人員密度無關 — [內政部建研所研究報告](https://ws.moi.gov.tw/Download.ashx?u=LzAwMS9VcGxvYWQvT2xkRmlsZV9BYnJpX0dvdi9yZXNlYXJjaC81OTMvMTQ0NzkyOTgzMDEucGRm&n=Y29tcGxldGUucGRm)
- 內政部建築技術審議委員會（98 年）討論第 102 條修正：草案改依「使用類組人員密度」及「每 m² 所需新鮮外氣量」訂定，但會中也指出「新鮮外氣量」沒有明確定義 — [國土管理署會議紀錄](https://www.nlma.gov.tw/uploads/files/b0b198ed8d901e70472d990f974c7a87.pdf)

**台灣：新建住宅「空氣環境」性能評估表（住宅性能評估；非強制）**
- C 級以上：「符合法規，且機械通風引入新鮮外部空氣」，**臥室、起居室至少引入 4 m³/h·m² 新鮮外氣**。廚房 ≥32、浴廁 ≥23 m³/h·m²。B 級另要求浴廁獨立管道排風，A 級再要求天花板內空間與其他空間氣密隔絕。換算方式為通風設施性能（CMH）除以居室面積 — [rootlaw 附件 PDF（新建住宅空氣環境性能評估表）](https://www.rootlaw.com.tw/Attach/L-Doc/A040040100019800-1150720-3000-005.pdf)

**ASHRAE 62.2（美國住宅）**
- 全宅連續通風量：Qtot = 0.03·Afloor(ft²) + 7.5·(Nbr+1) cfm；SI 形式 **Qtot = 0.15·Afloor(m²) + 3.5·(Nbr+1) L/s**（62.2-2013 起）— [Retrotec Residential Ventilation Primer](https://retrotec.com/?p=3801)
- SI 版本中 Qtot 單位 L/s、Afloor m²，Nbr = 臥室數且不得小於 1 — [ASHRAE 62.2-2010 Addendum r](https://www.ashrae.org/File%20Library/Technical%20Resources/Standards%20and%20Guidelines/Standards%20Addenda/62_2_2010_addendum_r_Final.pdf)

**EN 16798-1（歐洲）**
- 非住宅、非適應者（non-adapted persons），CO2 高於室外的濃度與每人通風量：**Cat I 550 ppm（10 L/s·p）、Cat II 800 ppm（7 L/s·p）、Cat III 1350 ppm（4 L/s·p）** — [Olesen, AIVC 簡報](https://aivc.org/system/files/7-Bjarne%20Olesen.pdf)
- Eurovent IAQ 指引：推薦 >36 m³/h·p（10 L/s），可接受 25–36 m³/h·p（7–10 L/s）— [Eurovent 2024 IAQ flyer](https://www.eurovent.eu/wp-content/uploads/publications-files/2024-eurovent-iaq-flyer-web.pdf)
- 前身標準（搜尋摘要寫作「EN 15152」，應為 EN 15251）：新建住宅最大 CO2 為高於室外 500 ppm（Cat II），既有建築 800 ppm（Cat III）— [論文（core.ac.uk）](https://core.ac.uk/download/491283455.pdf)

**WHO 與其他**
- WHO 通風路線圖（COVID-19 背景，2021）：非醫療場所最低 **10 L/s·人**。原文沒說明是否包含住宅 — [BC Lung 摘要](https://bclung.ca/node/1332)
- 大量產生氣膠的空間另需 ≥15 L/s·人。「CO2 ≤800 ppm」是英國 SAGE-EMG 的建議，**不是 WHO 的** — [PMC8363431](https://pmc.ncbi.nlm.nih.gov/articles/PMC8363431/)
- 1999 年 LBNL 文獻回顧（以辦公室為主）：約一半的 CO2 研究顯示，CO2 低於 800 ppm 後，病態建築症候群風險仍隨濃度下降而顯著降低 — [LBNL: Association of ventilation rates and CO2 concentrations with health](https://indoor.lbl.gov/publications/association-ventilation-rates-and-co2)

**臥室 CO2 與睡眠的研究**
- **Akimoto 等 2025 整合研究**（17 篇研究、22 組實驗資料；Sekhar 為共同作者）：造成睡眠受擾的最低外氣通風量，約對應 **絕對 CO2 1000 ppm**。建議臥室 CO2 **≤1000 ppm，最好 ≤800 ppm**（CO2 作為通風是否足夠的指標，本身不視為污染物）。達標約需 **每人 8 L/s**，「至少是許多現行住宅標準的兩倍」 — [EurekAlert 新聞稿](https://www.eurekalert.org/news-releases/1102252)；[Waseda 新聞](https://www.waseda.jp/top/en/news/86065)；[DTU Orbit](https://orbit.dtu.dk/en/publications/new-research-on-bedroom-ventilation-and-sleep-quality-suggests-th/)
- 同一文獻脈絡的提醒：約 850 ppm 的「無影響點」因感測器精度與安全裕度考量，不能視為 NOAEL — [EurekAlert](https://www.eurekalert.org/news-releases/1102252)
- 丹麥研究脈絡（引用 Sekhar 等 2020 的暫定關係）：CO2 **<~750 ppm 不干擾睡眠，750–1150 ppm 可能干擾**；並提到丹麥臥室標準為 800 ppm（作者強調此關係仍待驗證）— [Clima 2022 proceedings（TU Delft）](https://proceedings.open.tudelft.nl/clima2022/article/download/335/314/323)；原始回顧為 [Sekhar et al. 2020, Building and Environment 184](https://doi.org/10.1016/j.buildenv.2020.107229)
- DTU：臥室約需 **每人 10 L/s** 才能避免睡眠受擾，約對應高於室外 400 ppm、約 1 ACH — [DTU: How much ventilation is necessary to avoid disturbance to sleep](https://orbit.dtu.dk/en/publications/how-much-ventilation-is-necessary-to-avoid-disturbance-to-sleep/)
- **Strøm-Tejsen 等 2016**（Indoor Air 26(5):679–686，單人學生宿舍）：前導實驗（N=14）關窗平均 **2585 ppm**、開窗 660 ppm；第二實驗（N=16）在 CO2 >900 ppm 時開風扇，兩條件平均 **2395 vs 835 ppm**。CO2 較低時，腕動計測得的睡眠品質與空氣新鮮感顯著改善，隔天嗜睡、專注力與邏輯思考測驗表現也較好 — [DTU Orbit](https://orbit.dtu.dk/en/publications/the-effect-of-cosub2sub-controlled-bedroom-ventilation-on-sleep-a/)；[core.ac.uk 全文](https://core.ac.uk/download/83998549.pdf)；[Roomvent 2014 版本](https://backend.orbit.dtu.dk/ws/portalfiles/portal/101895512/Roomvent_2014_Paper_ID_148.pdf)
- Mishra 等 2017（Indoor Air，17 位年輕成人）：開門/窗平均 717 ppm，關閉 1150 ppm，開啟時睡眠品質較好 — [Sci.News](https://www.sci.news/medicine/opening-windows-doors-sleep-quality-05459.html)；[Science Trends](https://sciencetrends.com/using-open-door-windows-to-ventilate-bedrooms-and-the-consequent-effect-on-sleep-quality)
- Liao 等 2022（Building and Environment 224，丹麥 84 戶住宅、每戶量測一週）：開臥室門或窗（作為加強通風的代理指標）改善主觀睡眠品質與 IAQ — [DOI 10.1016/j.buildenv.2022.109557](https://doi.org/10.1016/j.buildenv.2022.109557)

### Inferences
- 《室內空氣品質管理法》與其標準只管環境部公告的「公告場所」，私人住宅不是法定管制對象（此點為背景知識，本次未取得條文原文佐證）。實務上，1000 ppm/8h 可當作住宅「及格線」。睡眠研究支持臥室夜間目標設在 **≤800 ppm**，1000 ppm 是上限。
- 第 102 條 8 m³/h·m² 用在本案：臥室 22×8 = **176 m³/h**，客廳 30×8 = **240 m³/h**，合計 **416 m³/h**，超過 LGH-35RVX3-E 的 350 m³/h 上限。不過條文沒限定通風量必須是外氣（內政部會議也指出「新鮮外氣量」未定義），且只在「設置機械通風設備時」才適用。一般住宅靠開窗自然通風合規，這條不算對 ERV 外氣量的強制要求。
- 住宅性能評估 C 級 4 m³/h·m² 外氣：臥室 88 m³/h、客廳 120 m³/h，合計 **208 m³/h**，ERV 用 speed 3（263 m³/h）即可涵蓋。
- ASHRAE 62.2 若只把 2F（52 m²、1 臥室）當成獨立居住單元：0.15×52 + 3.5×(1+1) = **14.8 L/s ≈ 53 m³/h**。下面第 2 節的計算顯示，即使這 53 m³/h 全部送進臥室，兩人睡眠時的穩態約 920 ppm；若平均分配，臥室會超過 1000 ppm。可見 62.2 的全宅最低量不足以讓關門的雙人臥室達到 800 ppm，與 Akimoto 2025「約需現行住宅標準兩倍」的結論一致。
- 各標準換成「每人外氣量」比較：EN Cat II 7 L/s = 25 m³/h·p；Akimoto 8 L/s = 28.8 m³/h·p；EN Cat I 及 DTU、WHO 10 L/s = 36 m³/h·p。

### Gaps
- EN 16798-1 針對「住宅臥室」的專用表（常被引用為 Cat I/II/III 高於室外 380/550/950 ppm，及臥室每人 L/s 值）本次**未能取得原文佐證**。只確認了非住宅的 550/800/1350 ppm。
- 台灣綠建築 EEWH（住宿類 EEWH-RS）、健康建築標章是否有具體 CO2 或住宅換氣量門檻，本次沒有找到。
- 第 102 條的現行全文與第 43 條（自然通風開口）未在全國法規資料庫原頁面核對，只靠 rootlaw、LawPlayer 的轉載。
- WHO 對住宅 CO2 沒有找到任何具體數值指引。WHO 路線圖原文未讀到。
- ASHRAE 62.2-2019/2022 最新版係數沒有直接從標準原文核對（Addendum r 的抽取文字缺係數），0.15/3.5 來自 Retrotec 的轉述。

---

## 2. 每人/每面積外氣量與質量平衡計算：CO2 產生率（睡眠 vs 坐姿）、2 人 22 m² 臥室與 4 人 30 m² 客廳所需風量

### Takeaway
採保守的睡眠 CO2 產生率 13.3 L/h·人（Persily 85 kg 男性例），室外 420 ppm 時：**2 人關門臥室要維持 ≤1000 ppm 需約 46 m³/h 外氣，≤800 ppm 需約 70 m³/h**（室外 450 ppm 時分別約 48、76 m³/h）。4 人坐姿客廳（18 L/h·人）≤1000 ppm 需約 **124–131 m³/h**，≤800 ppm 需約 **190–206 m³/h**。

### Cited Findings
- Persily & de Jonge 2017（Indoor Air 27(5):868–879，DOI 10.1111/ina.12383）以基礎代謝率（BMR）、活動量（MET）、身體尺寸、性別、年齡推估 CO2 產生率，取代 1980 年代沿用至今的舊公式 — [Wiley 全文頁](https://onlinelibrary.wiley.com/doi/full/10.1111/ina.12383)；[NIST 頁面](https://www.nist.gov/publications/carbon-dioxide-generation-rates-building-occupants-0)；[NIST PDF](https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=920870)
- 簡化式（二手來源）：**g [L/s] = 0.000569 × RQ × BMR [MJ/day] × M**，RQ 約 0.85 — [AIVC 論文（Oke）](https://aivc.org/sites/default/files/123-178-Oke-Oluwatobi.pdf)（搜尋摘要轉述）
- 論文範例：**85 kg、30–60 歲男性，BMR 7.73 MJ/day → 約 0.0037 L/s CO2**（M = 1.0）。表中睡眠的 MET 為 0.95（另一表格寫 1.0，兩處不一致）— [Wiley 全文頁](https://onlinelibrary.wiley.com/doi/full/10.1111/ina.12383)
- 舊式「成人單一值」約 **0.3 L/min（= 18 L/h）**，不分個人特徵 — [News-Medical 報導 NIST 研究](https://www.news-medical.net/news/20170428/Researchers-develop-new-computation-methodc2a0for-better-estimation-of-indoor-carbon-dioxide.aspx)
- 中國研究：舊方法高估實測 CO2 產生量，女性約 25%、男性約 16% — [News-Medical](https://www.news-medical.net/news/20170428/Researchers-develop-new-computation-methodc2a0for-better-estimation-of-indoor-carbon-dioxide.aspx)
- 驗證研究：Persily-de Jonge 預測值比 ASHRAE 方法更接近實測 VCO2，平均絕對差 6–21% — [Maastricht University CRIS](https://cris.maastrichtuniversity.nl/en/publications/assessing-the-accuracy-of-predicted-values-of-human-co2-generatio/)
- 女性在相同活動量下 CO2 產生量較低，主因是體重較輕 — [ScienceDirect: CO2 generation rates of different age and gender](https://www.sciencedirect.com/science/article/abs/pii/S0360132320306880)
- DTU：每人 10 L/s 約對應臥室高於室外 400 ppm — [DTU Orbit](https://orbit.dtu.dk/en/publications/how-much-ventilation-is-necessary-to-avoid-disturbance-to-sleep/)

### Inferences（計算，含假設）

**(a) 公式**
- 單一完全混合區的質量平衡：V·dC/dt = Q·(C_out − C) + G×10⁶
  - V：房間體積 m³；Q：有效外氣量 m³/h；G：CO2 產生率 m³/h；C：ppm
- 穩態：**C_ss = C_out + G×10⁶ / Q**，所以 **Q = G×10⁶ / (C_target − C_out)**
- 暫態：C(t) = C_ss + (C₀ − C_ss)·e^(−t/τ)，時間常數 τ = V/Q

**(b) CO2 產生率假設**
- 驗算：0.000569×0.85×7.73×1.0 = 0.00374 L/s，與論文的 0.0037 L/s 一致，代表上面的常數可用。
- 設計用睡眠值取 **13.3 L/h·人（0.0037 L/s）**，屬保守值（85 kg 男性、M = 1.0）。
- 台灣常見體型（筆者假設，BMR 依 Schofield 式估算）：70 kg 男性 BMR ≈ 7.0 MJ/d → 睡眠 M 0.95 約 11.6 L/h，M 1.0 約 12.2 L/h；58 kg 女性 BMR ≈ 5.5 MJ/d → 睡眠約 9.1–9.6 L/h。夫妻合計約 **21–22 L/h**；保守設計取 **26.6 L/h（2×13.3）**。
- 坐姿看電視、聊天（M 約 1.3–1.5）：70 kg 男性約 16–18 L/h，58 kg 女性約 12.5–14.4 L/h。設計取 0.3 L/min 單一值 **18 L/h·人**；4 人 = **72 L/h**。若有兩位兒童，約 60 L/h。

**(c) 臥室：2 人睡眠、22 m²，假設淨高 2.7 m → V ≈ 59 m³**

| G（2 人） | C_out | 目標 ≤1000 ppm | 目標 ≤800 ppm |
|---|---|---|---|
| 26.6 L/h（保守） | 420 | **45.9 m³/h**（0.78 ACH） | **70.0 m³/h**（1.18 ACH） |
| 26.6 L/h | 450 | 48.4 | 76.0 |
| 22 L/h（台灣典型體型） | 420 | 37.9 | 57.9 |
| 22 L/h | 450 | 40.0 | 62.9 |

- 換算每人：≤1000 ppm 約需 **19–24 m³/h·人（5.3–6.7 L/s）**；≤800 ppm 約需 **29–38 m³/h·人（8–10.6 L/s）**，與 Akimoto 的 8 L/s、DTU 的 10 L/s 相符。
- 臥室外氣量與穩態 CO2 的對照（C_out 420；保守 / 典型）：

| 外氣量 m³/h | 穩態 CO2 ppm（26.6 / 22 L/h） |
|---|---|
| 9 | 3376 / 2864 |
| 15 | 2193 / 1887 |
| 20 | 1750 / 1520 |
| 30 | 1307 / 1153 |
| 44 | 1025 / 920 |
| 53 | 922 / 835 |
| 60 | 863 / 787 |
| 70 | 800 / 734 |
| 88 | 722 / 670 |

- 暫態（起始 600 ppm，8 小時夜間，G = 26.6 L/h）：

| 外氣量 | τ | 8 小時後 | 8 小時平均 |
|---|---|---|---|
| 45 m³/h | 1.3 h | 1010 ppm | 943 ppm |
| 70 m³/h | 0.85 h | 800 ppm | 779 ppm |

  約 3τ（3–4 h）內就接近穩態，所以夜間 8 小時平均基本上由穩態值決定。

**(d) 客廳：4 人坐姿、30 m²，V ≈ 81 m³**

| G | C_out | ≤1000 ppm | ≤800 ppm |
|---|---|---|---|
| 72 L/h（4 成人） | 420 | **124 m³/h** | **190 m³/h** |
| 72 L/h | 450 | 131 | 206 |
| 60 L/h（2 大 2 小） | 420 | 103 | 158 |
| 80 L/h（較活躍） | 450 | 146 | 229 |

- 對照：客廳 4 人時，100 m³/h → 1140 ppm；150 → 900；175 → 831；200 → 780；263 → 694 ppm。
- 換算每人：≤1000 ppm 約 31–33 m³/h·人；≤800 ppm 約 47–51 m³/h·人。坐姿人員的 CO2 產生率約是睡眠的 1.4–1.6 倍，所需外氣量也同比例增加。

**(e) 室外背景值**
- 全球背景約 420 ppm。台灣都市夜間逆溫或靠近道路時，室外常見 450–500 ppm（筆者推估，未取得台灣實測文獻）。每升高 30 ppm，800 ppm 目標所需風量約增加 9%。建議以實測室外值設計。

**(f) 與 ERV 能力的比較**
- 兩人臥室 ≤800 ppm（70–76 m³/h）加客廳 4 人 ≤1000 ppm（124–131 m³/h），兩者都在 LGH-35RVX3-E 的能力內。
- 若「客廳 4 人 ≤800」與「臥室 2 人 ≤800」同時發生，約需 190+70 = **260–280 m³/h**，約為 speed 3–4。這種情況實際上很少同時出現。

### Gaps
- Persily 2017 表格中 0.95 MET、30–60 歲女性的確切 L/s 值沒有取得（PMC、Wiley 全文無法抓取）。上面的台灣體型數值是筆者以 Schofield 式自行估算，非原文表值。
- 「Emission rate of carbon dioxide while sleeping」（ResearchGate 2021，以及老年人版 2023 Building and Environment）有實測睡眠 CO2 排放率，但本次沒取得數值 — [ResearchGate](https://www.researchgate.net/publication/353640001_Emission_rate_of_carbon_dioxide_while_sleeping)；[ScienceDirect 老年人版](https://www.sciencedirect.com/science/article/abs/pii/S0360132323003268)
- 日本/台灣教科書常用的「睡眠 0.011、安靜 0.0132、極輕作業 0.022 m³/h·人」，本次**找不到出處**，不宜直接引用。
- 台灣住宅實際淨高（有無天花板風管降板）會影響 τ，但不影響穩態值。

---

## 3. 房間間風量分配、ERV 風速排程、CO2 感測連動（LGH-35RVX3-E/台灣常見控制器）與感測器位置

### Takeaway
LGH-35RVX3-E 有 4 段風速：**88 / 175 / 263 / 350 m³/h**（15 / 29 / 61 / 120 W），可在 25–100% 以 5% 調整。原廠 CO2 感測器（PZ-70CSW-E 壁掛 / PZ-70CSD-E 風管型）可直接插到機板，在 Auto Fan Mode 下自動調風，並可用 PZ-62DR-E 設定上下限 300–2000 ppm。但它是**整機一顆感測器**：無法同時依臥室與客廳各自的 CO2 分區控制。分區要靠風管配比（固定）或電動風門（另購第三方）。

### Cited Findings
- LGH-35RVX3-E 風速（NZ 規格表）：speed 4 **350 m³/h（97 L/s）/120 W**，speed 3 **263 m³/h（73 L/s）/61 W**，speed 2 **175 m³/h（49 L/s）/29 W**，speed 1 **88 m³/h（24 L/s）/15 W** — [SPC_LGH-35RVX3-E](https://mitsubishi-electric.co.nz/materials/PRODUCT/Ventilation/LGH-RVX3-E/01_Specifications/SPC_LGH-35RVX3-E.pdf)
- 預設最低速 speed 1 = 25%。送風、排風的預設風速可各自在 **25–100% 間以 5% 調整**。RVX3-E 系列另有「Signal output terminal PZ-4GS-E」，屬輸出配件，不是 CO2 輸入 — [Mitsubishi Australia Flyer Lossnay RVX3-E 2024-11](https://mitsubishielectric.com.au/wp-content/uploads/2024/12/Flyer_Lossnay-RVX3-E-2024-11.pdf)
- CO2 感測器 PZ-70CSW-E（壁掛）與 PZ-70CSD-E（風管型）直接接到 Lossnay 機組，即插即用、不需外接電源（由 Lossnay 控制板供電）。須設定 **Auto Fan Mode** 才會依 CO2 調風。可用 PZ-62DR-E 遙控器把 CO2 上下限設在 **300–2000 ppm，50 ppm 一級** — [Mitsubishi NZ: Lossnay PZ-70CS(W)(D)-E CO2 Sensors](https://www.mitsubishi-electric.co.nz/materials/ventilation/brochures/Lossnay-PZ-70CS(W)(D)-E-CO2-Sensors.pdf)；[NZ 壁掛 CO2 感測器頁](https://www.mitsubishi-electric.co.nz/heatpump/i/685141/wall-mounted-co2-sensor)
- PZ-70CSW-E2 / PZ-70CSD-E2 相容 **LGH-RVX3、LGH-RVS、LGH-RVXT3** 系列。風量以 16 段（25–100%）調整，壁掛型附紅綠燈 LED。偵測到中/高 CO2 時 Auto Fan Mode 提高風速，CO2 恢復正常後回到原風速 — [Cooling Post: Mitsubishi adds CO2 sensors to Lossnay units](https://coolingpost.com/products/mitsubishi-adds-co2-sensors-to-lossnay-units)
- 選配 Wi-Fi Control Interface 可即時查看 CO2 濃度 — [Mitsubishi NZ Lossnay Wi-Fi Control](https://mitsubishi-electric.co.nz/publications/ventilation/Lossnay-Fresh-Air-Heat-Recovery-Ventilation-Wi-Fi-Control/13/)
- 接線圖：感測器經 CO2 sensor cable 與 LED cable（隨附）接到機組控制板，沒有另設外部輸入端子的說明 — [Mitsubishi NZ CO2 sensor brochure](https://www.mitsubishi-electric.co.nz/materials/ventilation/brochures/Lossnay-PZ-70CS(W)(D)-E-CO2-Sensors.pdf)
- Strøm-Tejsen 2016 第二實驗用簡單的「CO2 >900 ppm 開風扇」控制，讓臥室平均 CO2 降到 835 ppm — [DTU Orbit](https://orbit.dtu.dk/en/publications/the-effect-of-cosub2sub-controlled-bedroom-ventilation-on-sleep-a/)

### Inferences
**風量分配與排程（以第 2 節保守值、C_out 420 計）**
- **夜間（22:30–07:00，2 人在主臥、門關）**：臥室需 ≥70 m³/h 才能 ≤800 ppm。
  - speed 1（88 m³/h）時，臥室分配比例與穩態 CO2：

    | 臥室分配 | 臥室外氣量 | 穩態 CO2（保守 / 典型） |
    |---|---|---|
    | 30% | 26 m³/h | 1428 / 1253 ppm |
    | 50% | 44 m³/h | 1025 / 920 ppm |
    | 70% | 62 m³/h | 852 / 777 ppm |
    | 80% | 70 m³/h | 798 / 732 ppm |

  - 結論：**夜間臥室需取得總送風的 ≥75–80%（speed 1），或在 50/50 固定配比下改跑 speed 2（臥室約 87 m³/h → ~725 ppm）**。speed 2 只有 29 W，耗電差異很小，但要確認臥室出風口的噪音。
- **晚間客廳（4 人）**：≤1000 ppm 需約 125–131 m³/h 到客廳。
  - 固定 55/45（客廳/臥室）配比時：speed 2 給客廳約 96 m³/h → ~1170 ppm，不足；**speed 3** 約 145 m³/h → ~915 ppm；speed 4 約 193 m³/h → ~795 ppm。
- **固定配比的建議**：臥室約 45%、客廳約 55%，排程如下：

  | 時段 | 風速 | 主要結果 |
  |---|---|---|
  | 夜間 | speed 2 | 臥室 ~79 m³/h → ~760 ppm |
  | 晚間 4 人 | speed 3 | 客廳 ~915 ppm |
  | 白天無人 | speed 1 | 2F 約 88 m³/h ≈ 0.6 ACH 背景換氣 |

  若要壓低夜間噪音、讓 speed 1 也達標，就需要電動風門（Lossnay 本身沒有分區風門控制；第三方產品待查）。
- **CO2 連動策略**：機組只接一顆原廠感測器。
  - **壁掛型放主臥**：夜間依臥室 CO2 調速最直接，Strøm-Tejsen 式的閾值控制已證實有效。建議下限約 700、上限約 900–1000 ppm（筆者建議值）。缺點是晚上客廳 4 人時不會反應，需配合排程或手動切速。
  - **風管型裝在回風/排風管**：讀到的是各室排氣的混合值。若臥室回風只占一部分，關門臥室偏高時會被稀釋，**低估臥室 CO2**。不建議當作臥室保護手段。
- **獨立 CO2 計作為驗證**：建議另放一台獨立的 NDIR CO2 記錄器（可記錄、有自動校正）在臥室，第一週量測夜間曲線，以驗證實際外氣量。反推方式：穩態 Q ≈ G×10⁶/(C_ss − C_out)，或用睡前開門讓 CO2 下降的衰減斜率求 τ。
- **感測器擺放（一般實務原則，本次未取得專門文獻）**：呼吸區高度（臥室約床面高度至 1.2 m，客廳 1.0–1.5 m），距床頭/人 ≥1–2 m（避免直接吐氣），避開送風口氣流、窗戶、門縫與廚房。

### Gaps
- **LGH-35RVX3-E（-E 歐規/紐澳版）在台灣是否有正式代理、台灣三菱的對應型號是否相同**，本次查不到。PZ-62DR-E 與 PZ-70CS 系列在台是否可購也沒有資料。
- 機組是否有「外部接點/0–10 V 輸入」可接第三方 CO2 控制器（例如台灣常見的 CO2 連動控制器），**本次沒找到原文佐證**（只找到輸出端子 PZ-4GS-E）。需查 LGH-RVX3-E 安裝手冊（控制板端子表）。
- 4 段風量是在什麼外部靜壓下測得、是否有定風量控制，沒取得原文。實際風管阻力下 speed 1 的風量可能低於 88 m³/h，必須用風罩或風速計現場量測。
- PZ-62DR-E 是否有週排程（weekly timer）、夜間模式，本次未取得佐證。
- 各風速在臥室出風口的噪音值（dB(A)）未取得。這會直接影響夜間能否跑 speed 2。
- 台灣市面其他全熱交換器控制器（Panasonic、國產品牌）的 CO2 連動功能，本次沒查到可靠資料。

---

## 4. ERV 短路、分配不良對實際房間 CO2 的影響；為何關門臥室在沒有專用送風時常達 1500–2500 ppm

### Takeaway
關門臥室若只靠滲漏（約 0.1–0.25 ACH，≈6–15 m³/h），2 人睡 8 小時會從 600 ppm 升到 **約 2000–3000 ppm，夜間平均約 1500–1900 ppm**。這與 Strøm-Tejsen（單人宿舍平均 2395–2585 ppm）及 ASHRAE Journal（多人關門臥室平均 1327 ppm）的實測一致。ERV 總風量再大，只要外氣沒有真正送進關門的臥室，或在室外端有排氣回吸、在室內端送風口直接被排風口吸走，臥室 CO2 就會偏離設計值。

### Cited Findings
- 關門臥室實測：Strøm-Tejsen 2016 關窗 **2585 ppm**（前導）與 **2395 ppm**（第二實驗）平均值；開窗或開風扇時 660/835 ppm — [DTU Orbit](https://orbit.dtu.dk/en/publications/the-effect-of-cosub2sub-controlled-bedroom-ventilation-on-sleep-a/)；[core.ac.uk](https://core.ac.uk/download/83998549.pdf)
- ASHRAE Journal 2021 年 4 月專欄：關門臥室平均 CO2，**多人共用 1327 ppm、單人 1004 ppm**；開門或開窗時兩者都接近 500 ppm — [ASHRAE Journal April 2021](https://nxtbook.com/nxtbooks/ashrae/ashraejournal_JPPKRR/index.php?startid=58)
- Mishra 2017：關門窗 1150 ppm vs 開 717 ppm — [Sci.News](https://www.sci.news/medicine/opening-windows-doors-sleep-quality-05459.html)
- ASHRAE Journal 另有比較臥室自然通風與機械通風 CO2 曲線的專文（內容未取得）— [ASHRAE: Natural vs Mechanical Ventilation: Comparing CO2 Profiles in Bedrooms](https://www.ashrae.org/news/ashraejournal/natural-vs-mechanical-ventilation-comparing-co2-profiles-ventilation-in-bedrooms)
- 個人自我實驗（n=1，可靠度低）：關門夜間峰值約 2800 ppm — [gwern.net CO2](https://gwern.net/zeo/co2)

### Inferences（計算）
**(a) 關門、沒有專用送風的臥室（V 59 m³，2 人，G 26.6 L/h，起始 600 ppm，C_out 420）**

| 滲漏/轉移風量 | 8 小時後 | 8 小時平均 |
|---|---|---|
| 0 ACH（完全密閉） | 4182 ppm | 2391 ppm（升速 ≈ G/V = 450 ppm/h） |
| 0.10 ACH（6 m³/h） | 2958 ppm | 1936 ppm |
| 0.15 ACH（9 m³/h） | 2550 ppm | 1767 ppm |
| 0.25 ACH（15 m³/h） | 1982 ppm | 1509 ppm |
| 0.5 ACH（30 m³/h） | 1294 ppm | 1135 ppm |

- 因此「1500–2500 ppm」正是**台灣常見鋼筋混凝土加氣密鋁窗、開分離式冷氣（只循環、不引外氣）的關門臥室**落在 0.1–0.25 ACH 時的預期值。分離式冷氣、除濕機都不提供外氣，對 CO2 沒有幫助。

**(b) 分配不良的典型情況**
1. **送風、排風口都在客廳或走道，臥室只有門縫**：臥室外氣來源只剩門縫轉移與滲漏，回到上表 0.1–0.25 ACH 的情況。客廳 CO2 很低，臥室卻 2000+ ppm。
2. **臥室只有送風、沒有回風，而且門縫或轉移格柵太小**：臥室正壓。送風會因背壓下降（機組風量隨外部靜壓降低），多出來的空氣從外牆縫隙洩出。實際送進的外氣可能少於設計值，需要現場量測。建議臥室設回風口（平衡式），或設足夠的轉移通路（門底留縫/轉移格柵）。具體開口面積本次未取得來源。
3. **室內短路**：臥室內送風口與回風口距離太近（例如同一面天花板相距 <1 m），部分新鮮外氣沒有和房間空氣混合就被排走，有效換氣效率 ε <1。
   - 有效外氣量 = Q × ε。例：設計 70 m³/h、ε = 0.7 時，有效 49 m³/h → 穩態約 960 ppm，不是 800 ppm。
4. **室外端短路（排氣回吸）**：室外進氣口與排氣口太近（設備在樓梯下、兩支風管從同一面牆出去時常見），一部分排氣（含室內 CO2）被吸回送風。設回吸比例 r，穩態 C = C_out + G×10⁶/[Q(1−r)]。臥室 70 m³/h 時：

   | r | 0 | 5% | 10% | 20% |
   |---|---|---|---|---|
   | 穩態 CO2 | 800 ppm | 820 ppm | 842 ppm | 895 ppm |

   影響比室內分配不良小，但會疊加。
5. **CO2 感測器裝在回風總管**：混合值低估關門臥室（見第 3 節），控制系統「以為」已達標而維持低速。

**(c) 設計重點**
- 主臥要有**專用送風口**，夜間有效外氣量 ≥70 m³/h（≈1.2 ACH）。
- 主臥最好也有回風口；若無，要有足量的轉移通路。
- 送、回風口拉開距離或對角配置。
- 室外進/排氣口分開。
- 完工後用獨立 CO2 記錄器量測夜間曲線驗證。

### Gaps
- 台灣住宅（RC、鋁窗）臥室的實測滲漏換氣率（ACH）沒有找到在地文獻。上面 0.1–0.25 ACH 是筆者假設。
- Lossnay 熱交換芯的排氣轉移率（EATR，排氣漏到送風的比例）本次未取得原廠數值。
- 室外進/排氣口最小間距（各國規範或原廠建議）、門底留縫/轉移格柵的開口面積規範，本次沒有取得來源。
- 換氣效率 ε 的實測值（不同送/回風口配置）沒有取得文獻。上面 0.7 只是示意值。
