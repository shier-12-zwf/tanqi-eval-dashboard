# TV05 基础层评分（V3.3R2 试评｜单模型初评）

- 报告：檀棋2.0-ArctiSwarm（DeepSeek-V4-flash 基模）《俄乌战争中无人与反无人作战体系——聚焦2026年6月中旬乌克兰对莫斯科的大规模无人机袭击》
- 评测性质：有题面
- 报告版本：sha256 d7525dedc021…
- 主标准／公式版本：V3.3R2 模型评估修订稿 2026-09-10；r2_calc-1.0
- 任务卡／台账／证据包：Q05-任务卡；TV05-台账.json（build_ledger v1＋规则/人工复核：fix_refs_tv：来源表 34 条，句级编号映射 0 单元；人工复核改判 55 条；清单按来源名/日期指认挂载 31 单元）；台账/TV05/evidence（fetch_evidence 2026-10-08：27 源 15 可读；Reuters ×12 401、ISW ×2 403、FT 403）＋同题证据包复用：B7F/ref-0010（Reuters 6/18 MarketScreener 镜像）、DS07/ref-5（Reuters 6/24 mil.in.ua 镜像）、Q05/ref-3 WaPo、TG07/ref-30、B7E/ref-0157・0016・0002、K09/ref-0008、TK05/ref-13・ref-8・ref-30、Q07/ref-3；补查 2026-10-09：Reuters 9/15 经 ground.news 全文镜像＋TechTimes 9/29、Reuters 2023-12-19 经 Wayback（补查/）；其余 Reuters 2026 年条目 Wayback 无快照；web_search 工具不可用（DDG 验证码、Bing 失真），已记录
- 资料截止时点：报告未标注；最新事实为 2026-09-20（莫斯科袭击）
- 运行条件：同 00-执行口径与状态.md；单模型初评（Claude）；檀棋2.0-ArctiSwarm DeepSeek-V4-flash 基模系列
- 过程状态：初评完成
- 综合结果状态：仅基础层；S1–S4、H、Q、档位留空待人工

## 一、基础层结果

**基础质量分 B（初评）：69.3–80.4（含U范围）**　状态：有效U

| 维度 | 得分或范围 | 分子／分母 | 基础权重 | 有效权重 | 口径与状态 |
|---|---:|---|---:|---:|---|
| O1 判定点达成 | 80.0 | P=8.00／W=10.00（已判9，U0，NA0） | 30 | 30.0 | 按任务卡 R 项逐项 0/0.5/1，理由附原文位置；D 项权重 2｜有效 |
| E1 事实与证据支持审计 | 59.3–86.4 | P=31.43／W=53.00（已判30，U10，NA0） | 20 | 20.0 | 初筛：核心10条（w=1）＋其余30条（w=43/30=1.4333）；台账事实候选 53 条｜有效U |
| O7 来源合规可追溯 | 25.9–63.3 | P=13.75／W=53.00（已判25，U15，NA0） | 15 | 15.0 | 无句级 URL 口径（Q05 来源约束：英语主流媒体/英语专业军事网站）：句内具名＋文末清单可读对应 0.5（上限）；清单不可读（Reuters 401/ISW｜有效U |
| O2 独立信源多样性 | 83.3 | G05-1 核心事件事实:3/3；G05-2 演进脉络与战例:2/2；G05-3 产能与产业:1/2 | 10 | 10.0 | 任务卡需求组等权；edges 仅计已核出有效来源｜有效 |
| O5 冲突证据裁决 | 87.5 | P=7.00／W=8.00（已判8，U0，NA0） | 10 | 10.0 | 按任务卡 C 项四步各 0/0.5/1｜有效 |
| O8 关键进程覆盖 | 83.3 | P=5.00／W=6.00（已判6，U0，NA0） | 10 | 10.0 | 按任务卡 U 项 0/0.5/1｜有效 |
| O9 交付合规 | 83.3 | P=5.00／W=6.00（已判6，U0，NA1） | 5 | 5.0 | R 型清单 0/0.5/1；交付期限 NA｜有效 |

