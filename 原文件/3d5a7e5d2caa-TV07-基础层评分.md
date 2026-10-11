# TV07 基础层评分（V3.3R2 试评｜单模型初评）

- 报告：檀棋2.0-ArctiSwarm（DeepSeek-V4-flash 基模）《俄乌战争无人与反无人体系研究：2026年6月18日莫斯科袭击核验报告》
- 评测性质：有题面
- 报告版本：sha256 8a7d12e621a3…
- 主标准／公式版本：V3.3R2 模型评估修订稿 2026-09-10；r2_calc-1.0
- 任务卡／台账／证据包：Q07-任务卡；TV07-台账.json（build_ledger v1＋规则/人工复核：fix_refs_tv：来源表 22 条，句级编号映射 0 单元；人工复核改判 16 条；清单按来源名/日期指认挂载 29 单元）；台账/TV07/evidence（fetch_evidence 2026-10-08：22 源 14 可读；Reuters ×10 401（ref-16/21 wayback 可读）、ISW ×2 403、Bloomberg/Breaking Defense 经 jina）＋同题证据包复用：B7F/ref-0010、DS07/ref-5、Q05/ref-3・ref-35、Q07/ref-3、TK05/ref-8・ref-30、K05/ref-0125、B7E/ref-0029・0199、TV05/ref-21・ref-25；补查 2026-10-09：Reuters 2023-12-19 经 Wayback 可读；2023-05-03、2025-07-28 无快照
- 资料截止时点：报告未标注；最新事实为 2026-07（北约安卡拉峰会）
- 运行条件：同 00-执行口径与状态.md；单模型初评（Claude）；檀棋2.0-ArctiSwarm DeepSeek-V4-flash 基模系列
- 过程状态：初评完成
- 综合结果状态：仅基础层；S1–S4、H、Q、档位留空待人工

## 一、基础层结果

**基础质量分 B（初评）：68.6–73.4（含U范围）**　状态：有效U

| 维度 | 得分或范围 | 分子／分母 | 基础权重 | 有效权重 | 口径与状态 |
|---|---:|---|---:|---:|---|
| O1 判定点达成 | 80.0 | P=8.00／W=10.00（已判9，U0，NA0） | 30 | 30.0 | 按任务卡 R 项逐项 0/0.5/1，理由附原文位置；D 项权重 2｜有效 |
| E1 事实与证据支持审计 | 69.7–82.5 | P=29.30／W=42.00（已判35，U5，NA0） | 20 | 20.0 | 初筛：核心10条（w=1）＋其余30条（w=32/30=1.0667）；台账事实候选 42 条｜有效U |
| O7 来源合规可追溯 | 36.3–51.0 | P=15.27／W=42.00（已判34，U6，NA0） | 15 | 15.0 | 无句级 URL 口径（Q07 来源约束：英语主流媒体/英文军事网站）：句内具名＋文末清单可读对应 0.5（上限）；清单不可读（Reuters 401/ISW 4｜有效U |
| O2 独立信源多样性 | 83.3 | G07-1 核心事件事实:3/3；G07-2 演进与反制:2/2；G07-3 供应链与产能:1/2 | 10 | 10.0 | 任务卡需求组等权；edges 仅计已核出有效来源｜有效 |
| O5 冲突证据裁决 | 81.3 | P=6.50／W=8.00（已判8，U0，NA0） | 10 | 10.0 | 按任务卡 C 项四步各 0/0.5/1｜有效 |
| O8 关键进程覆盖 | 50.0 | P=3.00／W=6.00（已判6，U0，NA0） | 10 | 10.0 | 按任务卡 U 项 0/0.5/1｜有效 |
| O9 交付合规 | 75.0 | P=4.50／W=6.00（已判6，U0，NA1） | 5 | 5.0 | R 型清单 0/0.5/1；交付期限 NA｜有效 |

说明：有 U 时给范围（下界向下、上界向上取 1 位），不是统计置信区间；B 不套用综合档位。

