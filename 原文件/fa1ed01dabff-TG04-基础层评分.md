# TG04 基础层评分（V3.3R2 试评｜单模型初评）

- 报告：檀棋2.0-GPT6基模《美国海岸警卫队“哨兵级”转赴亚太后的活动特点与影响》（冻结快照；2026-09-24 文件）
- 评测性质：有题面
- 报告版本：sha256 a3eb1f2ea463…
- 主标准／公式版本：V3.3R2 模型评估修订稿 2026-09-10；r2_calc-1.0
- 任务卡／台账／证据包：Q04-任务卡；TG04-台账.json（build_ledger v1＋规则/人工复核：人工复核改判 26 条；人工复核改判 48 条；人工复核改判 63 条；人工复核改判 63 条；人工复核改判 68 条）；台账/TG04/evidence（fetch_evidence 2026-09-28：22 源 19 可读；GlobalSecurity 403→wayback、DVIDS 一条 404、Runtime Error 一条）
- 资料截止时点：活动记录分布 2026-06 至 2026-09（报告自述）
- 运行条件：同 00-执行口径与状态.md；单模型初评（Claude）；檀棋2.0-Kimi基模系列
- 过程状态：初评完成
- 综合结果状态：仅基础层；S1–S4、H、Q、档位留空待人工

## 一、基础层结果

**基础质量分 B（初评）：79.8–81.0（含U范围）**　状态：有效U

| 维度 | 得分或范围 | 分子／分母 | 基础权重 | 有效权重 | 口径与状态 |
|---|---:|---|---:|---:|---|
| O1 判定点达成 | 85.0 | P=8.50／W=10.00（已判9，U0，NA0） | 30 | 30.0 | 按任务卡 R 项逐项 0/0.5/1，理由附原文位置；D 项权重 2｜有效 |
| E1 事实与证据支持审计 | 94.4 | P=25.50／W=27.00（已判27，U0，NA0） | 20 | 20.0 | 全查：核心10条（w=1）＋其余17条（w=17/17=1.0000）；台账事实候选 27 条｜有效 |
| O7 来源合规可追溯 | 85.1–92.6 | P=23.00／W=27.00（已判25，U2，NA0） | 15 | 15.0 | 有 URL 标准口径：可读且对应 1；仅来源名/清单指认 0.5；无来源 0；不可读/失效 U；违反来源约束 0｜有效U |
| O2 独立信源多样性 | 72.2 | G04-1 部署事实:2/3；G04-2 活动与 MCA:2/2；G04-3 意图与影响:1/2 | 10 | 10.0 | 任务卡需求组等权；edges 仅计已核出有效来源｜有效 |
| O5 冲突证据裁决 | 50.0 | P=4.00／W=8.00（已判8，U0，NA0） | 10 | 10.0 | 按任务卡 C 项四步各 0/0.5/1｜有效 |
| O8 关键进程覆盖 | 58.3 | P=3.50／W=6.00（已判6，U0，NA0） | 10 | 10.0 | 按任务卡 U 项 0/0.5/1｜有效 |
| O9 交付合规 | 91.7 | P=5.50／W=6.00（已判6，U0，NA1） | 5 | 5.0 | R 型清单 0/0.5/1；交付期限 NA｜有效 |

说明：有 U 时给范围（下界向下、上界向上取 1 位），不是统计置信区间；B 不套用综合档位。

## 二、可用性检查与重大缺陷候选（模型候选，待真人确认）

- V1 核心证据与推理最低基础：**检查未见候选**。核心 10 条全部与 Janes/DVIDS/Stripes/第七舰队原文一致 问题ID：
- V2 时效关键窗口：**NA**。
- 重大缺陷候选：检查未见候选（不等于已确认通过）

## 三、核心依赖记录

| 核心判断 | 依赖事实ID | 支持状态 | 推理连接 | 是否需复核 |
|---|---|---|---|---|
| 前沿合作部署而非固定争议海域巡逻 | ['TG04-P020-S01', 'TG04-P030-T', 'TG04-P032-T', 'TG04-P033-T'] | A/A/A/A | 官方图注/公告链 | 否 |

## 四、问题清单（唯一编号，主要维度归属）