说明：有 U 时给范围（下界向下、上界向上取 1 位），不是统计置信区间；B 不套用综合档位。

## 二、可用性检查与重大缺陷候选（模型候选，待真人确认）

- V1 核心证据与推理最低基础：**检查未见候选**。核心 10 条：补查后 7A+3P；样本无 N；Reuters 12 条中 2 条经镜像/Wayback 核到 问题ID：
- V2 时效关键窗口：**NA**。
- 重大缺陷候选：检查未见候选（不等于已确认通过）

## 三、核心依赖记录

| 核心判断 | 依赖事实ID | 支持状态 | 推理连接 | 是否需复核 |
|---|---|---|---|---|
| 6/18 袭击为全面战争以来最大规模、一周内两度瘫痪莫斯科炼油厂两大装置，规模曲线持续抬升 | ['TV05-P003-S02', 'TV05-P004-S01', 'TV05-P005-S02', 'TV05-P005-S03', 'TV05-P009-S03'] | A/P/A/A/A | CNN/ABC/BBC＋Reuters 镜像＋ISW | 否 |

## 四、问题清单（唯一编号，主要维度归属）

| 问题ID | 主要维度 | 次要影响 | 描述 | 原文位置 |
|---|---|---|---|---|
| ITV05-01 | O7 | ['E1'] | 清单 34 条中 Reuters 12 条全部 401、ISW 6/18・4/9 403、FT 403；核心/样本 15 条据此记 U；凡能在同题证据包镜像核到者 E1 已给 A/P | §五 |
| ITV05-02 | O9 | [] | 无句级编号或 URL，仅句内具名＋四类口径标签；清单按来源分组但不与句子对应 | 全文 |
| ITV05-03 | O1 | [] | R05-07 瓶颈（部件/供应链）无事实；R05-05 战例无共同比较字段；R05-D1 未列质变维度与不可比项 | §二/§三 |
| ITV05-04 | E1 | [] | ‘3/11 74 架前纪录’‘莫斯科三分之一汽油供应’‘每三个被毁中一个由拦截机完成’‘500–700 km/h 拦截机’‘Skyfall 370 km/h’‘欧盟 11 亿美元协议’等 6 处在证据包与补查中均未核到 | §一/§三/§四 |
| ITV05-05 | O8 | [] | U05-5 2024 库尔斯克战例缺失；‘16 人受伤’与 WaPo/Kyiv Independent ‘17 人’口径未并列 | §一/§二 |

## 五、逐项判定

### O1 判定点（按任务卡 R 项逐项 0/0.5/1，理由附原文位置；D 项权重 2）

| id | w | v | 理由 | 问题ID |
|---|---|---|---|---|
| R05-01 | 1 | 1 | §一：2026-06-18 凌晨、莫斯科炼油厂（Kapotnya，距克宫 15 km）、194/555/992——日期、目标、规模唯一对应，多家英文媒体 |  |
| R05-02 | 1 | 1 | §一：规模（194/555/992/239）、战果（CDU-6 53%、Euro+ 47%、6 个月停产）、技术（FP-1/An-196/Bars，标 OSINT）、战术（波浪式+诱饵，CSIS Bondar）、战略影响（防空再部署、40 天行动） |  |
| R05-03 | 1 | 1 | §一末段：3/11 74 架前纪录、6/16 60→6/18 194→6/19 76→6/22 84→9/20 450，给出可比指标（莫斯科方向拦截数）与出处 |  |
| R05-04 | 1 | 1 | §二三阶段（2022 TB2/Shahed；2023–24 FPV/军种化；2024–26 光纤/喷气/拦截机），每阶段附 RUSI/CNAS/ABC/Reuters 依据 |  |
| R05-05 | 1 | 0.5 | 标志性战例（5/3/2023 克宫、6/18、9/20）散见但未用共同比较字段并列 |  |
| R05-06 | 1 | 1 | §三：拦截率 90%/57%/60%、单架 3000–5000 美元、2 月 6300 架次/1500 架、炼油产能 42.74%/>20%/28%——保留期间与口径标签 |  |
| R05-07 | 1 | 0.5 | 产量 100 万/400 万/700 万/1000 万/2000 万、制造商 7→500 家有来源；瓶颈（部件/供应链/融资）仅‘融资可行性’一句，无具体瓶颈事实 |  |
| R05-08 | 1 | 1 | §四：速度竞赛、光纤/AI、军种化外溢、工业合作四方向各有来源，并给条件化判断 |  |
| R05-D1 | 2 | 0.5 | ‘规模曲线持续抬升’‘方法革新’有比较，但未事先列出质变判断维度，也未说明哪些部分不可比（如俄方拦截数 vs 乌方发射数无法对账） |  |