## 二、可用性检查与重大缺陷候选（模型候选，待真人确认）

- V1 核心证据与推理最低基础：**检查未见候选**。核心 10 条：7A+3P（P009-S01/P012-S02 Reuters 2023-05-03、2025-07-28 无 Wayback 快照）；样本无 N 问题ID：
- V2 时效关键窗口：**NA**。
- 重大缺陷候选：检查未见候选（不等于已确认通过）

## 三、核心依赖记录

| 核心判断 | 依赖事实ID | 支持状态 | 推理连接 | 是否需复核 |
|---|---|---|---|---|
| 6/18 为全面战争以来最大规模、一周内两度瘫痪莫斯科炼油厂两大装置；变化在量级与目标性质而非型号 | ['TV07-P001-S02', 'TV07-P003-T', 'TV07-P004-T', 'TV07-P006-T', 'TV07-P014-S01', 'TV07-P017-S01'] | A/A/A/A/A/A | CNN/BBC＋Reuters 镜像＋WotR＋CSIS | 否 |

## 四、问题清单（唯一编号，主要维度归属）

| 问题ID | 主要维度 | 次要影响 | 描述 | 原文位置 |
|---|---|---|---|---|
| ITV07-01 | O7 | ['E1'] | 清单 22 条中 Reuters 10 条 401（2 条经 wayback 可读）、ISW 2 条 403、AP jina 仅导航页；核心/样本 7 条 O7 记 U | §六 |
| ITV07-02 | O9 | [] | 无句级编号或 URL；清单无标题/日期，仅能按来源名/主题推断配对 | 全文 |
| ITV07-03 | O8 | ['O1'] | U07-2 蛛网行动、U07-6 6/28 普京燃料短缺与限供、Rubicon、海上无人艇均缺；R07-07 北约援助机制/数据缺 | §三/§五 |
| ITV07-04 | E1 | [] | AP/Reuters 归属的泽连斯基原话、普京空防表态、Atlantic Council 500–600 万估计、乌转向台日供应商、ISW 2025-10 Molniya 月产 5 万等 6 处未核到（后两处报告已自标） | §二/§四/§五 |
| ITV07-05 | E1 | [] | §一波及栏‘Sheremetyevo 疏散、环城高速封闭、Zhukovsky 住宅受损’在可读来源中未核到 | §一 |

## 五、逐项判定

### O1 判定点（按任务卡 R 项逐项 0/0.5/1，理由附原文位置；D 项权重 2）

| id | w | v | 理由 | 问题ID |
|---|---|---|---|---|
| R07-01 | 1 | 1 | §一证据等级表：规模（555/992/180/194）、型号（标未证实）、战术（§三诱饵/波次）、战果（CDU-6/Euro+/6 个月）、战略影响（§四防空再部署）——均有英文来源 |  |
| R07-02 | 1 | 1 | §二：以 2023-05-03 克宫为基线，四个比较维度（数量级、目标性质、多目标同步、首都运行中断）各附来源 |  |
| R07-03 | 1 | 1 | §三三阶段各有标志性事实：TB2/Shahed/Lyutyi 立项；FPV 150 万→450 万、光纤；诱饵/Auterion AI 套件/炼油厂 194 次/6-30 Dubna |  |
| R07-04 | 1 | 1 | §三/§四：炼油厂 194 次（11 倍）、拦截机 6300/1500/70%、FPV 采购量——数据带期间与出处 |  |
| R07-05 | 1 | 0.5 | §四：CSIS 四大瓶颈（碳纤维/稀土磁体/锂电池/氮化镓）集中于中国、乌转向台日——组件与来源国有；‘比例’明示不采信，缺数据 |  |
| R07-06 | 1 | 1 | §四：S-400 新阵地（6/4 影像）、Pantsir 由前线转调、普京承认突破、90% 拦截率 vs ISW 评估——成效与不足并列 |  |
| R07-07 | 1 | 0.5 | §五：北约安卡拉峰会议程、乌国防工业与盟友共建——无具体机制/预算数据（报告自陈‘未核对，不列出’） |  |
| R07-08 | 1 | 1 | §五：AI 末制导（Auterion）、俄 AI 寻的头、光纤使射频干扰失效、‘人在回路’主流——有依据 |  |
| R07-D1 | 2 | 0.5 | 区分俄国防部全国数 vs 莫斯科市长数 vs 实际命中（炼油厂两装置），并明示‘俄方所有拦截数字均为单方声称’；但未给乌方发射数，三口径对账不完整 |  |