| 问题ID | 主要维度 | 次要影响 | 描述 | 原文位置 |
|---|---|---|---|---|
| ITG04-01 | O9 | [] | 正文残留 4 处“该项无法从本次冻结快照中的证据得到核实，故不作为结论”模板句，直接跟在有引用的事实句后，自相矛盾 | §1 |
| ITG04-02 | O1 | ['O8'] | 3 月转场/4 月补给节点、东海活动、参数口径冲突未涉及；影响分析无量化 | §4/§7 |

## 五、逐项判定

### O1 判定点（按任务卡 R 项逐项 0/0.5/1，理由附原文位置；D 项权重 2）

| id | w | v | 理由 | 问题ID |
|---|---|---|---|---|
| R04-01 | 1 | 1 | §2.1：6 艇具名（Stripes 7/20）、原驻巴林、7/15 公告转向西太、新加坡/苏比克、授权至 2026-09（Janes） |  |
| R04-02 | 1 | 1 | §2.2–2.3：新加坡指挥后勤/苏比克轮流进入（Janes），并明确“轮换”指节点使用而非已知换班表 |  |
| R04-03 | 1 | 0.5 | §4：多地合作清楚、“固定规律尚不可测”；无频次/周期数据（诚实标注） |  |
| R04-04 | 1 | 0.5 | §1/§4：南海有具体记录（6/18 MCA），东海不能确认；位置精度止于“南海” |  |
| R04-05 | 1 | 1 | §3 逐艇时间线：6/9、6/18、6/26、7/15–16、9/2、9/5 均具日期、地点、来源，并保留图注/Date Taken 差异 |  |
| R04-06 | 1 | 1 | §6 意图：公开任务表述 vs 前沿可用性 vs 专门对华三层，逐层给证据边界 |  |
| R04-07 | 1 | 0.5 | §7 影响：对美/伙伴/中国周边分列，但均为机制性可能，无量化或地区反应材料（自陈） |  |
| R04-08 | 1 | 1 | 全文对象为哨兵级 FRC（WPC 1141/1145 等），未混入 NSC |  |
| R04-D1 | 2 | 1 | §2 六艇表逐艇列“已确认 Fact 未提供具体亚太活动”，只以 Moulthrope/Tunnell 两艇立论 |  |

### E1 事实与证据支持（全查：核心10条（w=1）＋其余17条（w=17/17=1.0000）；台账事实候选 27 条）

抽样：种子 2026092804，抽样框 85 条，样本 17 条，核心全查 10 条；台账事实候选合计 194。

标签计数：A 24；P 3