### E1 事实与证据支持（初筛：核心10条（w=1）＋其余30条（w=43/30=1.4333）；台账事实候选 53 条）

抽样：种子 2026100805，抽样框 43 条，样本 30 条，核心全查 10 条；台账事实候选合计 83。

标签计数：A 19；P 11；U 10

| id | 核心 | 标签 | w | 理由 | 问题ID |
|---|---|---|---|---|---|
| TV05-P003-S02 | True | A | 1 | TV05 包 ref-15 CNN 6/18（可读）‘largest attack on Moscow since start of full-scale war’、ref-21 ABC、ref-13 AP（jina）、ref-18 Bloomberg（jina）同日报道；ref-25 ISW 6/19 可读 |  |
| TV05-P004-S01 | True | P | 1 | ref-15 CNN：at least 194 drones…according to Sobyanin；Q05 包 ref-3 WaPo 同；‘3 月 11 日 74 架前纪录’未在任何证据包核到 |  |
| TV05-P004-S02 | True | A | 1 | Q05 包 ref-3 WaPo：Defense Ministry…at least 992 drones…in the past 24 hours；555 见 Q05 包 ref-1/2/5 |  |
| TV05-P005-S02 | True | A | 1 | B7F 包 ref-0010 MarketScreener（Reuters 6/18 全文转载）：June 16 attack…CDU-6…53% of the plant's capacity…damaged and caught fire；Sources said |  |
| TV05-P005-S03 | True | A | 1 | 同上：Thursday's attack damaged the Euro+ combined oil refining unit…crude distillation section…140,000 bpd—47% of the refinery's capacity |  |
| TV05-P006-S03 | True | P | 1 | DS07 包 ref-5 mil.in.ua 转 Reuters 6/24：expected to remain out of operation for at least six months、until 2027；‘直接影响莫斯科地区约三分之一汽油供应’未核到 |  |
| TV05-P009-S03 | True | A | 1 | ref-14 BBC 9/20（可读）：450 drones downed…two people died、parliamentary election third day；TG07 包 ref-30：more than 1,600 drones since Saturday；ref-17 CNN：at least three people killed——‘2-3 人’口径差异报告已并列 |  |
| TV05-P012-S05 | True | P | 1 | ref-32 War on the Rocks（可读）：Syrskyi 3/3 称 2 月拦截机 6,300 架次、击毁 1,500+、基辅 70%+ Shahed 由拦截机击落——对应；ref-33 Defense News 3/5 可读但‘每三个被毁中约一个由拦截机完成’未在抓取文本核到 |  |
| TV05-P018-S01 | True | A | 1 | ref-8 Reuters 9/15 原站 401；补查 ground.news 全文镜像（补查/groundnews-jet.html）：‘Ukraine previously achieved around 90% interception rates against slower Shahed-type UAVs, new jet models fly at speeds exceeding 400 km/h’；57% 见 TechTimes 9/29（补查/techtimes-57.html，引乌空军 as of 9/28）——数字与方向均对应，‘57% 出自 Reuters’归属略偏 |  |
| TV05-P022-S01 | True | A | 1 | ref-12 Reuters 2023-12-19 经 Wayback（20231227 快照，补查/reuters-20231219-wayback.txt）可读：‘Ukraine will produce one million drones next year…Zelenskiy said on Tuesday’ |  |
| TV05-P023-S02 | False | U | 1.4333 | 无 URL；B7E 包 drone-warfare 载 370 km/h 为某拦截机争议数值（另说 600），未与 Skyfall/Breaking Defense 对应 |  |
| TV05-P007-S01 | False | P | 1.4333 | 无 URL；B7E 包 drone-warfare.com An-196 Liutyi/FP-1 研究页存在，‘该波次为 FP-1/An-196/Bars 混编’的 CyberBoroshno 判读未定位；报告已标 OSINT 未证实 |  |
| TV05-P017-S01 | False | P | 1.4333 | ref-24 ISW 6/18 403；ref-25 ISW 6/19 可读：Russian air defenses performing well ‘despite everything’…large number of Ukrainian drones；‘军事博主约 90%’未核到 |  |
| TV05-P011-S03 | False | A | 1.4333 | ref-22 ABC（可读）：Ukraine on Tuesday [June 11, 2024] launched its Unmanned Systems Forces…first of its kind；Zelenskyy announced in February |  |
| TV05-P005-S05 | False | A | 1.4333 | ref-15 CNN：Video geolocated by CNN showed…drones approached the refinery；厂区大火 |  |
| TV05-P014-S01 | False | U | 1.4333 | ref-27 ISW 4/9 403；1/2/3 月 41/61/115 次中程打击未核 |  |
| TV05-P026-S02 | False | U | 1.4333 | 无 URL（句内具名 DW）；B7E 包命中‘1.1 billion’为欧盟贸易数据，非无人机协议；未核 |  |
| TV05-P015-S03 | False | A | 1.4333 | ref-19 FT 403；B7E 包 ref-0157（Wikipedia 转 FT）：Russia produced 4.1 million bpd in June 2026 (28% below the 5-year average)；B7E ref-0028 drone-warfare：fuel restrictions affecting roughly 50 million people |  |
| TV05-P022-S05 | False | A | 1.4333 | ref-29 CSIS Beyond Parallel（可读）：Yelabuga…reportedly producing more than 5,500 units per month |  |
| TV05-P011-S04 | False | U | 1.4333 | ref-31 RUSI 页面仅摘要（2,686 字）；‘俄 2024 年 12 月组建无人系统兵种’未核 |  |
| TV05-P026-S01 | False | P | 1.4333 | ref-9 Reuters 7/24 401；Q08/Q06 包存在 ‘Drone Dominance’ 计划（DIU）页面；美乌联合生产谈判 7/24 具体报道未打开 |  |
| TV05-P004-S03 | False | A | 1.4333 | B7E 包 ref-0002 ABC 6/18：Russia…firing at least seven ballistic missiles and 239 drones at Ukraine overnight, the General Staff said（报告写‘乌空军口径经 ISW 转引’，出处层级小偏差） |  |
| TV05-P015-S01 | False | A | 1.4333 | B7E 包 ref-0157（Wikipedia 引乌总参 7/4）：General Staff estimated 42.74% of Russia's oil refining capacity had been disabled |  |
| TV05-P024-S02 | False | U | 1.4333 | 无 URL；Reuters 2024-12 乌收集数据训练 AI 报道未核 |  |
| TV05-P025-S02 | False | U | 1.4333 | 无 URL；乌 2026 年 7 月设‘远程打击联合指挥部’未核 |  |
| TV05-P012-S03 | False | U | 1.4333 | ref-10 Reuters 7/10 401；标题 russia-evades-ukraine-electrical-substation-defences-with-small-unjammable 与断言主题一致，正文未打开 |  |
| TV05-P022-S02 | False | P | 1.4333 | 无 URL；2025 年官方‘计划采购约 450 万架 FPV’（Reuters 3/10/2025，见 TV07 清单）为计划数；‘2025 超 400 万架’实际产量未核 |  |
| TV05-P008-S02 | False | P | 1.4333 | ISW 6/18 403；ISW 6/19 可读中含对俄防空与国内成本的评估性表述，原句未精确定位 |  |
| TV05-P009-S02 | False | A | 1.4333 | B7E 包 ref-0016 Moscow Times 6/16：Ukraine launched 60 drones at the capital；ref-15 CNN 194；K05 包 76（6/19）；TK05 包 ref-30 ISW 6/22：Sobyanin 84 drones |  |
| TV05-P008-S01 | False | U | 1.4333 | 无 URL；Zelensky 6/24 称俄向莫斯科/克里米亚大桥再部署防空——未核 |  |
| TV05-P006-S01 | False | P | 1.4333 | ref-3 Reuters 401；TK05 包 ref-8 CNBC：16 people injured；Q05 包 WaPo/Q07 包 Kyiv Independent：17 people——人数口径 16/17 并存 |  |
| TV05-P015-S02 | False | P | 1.4333 | 无 URL；B7E 包 ref-0157 载‘…while the International Energy A[gency]…’紧随 42.74% 之后，具体‘超过 20%’数值截断未见 |  |
| TV05-P012-S04 | False | A | 1.4333 | K09 包 ref-0008 ISIS 报告：Ukrainian Defence Intelligence assessed combined Geran-4/5 production at about 3,000 per month；jet-powered |  |
| TV05-P009-S01 | False | U | 1.4333 | ref-11 Reuters 2026-01-04 401；标题 ukraine-targets-moscow-daily-with-drones-this-year-russia-says 与断言一致，正文未打开 |  |
| TV05-P010-S02 | False | P | 1.4333 | ref-31 RUSI Watling & Reynolds 2025 页面仅摘要可读；TB2 失势为该系列报告通论，具体段落未核 |  |
| TV05-P008-S03 | False | A | 1.4333 | TK05 包 ref-13 Kyiv Post：Zelensky announced he had approved a 40-day SBU operation designed to increase pressure on Russia（6/25 前后） |  |
| TV05-P015-S04 | False | A | 1.4333 | B7E 包 ref-0157：On 23 June 2026, Deputy PM Novak stated the government was considering a ‘total ban’ on exports of diesel |  |
| TV05-P010-S03 | False | A | 1.4333 | Q05 包 ref-35 The Diplomat：Shahed/Alabuga 生产线自 2022 年 10 月起（Reuters 链接）；通论级事实，多包均载 |  |
| TV05-P023-S01 | False | U | 1.4333 | 无 URL；Defense News 2026-09 ‘500–700 km/h 拦截机在研’未核（B7D 包 700 km/h 为俄导弹参数，不对应） |  |
| TV05-P005-S04 | False | A | 1.4333 | Q07 包 ref-3 Kyiv Independent 6/18：At least five fires were reported at the Moscow Oil Refinery；General Staff confirmed damage |  |