### E1 事实与证据支持（初筛：核心10条（w=1）＋其余30条（w=32/30=1.0667）；台账事实候选 42 条）

抽样：种子 2026100807，抽样框 32 条，样本 30 条，核心全查 10 条；台账事实候选合计 60。

标签计数：A 21；P 14；U 5

| id | 核心 | 标签 | w | 理由 | 问题ID |
|---|---|---|---|---|---|
| TV07-P001-S02 | True | A | 1 | ref-7 CNN 6/18（可读）‘largest attack on Moscow since start of full-scale war’；ref-9 BBC、ref-10 Bloomberg（标题可读）、ref-6 AP（jina 导航页）同日报道 |  |
| TV07-P003-T | True | A | 1 | Q05 包 ref-3 WaPo：Defense Ministry…at least 992 drones…past 24 hours；555 见 Q05 包 ref-1/2/5；ref-7 CNN：194 (Sobyanin)；TV05 包 ref-21 ABC：About 180…shot down as they approached Moscow——‘先 180 后 194’对应 |  |
| TV07-P004-T | True | A | 1 | ref-7 CNN：Moscow Oil Refinery, just 15 kilometers from the Kremlin, in Kapotnya…struck and damaged on Tuesday（一周内第二次）、Video geolocated by CNN；Q07 包 ref-3 Kyiv Independent：Russian oil depot in Rostov Oblast hit |  |
| TV07-P006-T | True | A | 1 | B7F 包 ref-0010 MarketScreener（Reuters 6/18 全文）：CDU-6…53%、Euro+…140,000 bpd—47%、secondary units/pipelines/tanks damaged and caught fire；DS07 包 ref-5（Reuters 6/24 镜像）：at least six months |  |
| TV07-P007-T | True | P | 1 | ref-7 CNN：Flights at all major Moscow airports temporarily suspended；TK05 包 ref-8 CNBC：16 people injured、four airports grounded；ref-9 BBC：ring road 可见火光、‘black rain’；Sheremetyevo 疏散、环城高速封闭、Zhukovsky 住宅受损未核到 |  |
| TV07-P009-S01 | True | P | 1 | ref-22 Reuters 2023-05-03 401；标题 russia-says-ukraine-attacked-kremlin-with-drones-failed-bid-kill-putin 与断言一致，正文未打开 |  |
| TV07-P011-S01 | True | A | 1 | ref-16 Reuters 2025-03-10（wayback 可读）：purchased more than 1.5 million such drones [in 2024]—96% from Ukrainian manufacturers；plans to purchase around 4.5 million FPV drones in 2025；more than $2.6 billion |  |
| TV07-P012-S02 | True | P | 1 | ref-14 Reuters 2025-07-28 401；URL 标题 auterion-says-it-will-provide-ukraine-with-33000-ai-drone-guidance-kits 对应 3.3 万套；‘5000 万美元合同’‘约 1 公里自主追踪’未核到（Q08/B7E 包仅载 Auterion 公司信息） |  |
| TV07-P014-S01 | True | A | 1 | ref-17 War on the Rocks（可读）：Syrskyi 3/3 称 2 月拦截机 roughly 6,300 missions、destroyed more than 1,500 Russian drones、more than 70 percent of Shahed-type drones in the Kyiv area downed by interceptor drones |  |
| TV07-P017-S01 | True | A | 1 | ref-20 CSIS（可读）：drones on both sides contain materials and components that originate in Chinese factories；Carbon fiber, rare-earth magnets, lithium-ion cells, and gallium-nitride chips are critical nodes in the Chinese supply chain |  |
| TV07-P009-S08 | False | P | 1.0667 | ref-7 CNN：Zelensky called Thursday's attacks a ‘justified’ response to Russia targeting…UNESCO-listed monastery complex——报复定性对应；‘若乌克兰燃烧，莫斯科也将燃烧’‘是时候结束战争’原话未在可读来源核到（AP jina 为导航页、Reuters 401） |  |
| TV07-P014-S03 | False | A | 1.0667 | ref-19 Defense News 2026-03-20（可读）：Ukraine has deployed specialist teams to five Middle Eastern countries to help intercept drones and advise on air-defense measures |  |
| TV07-P012-S03 | False | A | 1.0667 | K05 包 ref-0125 Ukrinform（转 FT）：Russian refineries hit at least 194 times since the start of 2026—11 times more than the same period last year；U.S. intelligence support…helping Kyiv select optimal flight routes——报告已标‘二手转引’ |  |
| TV07-P015-S02 | False | P | 1.0667 | ref-17 WotR 可读；FPV 依赖人工操作/无导航辅助的具体句未定位（文中 CRPA/GPS 讨论为俄方） |  |
| TV07-P014-S02 | False | A | 1.0667 | ref-18 Breaking Defense（jina 可读）：引 RUSI 报告——propellor and turboprop-powered gunship interceptors [transport aircraft modified with onboard machine guns]…much more affordable, sustainable way |  |
| TV07-P009-S07 | False | A | 1.0667 | ref-7 CNN：airports suspended；ref-9 BBC：Moscow residents complain of black rain、fire visible from the Moscow ring road |  |
| TV07-P018-S02 | False | U | 1.0667 | 报告自标‘非名单内信源，仅作背景’；ISW 2025-10 Molniya 光纤与月产 5 万未核（B7E 包 drone-warfare 仅载 Molniya 类型） |  |
| TV07-P011-S02 | False | P | 1.0667 | ISW 清单条目（ref-11/12）403；俄 GPS/链路压制为 ISW 系列通论，ref-17 WotR 载俄方 CRPA/Kometa 抗干扰——方向一致，原句未核 |  |
| TV07-P013-S01 | False | A | 1.0667 | TK05 包 ref-30 ISW 6/22：satellite imagery collected on June 4 suggests Russia started constructing a new S-400 installation…west of Moscow City；The Telegraph reported on June 22 that Russia redeployed a Pantsir…from the frontline…near the Moscow Oil Refinery |  |
| TV07-P016-S03 | False | P | 1.0667 | 无 URL（报告自标‘经其他信源转引’）；T05-01/B7E 包载泽连斯基 1000 万/2000 万目标表述，Reuters NEXT 原访谈未核 |  |
| TV07-P013-S03 | False | U | 1.0667 | 无 URL；普京‘有些突破了进来，需要加强空防’（AP/Politico）未核 |  |
| TV07-P016-S02 | False | A | 1.0667 | ref-16 Reuters 2025-03-10（wayback）：plans to purchase around 4.5 million FPV drones in 2025, defence ministry said |  |
| TV07-P008-S01 | False | P | 1.0667 | ref-11 ISW 6/18 403；TV05 包 ref-25 ISW 6/19 可读含对俄防空的评估；‘军事博主约 90%’与‘重兵防御的首都’原句未核 |  |
| TV07-P005-T | False | P | 1.0667 | 无 URL；B7E 包 drone-warfare.com 载 An-196/FP-1 研究页，‘主流英文信源未确认型号’的否定性陈述与证据包状态一致，具体 OSINT 识别未定位 |  |
| TV07-P012-S04 | False | A | 1.0667 | ref-8 CNN 6/30（可读）：Dubna Satellite Communications Centre…hit；last week Zelensky announced a 40-day operation aimed at ‘compelling’ Russia to end the war |  |
| TV07-P009-S06 | False | P | 1.0667 | 无 URL；‘十余州多目标同步（乌方口径）’未核；TV05 包 ISW 6/19 载乌方对多地打击 |  |
| TV07-P013-S02 | False | U | 1.0667 | 无 URL；泽连斯基称俄调集大量防空保护少数要地（AP/PBS）未核 |  |
| TV07-P011-S03 | False | P | 1.0667 | 无 URL（ISW/Atlantic Council 具名）；光纤无人机 2024–25 规模化、俄先导为多包通论（B7E ref-0188 载俄 fiber-optic FPV 日配额）；‘射程超 30 公里’‘乌批准 80 余型’未核 |  |
| TV07-P018-S03 | False | P | 1.0667 | ref-19 Defense News 3/20 为中东部署稿，不含安卡拉峰会；B7E 包 ref-0199 载 NATO's Ankara summit 与 Drone Edge Initiative；‘7 月 7–8 日’‘以乌克兰与反无人机为核心议程’未精确核到 |  |
| TV07-P010-S01 | False | P | 1.0667 | 无 URL；2022 年 TB2 与商用机侦察校射为通论，未指认来源 |  |
| TV07-P018-S01 | False | P | 1.0667 | ref-14 Reuters 401（Auterion）；ref-18 Breaking Defense 可读但‘人在回路仍是主流’原句未定位；俄方 AI 寻的头（ISW）403 |  |
| TV07-P016-S04 | False | U | 1.0667 | 无 URL；Atlantic Council 2026 实际 500–600 万架估计未核 |  |
| TV07-P010-S02 | False | A | 1.0667 | Q05 包 ref-35 The Diplomat：俄自 2022 年 10 月起建 Alabuga Shahed 生产线（Reuters 链接）；Shahed 2022 年秋大规模袭乌为多包通论 |  |
| TV07-P010-S03 | False | A | 1.0667 | B7E 包 ref-0029 drone-warfare：Ukroboronprom announced [Lyutyi] publicly on 17 October 2022 |  |
| TV07-P001-S03 | False | A | 1.0667 | ref-7 CNN：Zelensky called Thursday's attacks a ‘justified’ response——公开确认 |  |
| TV07-P017-S02 | False | U | 1.0667 | 无 URL（报告自标‘媒体转引，未直接核对原文’）；乌转向台湾/日本替代供应商未核 |  |
| TV07-P015-S01 | False | A | 1.0667 | ref-13 CNAS Evolution Not Revolution（可读）：drones…have not replaced traditional air forces or been able to obtain air superiority |  |
| TV07-P012-S01 | False | A | 1.0667 | ref-17 WotR：Gerbera and Parodiya decoy drones fitted with a Luneburg lens to radar-imitate larger drones…to overload defenses |  |
| TV07-P015-S03 | False | A | 1.0667 | ref-21 Reuters 2025-01-24（wayback 可读）：‘unmanned systems alone cannot change the course of the war’…‘You still need infantry…artillery…aviation’ |  |
| TV07-P016-S01 | False | A | 1.0667 | ref-15 Reuters 2023-12-19 经 Wayback（TV05/evidence/补查/reuters-20231219-wayback.txt）可读：Ukraine will produce one million drones next year, Zelenskiy said |  |