| id | 核心 | 标签 | w | 理由 | 问题ID |
|---|---|---|---|---|---|
| TG04-P004-S02 | True | A | 1 | ref-4 Stripes：六艇 Robert Goldman/Charles Moulthrope/Glen Harris/Emlen Tunnell/John Scheuerman/Clarence Sutphin Jr. |  |
| TG04-P008-S01 | True | A | 1 | USCG 7/15 新闻稿（ref-9/11 GlobalSecurity 转载 403→wayback 可读）；Janes ref-1 同述转向西太、海上安全与伙伴合作 |  |
| TG04-P009-S02 | True | A | 1 | ref-5 DVIDS：260609 SUBIC BAY (June 9, 2026) Emlen Tunnell moors alongside…；Date Taken 6/8 差一天属实 |  |
| TG04-P020-S01 | True | A | 1 | ref-1 Janes：command and logistics handled out of Singapore and vessels rotating through Subic Bay |  |
| TG04-P026-S01 | True | A | 1 | ref-1 Janes：approved to operate from Singapore and Subic Bay through September [2026] |  |
| TG04-P029-T | True | A | 1 | ref-5 DVIDS 6/9 苏比克双艇靠泊 |  |
| TG04-P030-T | True | A | 1 | ref-3 DVIDS：South China Sea (June 18, 2026) AFP AW109 flies over Charles Moulthrope, MCA |  |
| TG04-P032-T | True | A | 1 | ref-6 第七舰队 7/16：CARAT Thailand 32nd concludes，Emlen Tunnell/Charles Moulthrope 参演 |  |
| TG04-P033-T | True | A | 1 | ref-17 DVIDS：Spencer Stout MET/ECS leads VBSS training aboard Emlen Tunnell, Jakarta, Sept. 2, 2026, Super Garuda Shield |  |
| TG04-P035-T | True | A | 1 | ref-8 DVIDS 9/5 Java Sea：与 KRI Siwar/Beladau 编队；ref-21 Photex 9/5 |  |
| TG04-P034-T | False | A | 1.0 | ref-19 Puspen TNI：Kopaska 与 US Navy 在 Charles Moulthrope 艇上 survey dan latihan parsial，Tanjung Priok，Rabu 2/9/2026，VBSS/CQB |  |
| TG04-P051-S02 | False | P | 1.0 | 6 月靓泊图片 7/15 发布：ref-12 404，发布日期未核 |  |
| TG04-P039-S02 | False | P | 1.0 | 两名艇长参加梭桃邑闭幕式：ref-6 正文未核到 commanding officer 出席句；ref-16 jina 部分可读 |  |
| TG04-P065-S02 | False | P | 1.0 | ref-14 Runtime Error 不可读；“支援印太司令部”未核 |  |
| TG04-P057-S02 | False | A | 1.0 | ref-10 艇员、ref-17 MET、ref-19 US Navy——三类参与者属实 |  |
| TG04-P057-S01 | False | A | 1.0 | ref-10 AFP、ref-19 Kopaska、ref-6 RTN |  |
| TG04-P043-S01 | False | A | 1.0 | ref-8/21：9/5 Java Sea transit 与 Photex 编队 |  |
| TG04-P041-S01 | False | A | 1.0 | ref-17 DVIDS：MET/ECS Spencer Stout 带训（Tunnell）；ref-19 Puspen TNI 称 US Navy（Moulthrope）——差异属实 |  |
| TG04-P084-T | False | A | 1.0 | 结论表：活动记录 6–9 月、授权披露至 9 月——与各源一致 |  |
| TG04-P065-S01 | False | A | 1.0 | ref-1 Janes 正文：operating from forward locations in Singapore and the Philippines to protect the homeland and maritime approaches, including Guam and the Pacific islands（ref-14 不可读，ref-1 同文） |  |
| TG04-P009-S01 | False | A | 1.0 | ref-5 图注 June 9, 2026 |  |
| TG04-P039-S01 | False | A | 1.0 | ref-6 第七舰队闭幕报道列出 Emlen Tunnell/Charles Moulthrope |  |
| TG04-P070-S01 | False | A | 1.0 | ref-10 损管、ref-17 VBSS、ref-6 CARAT、ref-8 编队航行 |  |
| TG04-P050-S01 | False | A | 1.0 | 6/18 MCA（ref-3）、CARAT Thailand（ref-6）、Super Garuda Shield（ref-17）均核实 |  |
| TG04-P008-S02 | False | A | 1.0 | ref-9/11 为 GlobalSecurity 转载 USCG 新闻稿（自陈属实） |  |
| TG04-P031-T | False | A | 1.0 | ref-10 DVIDS：Emlen Tunnell 舰员 damage control training with AFP, Subic Bay, June 26, 2026 |  |
| TG04-P021-S01 | False | A | 1.0 | ref-15（同 ref-5 DVIDS 图注）：ECS 描述为具指挥/后勤/支援能力的可部署 FRC 力量；ref-12 404 |  |

### O7 来源合规可追溯（有 URL 标准口径：可读且对应 1；仅来源名/清单指认 0.5；无来源 0；不可读/失效 U；违反来源约束 0）