### O7 来源合规可追溯（无句级 URL 口径（Q05 来源约束：英语主流媒体/英语专业军事网站）：句内具名＋文末清单可读对应 0.5（上限）；清单不可读（Reuters 401/ISW 403/FT 403）U；句内具名无 URL 0.5；无来源 0）

| id | w | v | 理由 |
|---|---|---|---|
| TV05-P003-S02/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV05-P004-S01/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV05-P004-S02/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV05-P005-S02/引用 | 1 | U | ref-2 Reuters 401 |
| TV05-P005-S03/引用 | 1 | U | ref-4 Reuters 401 |
| TV05-P006-S03/引用 | 1 | U | ref-5 Reuters 401 |
| TV05-P009-S03/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV05-P012-S05/引用 | 1 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV05-P018-S01/引用 | 1 | U | ref-8 Reuters 401 |
| TV05-P022-S01/引用 | 1 | 0.5 | ref-12 经 Wayback 可读且对应（无句级 URL 口径上限 0.5） |
| TV05-P023-S02/引用 | 1.4333 | 0.5 | 具名 Breaking Defense，无 URL |
| TV05-P007-S01/引用 | 1.4333 | 0.5 | 具名 drone-warfare.com/CyberBoroshno，无 URL |
| TV05-P017-S01/引用 | 1.4333 | U | ref-24 ISW 403 |
| TV05-P011-S03/引用 | 1.4333 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV05-P005-S05/引用 | 1.4333 | 0.5 | 具名 CNN，清单 ref-15 可读 |
| TV05-P014-S01/引用 | 1.4333 | U | ref-27 ISW 403 |
| TV05-P026-S02/引用 | 1.4333 | 0.5 | 具名 DW，无 URL |
| TV05-P015-S03/引用 | 1.4333 | U | ref-19 FT 403 |
| TV05-P022-S05/引用 | 1.4333 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV05-P011-S04/引用 | 1.4333 | U | ref-31 RUSI 仅摘要；美军期刊无 URL |
| TV05-P026-S01/引用 | 1.4333 | U | ref-9 Reuters 401 |
| TV05-P004-S03/引用 | 1.4333 | U | ref-24 ISW 403 |
| TV05-P015-S01/引用 | 1.4333 | 0.5 | 具名乌总参，无 URL |
| TV05-P024-S02/引用 | 1.4333 | 0.5 | 具名 Reuters 2024-12，无 URL |
| TV05-P025-S02/引用 | 1.4333 | 0 | 无来源名、无 URL |
| TV05-P012-S03/引用 | 1.4333 | U | ref-10 Reuters 401 |
| TV05-P022-S02/引用 | 1.4333 | 0 | 无来源名、无 URL |
| TV05-P008-S02/引用 | 1.4333 | 0.5 | 具名 ISW，清单 ISW 6/18 不可读、6/19 可读 |
| TV05-P009-S02/引用 | 1.4333 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV05-P008-S01/引用 | 1.4333 | 0 | 无来源名（仅‘Zelensky 引情报’）、无 URL |
| TV05-P006-S01/引用 | 1.4333 | U | ref-3 Reuters 401 |
| TV05-P015-S02/引用 | 1.4333 | 0.5 | 具名 IEA，无 URL |
| TV05-P012-S04/引用 | 1.4333 | U | ref-8 Reuters 401 |
| TV05-P009-S01/引用 | 1.4333 | U | ref-11 Reuters 401 |
| TV05-P010-S02/引用 | 1.4333 | 0.5 | 句内具名来源＋文末清单 URL 可读对应（无句级 URL 口径上限 0.5） |
| TV05-P008-S03/引用 | 1.4333 | 0.5 | 具名 Euronews，无 URL |
| TV05-P015-S04/引用 | 1.4333 | 0 | 无来源名、无 URL |
| TV05-P010-S03/引用 | 1.4333 | 0.5 | 具名 Reuters/CSIS 多篇，未指认具体条 |
| TV05-P023-S01/引用 | 1.4333 | 0.5 | 具名 Defense News 2026-09，无 URL |
| TV05-P005-S04/引用 | 1.4333 | U | ref-24 ISW 403 |