### O7 来源合规可追溯（无句级 URL 口径（Q07 来源约束：英语主流媒体/英文军事网站）：句内具名＋文末清单可读对应 0.5（上限）；清单不可读（Reuters 401/ISW 403）U；句内具名无 URL 0.5；无来源 0）

| id | w | v | 理由 |
|---|---|---|---|
| TV07-P001-S02/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P003-T/引用 | 1 | U | ref-11 ISW 403、ref-1 Reuters 401 |
| TV07-P004-T/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P006-T/引用 | 1 | U | ref-3/4/5 Reuters 401 |
| TV07-P007-T/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P009-S01/引用 | 1 | U | ref-22 Reuters 401 |
| TV07-P011-S01/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P012-S02/引用 | 1 | U | ref-14 Reuters 401 |
| TV07-P014-S01/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P017-S01/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P009-S08/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P014-S03/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P012-S03/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P015-S02/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P014-S02/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P009-S07/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P018-S02/引用 | 1.0667 | 0 | 报告自标非名单内信源，无 URL |
| TV07-P011-S02/引用 | 1.0667 | 0.5 | 具名 ISW，清单 ISW 条目不可读 |
| TV07-P013-S01/引用 | 1.0667 | U | ref-12 ISW 403（经 TK05 包核实内容） |
| TV07-P016-S03/引用 | 1.0667 | 0.5 | 具名 Reuters NEXT 经转引，无 URL |
| TV07-P013-S03/引用 | 1.0667 | 0.5 | 具名 AP/Politico，无 URL |
| TV07-P016-S02/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P008-S01/引用 | 1.0667 | U | ref-11 ISW 403 |
| TV07-P005-T/引用 | 1.0667 | 0.5 | 具名 OSINT 分析，无 URL |
| TV07-P012-S04/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P009-S06/引用 | 1.0667 | 0.5 | 具名乌方口径，无 URL |
| TV07-P013-S02/引用 | 1.0667 | 0.5 | 具名 AP/PBS，无 URL |
| TV07-P011-S03/引用 | 1.0667 | 0.5 | 具名 ISW/Atlantic Council，无 URL |
| TV07-P018-S03/引用 | 1.0667 | 0.5 | 具名 Defense News，清单 ref-19 为 3 月稿不对应 |
| TV07-P010-S01/引用 | 1.0667 | 0 | 无来源名、无 URL |
| TV07-P018-S01/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P016-S04/引用 | 1.0667 | 0.5 | 具名 Atlantic Council，无 URL |
| TV07-P010-S02/引用 | 1.0667 | 0 | 无来源名、无 URL |
| TV07-P010-S03/引用 | 1.0667 | 0 | 无来源名、无 URL |
| TV07-P001-S03/引用 | 1.0667 | 0.5 | 具名泽连斯基经 CNN，可读 |
| TV07-P017-S02/引用 | 1.0667 | 0 | ‘媒体转引’无具名、无 URL |
| TV07-P015-S01/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P012-S01/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P015-S03/引用 | 1.0667 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV07-P016-S01/引用 | 1.0667 | 0.5 | ref-15 经 Wayback 可读且对应（无句级 URL 口径上限 0.5） |

