**JooooDev** — renewable power forecasting, weather-model
verification, electricity-market settlement. BSc atmospheric science, MSc
climate change and energy.

### Public work: each repository answers one question

| Repository | Question | Answer |
|---|---|---|
| [aiwp-china-verification](https://github.com/JoooDev-TPP/aiwp-china-verification) | Which of ten global weather models is most accurate at Chinese stations? | None overall — there is a best model per variable, and the ranking inverts between them. |
| [cn-weather-cube](https://github.com/JoooDev-TPP/cn-weather-cube) | How do you fetch point weather you can trust? | Every number carries its unit, every series names its source, and a unit mismatch is refused rather than passed through. |
| [Carbon-Footprint-LCA](https://github.com/JoooDev-TPP/Carbon-Footprint-LCA) | Where does 100 MW of solar avoid the most CO2? | 65% more in the North grid than the South; carbon payback is 8 months for onshore wind, about 3 years for utility solar. |
| [GBA-Air-Quality-Analysis](https://github.com/JoooDev-TPP/GBA-Air-Quality-Analysis) | Did Greater Bay Area air get better in 2015–2024? | PM2.5 halved; ozone did not move — and it now sets the AQI on four polluted days in five. |
| [green-ai-ledger](https://github.com/JoooDev-TPP/green-ai-ledger) | How much carbon did a compute job emit? | IP-based trackers apply the grid of the network exit; here the factor is pinned to a cited official source. |

### How they are built

- **Every conclusion recomputes from the data beside it.** In
  aiwp-china-verification, CI recomputes every report page from the committed
  data on every push and compares each number.
- **Corrections are dated and left in place**, not edited away.
- **Limits sit next to the number they limit** — which "observation" is a
  satellite retrieval, which "truth" is a reanalysis, how many station-days a
  ranking rests on.

### 中文

新能源功率预测、气象模式检验、电力市场结算测算。

上面每个仓库回答一个问题，做法相同：**每个结论都能从旁边那份数据重算出来**——aiwp
的 CI 每次推送都从数据把报告页重算一遍，逐个数字比对，对不上就是红的；**错了就改，
更正注明日期和原说法**——aiwp 2026-09-21 的更正把去偏改成样本外滚动估计，风速的名次因此换了第一；
**边界写在结论旁边，不写在末尾**。

这些结论要拿去和每月真在对账的人讨论，一个经不起追问的数字比没有数字更糟。

在做的：新能源和储能的结算与分成复核——把市场规则和结算条款写成可以重算的程序，
核对账单里每一项。这部分不公开。