### O2 独立信源分组匹配（任务卡需求组等权；edges 仅计已核出有效来源）

- **G05-1 核心事件事实**（v=1，m=3，k=3）槽位：S1 英语主流媒体、S2 英语专业军事网站、S3 俄/乌官方英文或第二家独立英语媒体；来源族：CNN 6/18、BBC 9/20、ABC、ISW 6/19、War on the Rocks、Defense News、AP、Bloomberg（jina 可读）；确定有效匹配：[['CNN 6/18、BBC 9/20、ABC', 'S1 英语主流媒体'], ['ISW 6/19、War on the Rocks、Defense News', 'S2 英语专业军事网站'], ['AP、Bloomberg（jina 可读）', 'S3 俄/乌官方英文或第二家独立英语媒体']]；待核验：[]。三槽均可读；Reuters 全部 401 未计
- **G05-2 演进脉络与战例**（v=1，m=2，k=2）槽位：S1 英语专业研究、S2 英语主流媒体；来源族：CSIS Beyond Parallel、RUSI（摘要）、War on the Rocks、ABC（USF）、CNN；确定有效匹配：[['CSIS Beyond Parallel、RUSI（摘要）、War on the Rocks', 'S1 英语专业研究'], ['ABC（USF）、CNN', 'S2 英语主流媒体']]；待核验：[]。两槽
- **G05-3 产能与产业**（v=1，m=2，k=1）槽位：S1 乌方官方/行业（英文）、S2 独立英语媒体或研究；来源族：、CSIS Beyond Parallel（Yelabuga）；确定有效匹配：[['CSIS Beyond Parallel（Yelabuga）', 'S2 独立英语媒体或研究']]；待核验：[]。乌方官方产量数字均经 Reuters（401）转述，无可读官方英文来源