### O2 独立信源分组匹配（任务卡需求组等权；edges 仅计已核出有效来源）

- **G07-1 核心事件事实**（v=1，m=3，k=3）槽位：S1 英语主流媒体、S2 英文军事网站、S3 第二家独立英语来源；来源族：CNN 6/18・6/30、BBC、War on the Rocks、Breaking Defense、Defense News、CNAS、CSIS、Bloomberg（标题可读）、Reuters 镜像（同题包）；确定有效匹配：[['CNN 6/18・6/30、BBC', 'S1 英语主流媒体'], ['War on the Rocks、Breaking Defense、Defense News、CNAS、CSIS', 'S2 英文军事网站'], ['Bloomberg（标题可读）、Reuters 镜像（同题包）', 'S3 第二家独立英语来源']]；待核验：[]。三槽；Reuters 原站全部 401，ISW 全部 403
- **G07-2 演进与反制**（v=1，m=2，k=2）槽位：S1 英文研究机构、S2 英语媒体；来源族：CNAS、CSIS、War on the Rocks、CNN、Reuters（wayback ×2 可读）；确定有效匹配：[['CNAS、CSIS、War on the Rocks', 'S1 英文研究机构'], ['CNN、Reuters（wayback ×2 可读）', 'S2 英语媒体']]；待核验：[]。两槽
- **G07-3 供应链与产能**（v=1，m=2，k=1）槽位：S1 乌方/北约官方（英文）、S2 独立英文媒体或研究；来源族：、CSIS 供应链、Reuters 3/10/2025（乌国防部采购计划，wayback 可读）；确定有效匹配：[['CSIS 供应链、Reuters 3/10/2025（乌国防部采购计划，wayback 可读）', 'S2 独立英文媒体或研究']]；待核验：[]。乌方官方数字均经媒体转述，无官方英文原始来源；北约官方无