| id | w | v | 理由 |
|---|---|---|---|
| TG04-P004-S02/引用 | 1 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P008-S01/引用 | 1 | 0.5 | ref-9/11 GlobalSecurity 403（wayback 有正文），按具名 0.5 |
| TG04-P009-S02/引用 | 1 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P020-S01/引用 | 1 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P026-S01/引用 | 1 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P029-T/引用 | 1 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P030-T/引用 | 1 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P032-T/引用 | 1 | 1 | ref-6 proxy 可读对应；ref-16 jina 可读 |
| TG04-P033-T/引用 | 1 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P035-T/引用 | 1 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P034-T/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P051-S02/引用 | 1.0 | U | ref-12 404 |
| TG04-P039-S02/引用 | 1.0 | 1 | ref-6/7 可读；ref-16 jina |
| TG04-P065-S02/引用 | 1.0 | U | ref-14 400 Runtime Error |
| TG04-P057-S02/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P057-S01/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P043-S01/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P041-S01/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P084-T/引用 | 1.0 | 0 | 结论表无引用 |
| TG04-P065-S01/引用 | 1.0 | 1 | ref-14 不可读但 ref-1 同文可读对应 |
| TG04-P009-S01/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P039-S01/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P070-S01/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P050-S01/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P008-S02/引用 | 1.0 | 0.5 | ref-9/11 403 |
| TG04-P031-T/引用 | 1.0 | 1 | [[n]](#fact-reference-n)→参考文献块外部 URL，抓取可读且对应 |
| TG04-P021-S01/引用 | 1.0 | 1 | ref-15 可读对应；ref-12 404 |

### O2 独立信源分组匹配（任务卡需求组等权；edges 仅计已核出有效来源）

- **G04-1 部署事实**（v=1，m=3，k=2）槽位：S1 美方官方（USCG/INDOPACOM/第七舰队）、S2 独立专业媒体、S3 菲律宾/新加坡方来源；来源族：USCG 新闻稿（GlobalSecurity 转载）/DVIDS/第七舰队、Janes/Stripes、；确定有效匹配：[['USCG 新闻稿（GlobalSecurity 转载）/DVIDS/第七舰队', 'S1 美方官方（USCG/INDOPACOM/第七舰队）'], ['Janes/Stripes', 'S2 独立专业媒体']]；待核验：[]。两槽有效
- **G04-2 活动与 MCA**（v=1，m=2，k=2）槽位：S1 美方官方、S2 菲方官方/媒体；来源族：DVIDS/第七舰队、Puspen TNI/ISDS（印尼官方，非菲方）；确定有效匹配：[['DVIDS/第七舰队', 'S1 美方官方'], ['Puspen TNI/ISDS（印尼官方，非菲方）', 'S2 菲方官方/媒体']]；待核验：[]。菲方来源缺，印尼官方通报替代（同类伙伴国官方）计 1
- **G04-3 意图与影响**（v=1，m=2，k=1）槽位：S1 官方说明、S2 独立分析；来源族：USCG/Janes 引述发言人、；确定有效匹配：[['USCG/Janes 引述发言人', 'S1 官方说明']]；待核验：[]。无独立分析来源

### O5 冲突证据裁决（按任务卡 C 项四步各 0/0.5/1）

| id | v | 理由 |
|---|---|---|
| C04-1-发现 | 0 | 哨兵级参数口径差异未涉及 |
| C04-1-列证据 | 0 |  |
| C04-1-比较理由 | 0 |  |
| C04-1-结论或存疑 | 0 |  |
| C04-2-发现 | 1 | §2.1/§7：授权至 9 月的节点使用 vs 常态化前沿存在 |
| C04-2-列证据 | 1 | Janes 授权期限、DVIDS“持续前沿行动”描述、USCG 公告 |
| C04-2-比较理由 | 1 | 区分部署调整与临时访问；期限后须授权更新支持 |
| C04-2-结论或存疑 | 1 | 判为“既有力量区域部署调整”，持续性待授权续期复核 |

### O8 关键进程覆盖（按任务卡 U 项 0/0.5/1）

| id | v | 理由 |
|---|---|---|
| U04-1 | 1 | 7/15 USCG 公告（§2.1） |
| U04-2 | 0 | 3 月转场未提 |
| U04-3 | 0 | 4 月新加坡补给未提 |
| U04-4 | 1 | 6/9 苏比克到位、6/18 南海 MCA、6/26 损管训练 |
| U04-5 | 1 | 轮流进入苏比克机制与授权期限 |
| U04-6 | 0.5 | MCA 记录 6/18、6/26 两次，无统计 |

### O9 交付合规（R 型清单 0/0.5/1；交付期限 NA）

| id | v | 理由 |
|---|---|---|
| 核心判断或摘要 | 1 | 第一章摘要 |
| 整体证据入口或索引 | 1 | 参考文献 22 条带摘录与 URL |
| 事实与证据映射交付 | 1 | 句级 [[n]] 锚点 |
| 不确定性与限制说明 | 1 | §8 三项边界、证据使用说明 |
| 预测或情景时间窗 | 1 | §7 时间与复核条件（9 月授权节点） |
| 资料截止时点 | 0.5 | “活动记录主要分布在 6–9 月”，无明确基准日 |
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