### O5 冲突证据裁决（按任务卡 C 项四步各 0/0.5/1）

| id | v | 理由 |
|---|---|---|
| C05-1-发现 | 1 | §一：Sobyanin 194 vs 国防部 555→992 vs 乌方 239 来袭并列 |
| C05-1-列证据 | 1 | 各数字标【官方】/【经 ISW 转引】并给来源 |
| C05-1-比较理由 | 1 | 说明口径差异（莫斯科上空 vs 全国 24 小时 vs 对向来袭） |
| C05-1-结论或存疑 | 1 | 明示‘官方口径，未独立核实’，不取单一数 |
| C05-2-发现 | 1 | §三：100 万（2024 目标）/400 万（2025）/700 万（2026 计划，Boiev）/1000 万（泽连斯基 G7）/2000 万（7 月）并列 |
| C05-2-列证据 | 1 | 逐条标【官方】/【官方/行业】与发言人 |
| C05-2-比较理由 | 0.5 | 区分‘目标/计划/产能’标签，但未解释 700 万 vs 1000 万 vs 2000 万差异来源 |
| C05-2-结论或存疑 | 0.5 | 列入‘关键未知：2000 万架融资可行性’，未裁决 |

### O8 关键进程覆盖（按任务卡 U 项 0/0.5/1）