### O5 冲突证据裁决（按任务卡 C 项四步各 0/0.5/1）

| id | v | 理由 |
|---|---|---|
| C07-1-发现 | 1 | §一表：国防部 555 → 992（24h）vs Sobyanin 180 → 194，标‘ISW 记录，口径不一’ |
| C07-1-列证据 | 1 | ISW/CNN/ABC 口径并列 |
| C07-1-比较理由 | 1 | 全国 vs 莫斯科方向、当夜 vs 24 小时 |
| C07-1-结论或存疑 | 1 | ‘官方声称，无法独立核验’‘所有拦截数字均为单方声称’ |
| C07-2-发现 | 1 | §四：CSIS 四大瓶颈集中中国、双方共用中国部件生态；乌转向台日 |
| C07-2-列证据 | 0.5 | 仅 CSIS 一源；替代供应商为‘媒体转引未核’ |
| C07-2-比较理由 | 0.5 | 指出‘具体比例数字不采信’，承认口径差异但未呈现各家数字 |
| C07-2-结论或存疑 | 0.5 | ‘中国部件依赖是已确认分析’——存疑保留，未裁决比例 |

### O8 关键进程覆盖（按任务卡 U 项 0/0.5/1）

| id | v | 理由 |
|---|---|---|
| U07-1 | 1 | §一/§二：6/16 CDU-6、6/18 Euro+、一周内两度命中 |
| U07-2 | 0 | 2025 年 6 月‘蛛网行动’未提 |
| U07-3 | 1 | §三初期：TB2、Shahed 2022 秋、Lyutyi 2022-10 |
| U07-4 | 0.5 | §三中期：FPV/电子战/光纤有；Rubicon 未提 |
| U07-5 | 0.5 | §三近期：诱饵/AI/光纤/远程常态化有；海上无人艇未提 |
| U07-6 | 0 | 6/28 普京承认燃料短缺及限供未提（仅普京关于空防表态） |