| id | v | 理由 |
|---|---|---|
| U05-1 | 1 | §一：6/16 首袭 CDU-6、6/18 第二波 Euro+、6/19、6/22 逐日拦截数 |
| U05-2 | 0.5 | 1 月起几乎每日威胁（Reuters 1/4 标题对应，正文 401）；‘3/11 74 架前纪录’未核到——铺垫有但依据未核实 |
| U05-3 | 1 | §二阶段一：TB2 失势、Shahed 引入 |
| U05-4 | 1 | §二阶段二：FPV、USF 成立 |
| U05-5 | 0.5 | 2024 规模化有（USF、100 万目标）；库尔斯克无 |
| U05-6 | 1 | §二阶段三/§四：光纤 FPV、Geran-4/5、拦截机、AI 末端锁定 |

### O9 交付合规（R 型清单 0/0.5/1；交付期限 NA）

| id | v | 理由 |
|---|---|---|
| 核心判断或摘要 | 1 | §一开篇‘核验结论：事件确已发生，多源已证实’ |
| 整体证据入口或索引 | 1 | §五 34 条 URL 按来源分组 |
| 事实与证据映射交付 | 0.5 | 句内具名＋四类口径标签，无句级编号/URL |
| 不确定性与限制说明 | 1 | 四类标签贯穿全文；§四关键未知；限制说明 |
| 预测或情景时间窗 | 1 | §四条件化判断含 2026–2027 冬季与季度翻番 |
| 资料截止时点 | 0.5 | 未明示截止日期；最新事实 9/20 可推断 |
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