### O9 交付合规（R 型清单 0/0.5/1；交付期限 NA）

| id | v | 理由 |
|---|---|---|
| 核心判断或摘要 | 1 | §一开篇‘事件已确认发生’＋证据等级表 |
| 整体证据入口或索引 | 1 | §六 22 条 URL（无标题）＋限制说明 |
| 事实与证据映射交付 | 0.5 | 句内具名，无句级编号/URL；清单与句子不对应 |
| 不确定性与限制说明 | 1 | 证据等级列、‘未证实’标注、限制说明逐项 |
| 预测或情景时间窗 | 0.5 | §五趋势无明确时间窗（任务卡‘未来五年’） |
| 资料截止时点 | 0.5 | 未明示；最新事实 2026-07 北约峰会 |
| 按约定期限提交 | NA |  |

## 六、待补材料与变更请求


## 七、人工层与综合结果（留空，由云起/真人专家填写）

| 维度 | 层内权重 | 专家A等级(0–4) | 专家B等级(0–4) | 采用百分分 | 原文表现与理由 |
|---|---:|---|---|---|---|
| S2 严谨性与研判质量 | 35% |  |  |  |  |
| S1 全面性与重点把握 | 30% |  |  |  |  |
| S3 诚实性与不确定性表达 | 20% |  |  |  |  |
| S4 可读性与使用便利 | 15% |  |  |  |  |

专家层 H：________　原始综合分 Q = 0.6×B + 0.4×H：________　裁决后分：________　试行档位：________

重大缺陷确认（两名真人）：________　V1/V2 复核结论：________

> 本文件为模型基础层试评结果；未经真人复核与人工层评分，不构成综合质量判断，不得把 B 或 0.6B 当作综合分。