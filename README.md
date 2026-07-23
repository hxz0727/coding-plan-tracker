# AI Coding Plan & Token Plan 动态追踪

> 跟踪主流 AI 编程工具（Coding Plan）与按 Token 计费方案（Token Plan）的最新动态、厂商套餐、价格与订阅方式。
> **最新更新：2026-07-23** ｜ 更新频率：每周一、四 09:05（自动化）
> 数据来源：各厂商官方定价页 / 官方博客 + 第三方价格追踪（截至 2026-07 交叉验证）

---

## 一、最新动态（2026 年 7 月）

- **编程模型价格战（7/8–7/9）**：OpenAI 发布 **GPT-5.6**（Sol / Terra / Luna 三档）、xAI 发布 **Grok 4.5**、Meta 发布 **Muse Spark 1.1**，同周集中亮相，前沿模型输出单价被压到 \$4–6 / 百万 token，价格与 Token 效率同时成为竞争焦点。
- **SpaceX(xAI) 收购 Cursor**（约 2026 年 6 月，估值约 600 亿美元）：Grok 4.5 由 xAI 与 Cursor 联合训练，直接嵌入 Cursor 开发环境。
- **GitHub Copilot 全面转向 Token 计费**：6/1 起用 **GitHub AI Credits**（1 credit = \$0.01，按输入/输出/缓存 token 计费）替代原来的 Premium Request Units；6/15 新增 **Max \$100/月** 档；Business / Enterprise 在 6–9 月享促销额度。
- **Cursor Teams 拆分**：7/1 起续费客户生效，Teams 拆分为 **Standard \$40/用户/月** 与 **Premium \$120/用户/月（5× 用量）**；并区分自有模型（Auto）与第三方模型用量池。
- **Windsurf 重塑为 Devin Desktop**：6/2 起由 Cognition AI 更名，Cascade 智能体弃用、改为 **Devin Local**；套餐/扩展延续。
- **Anthropic Fable 5 退出订阅档**：6/22 起从 claude.ai Pro / Max 移除，转为付费 API（\$10 输入 / \$50 输出 per MTok，为 Opus 4.8 的两倍）。
- **OpenAI Codex 与 GPT-5.6 整合**：4/2 起 Codex 改为 API token 计费；7 月打通 ChatGPT / Codex / API，周活用户超 500 万（其中 100 万+ 用于编程以外）。
- **GitHub Code Quality 正式商用（7/20）**：按活跃提交者 \$10/月 + AI 能力用量计费。

---

## 二、厂商套餐、价格与订阅详情

> 价格均为美元（USD）/ 月，除非特别注明。套餐名称与额度以官方页面为准，第三方来源存在差异处已标注。

### 1. Cursor（Anysphere，已被 xAI/SpaceX 收购）
| 套餐 | 价格 | 包含用量 / 说明 | 可订阅 |
|---|---|---|---|
| Hobby | \$0 | 有限 Agent 请求 + Tab 补全，无需信用卡 | ✅ 免费 |
| Pro | \$20/月 | ~\$20 API 用量、无限 Tab、Auto/Chat/Agent、Background Agents | ✅ |
| Pro+ | \$60/月 | ~\$70 API 用量（Pro 的 3×） | ✅ |
| Ultra | \$200/月 | ~\$400 API 用量（20×）、优先体验新模型 | ✅ |
| Teams Standard | \$40/用户/月 | 集中计费、团队市场、SSO、用量分析 | ✅ |
| Teams Premium | \$120/用户/月 | Standard 的 5× 用量（7/1 起对续费客户生效） | ✅ |
| Enterprise | 定制 | 共享用量、SCIM、审计日志、发票 | ✅ 联系销售 |

- 计费逻辑：**Auto 模式无限额、不耗 credit**；手动选高级模型 / Max 模式才消耗 credit 池。
- Teams 中非 Auto 智能体请求额外收 **\$0.25 / 百万 token** 的 Cursor Token 费率。
- 年付 Pro 约 \$16/月（\$192/年）。

### 2. Claude Code（Anthropic）
> Claude Code 不单独售卖，通过 Claude 订阅或 API 计费。
| 套餐 | 价格 | Claude Code 用量 | 可订阅 |
|---|---|---|---|
| Free | \$0 | ❌ 不含（仅聊天） | ✅ 聊天 |
| Pro | \$20/月（年付 \$17） | ~44K token / 5h 滚动窗口，Sonnet 4.6 + Opus 4.7 | ✅ |
| Max 5× | \$100/月 | Pro 的 5× 容量 | ✅ |
| Max 20× | \$200/月 | Pro 的 20× 容量 | ✅ |
| Team Standard | \$25/席/月（年付 \$20） | 1.25× Pro，含管理控制 | ✅ |
| Team Premium | \$125/席/月（年付 \$100） | 6.25× Pro，SSO/优先级 | ✅ |
| Enterprise | \$20/席 + API 用量 | SCIM、审计、HIPAA | ✅ 联系销售 |
| API（按 token） | 按量 | Haiku 4.5 \$1/\$5、Sonnet 4.6 \$3/\$15、Opus 4.7/4.8 \$5/\$25（每 MTok） | ✅ |

- 4 月曾短暂将 Claude Code 从 Pro 挡到 Max 后迅速回滚；Fable 5 已于 6/22 转为付费 API。

### 3. GitHub Copilot（Microsoft）
> 6/1 起全面改用 **GitHub AI Credits**（1 credit = \$0.01），按 token 消耗计费；补全与 Next Edit 建议仍无限且不计费。
| 套餐 | 价格 | 包含 AI Credits | 可订阅 |
|---|---|---|---|
| Free | \$0 | 2,000 补全 + 50 次聊天/月 | ✅ |
| Pro | \$10/月 | 1,500 credits（≈\$15） | ✅ |
| Pro+ | \$39/月 | 7,000 credits（≈\$70） | ✅ |
| Max | \$100/月（6/15 新增） | 20,000 credits（≈\$200） | ✅ |
| Business | \$19/用户/月 | 1,900/用户（促销 3,000，至 9 月） | ✅ |
| Enterprise | \$39/用户/月 | 3,900/用户（促销 7,000，至 9 月） | ✅ |

- 超出后按模型 API 单价计费（如 GPT-5.5 \$5/\$30、Claude Opus 4.7 \$5/\$25、Gemini 3.1 Pro \$2/\$12 per MTok）。
- 企业版已上线自研 **MAI-Code-1-Flash** 模型（快速、低成本、数据不出微软栈）。
- 新用户 Pro/Pro+ 自注册曾暂停（可靠性措施），用量稳定后放宽。

### 4. OpenAI Codex（内置 ChatGPT）
> 无独立订阅，随 ChatGPT 套餐提供；4/2 起改为 API token 计费（输入/缓存输入/输出）。
| 套餐 | 价格 | Codex 用量 | 可订阅 |
|---|---|---|---|
| Free | \$0 | 有限试用 | ✅ |
| Go | \$8/月 | 轻量编程 | ✅ |
| Plus | \$20/月 | 慷慨额度（CLI/IDE/Web/云任务/自动评审） | ✅ |
| Pro 5× | \$100/月 | Plus 的 5× | ✅ |
| Pro 20× | \$200/月 | Plus 的 20× | ✅ |
| Business | \$20–25/用户/月 | 团队管理、更高额度 | ✅ |
| Enterprise | 定制 | SSO/SCIM/审计 | ✅ 联系销售 |
| API Key | 按量 | 仅按 token 付费（CLI/SDK/IDE，无云端特性） | ✅ |

- Token Rate Card（credit / 百万 token）：GPT-5.5 输入 125 / 缓存 12.5 / 输出 750；GPT-5.4 62.5 / 6.25 / 375；GPT-5.4-mini 18.75 / 1.875 / 113。
- 重度用户实际约 \$100–200/开发者/月（取决于模型、并发、Fast 模式）。

### 5. Windsurf → Devin Desktop（Cognition）
> 6/2 更名；Cascade → Devin Local。计费历经多次调整（3 月改为日/周配额）。
| 套餐 | 价格 | 说明 | 可订阅 |
|---|---|---|---|
| Free | \$0 | 无限 Tab 补全 + 25 credits/月 | ✅ |
| Pro | ~\$15–20/月 | 500 credits/月 + 日/周配额 | ✅ |
| Max | \$200/月 | 最高配额、无中断 | ✅ |
| Teams | ~\$40/用户/月 | 管理控制（来源间有差异，另有 \$80 基础 + \$40/席 之说） | ✅ |
| Enterprise | ~\$60/用户/月 | SOC2 / HIPAA / FedRAMP | ✅ 联系销售 |

- 仅 Cascade/Devin Local、Command、高级模型聊天消耗 credits；Tab 补全永远免费无限。

### 6. Trae（字节跳动）
> 2/24 起全面改为 **Token 制** 套餐（Basic Usage + Bonus Usage，超额可开 On-Demand 按 API 计费）。
| 套餐 | 连续包月 | Basic Usage/月 | 云端并行数 | 可订阅 |
|---|---|---|---|---|
| Free | \$0 | —（按 token 计费） | 2 | ✅ |
| Lite | \$3/月 | \$5 | 2 | ✅ |
| Pro | \$10/月 | \$20 | 10 | ✅（新用户 7 天试用） |
| Pro+ | \$30/月 | \$90 | 15 | ✅ |
| Ultra | \$100/月 | \$400 | 20 | ✅ |

- 同类中价格最激进（Lite \$3 远低于竞品）；支持 SOLO 多智能体并行；年付约省 25%。

### 7. Gemini Code Assist（Google）
| 套餐 | 价格 | 说明 | 可订阅 |
|---|---|---|---|
| Free（个人） | \$0 | 18 万补全/月、240 聊天/天、VS Code/JetBrains | ✅ |
| Standard | \$19/用户/月（年付）/ \$22.80（月付） | 更高配额、企业安全、IP 赔偿 | ✅ |
| Enterprise | \$45/用户/月（年付）/ \$54（月付） | 私有仓库感知、Google Cloud 接地、定制 | ✅ |

### 8. 其他值得关注
| 工具 | 价格模式 | 计费方式 | 可订阅 |
|---|---|---|---|
| Aider | 开源 | BYOK（API 按量），约 \$60–80/月重度 | ✅ 免费工具 |
| Cline | 开源 | BYOK（API 按量），约 \$50–100/月重度 | ✅ 免费工具 |
| Continue.dev | 开源 | BYOK | ✅ 免费工具 |
| Tabnine | \$12/月起 | 固定订阅 | ✅ |
| Zed | \$10/月 | 固定订阅 | ✅ |
| Amazon Q Developer | \$19/用户/月 | 固定（无 credit 套路） | ✅ |
| JetBrains AI | \$10 / \$30/月 | 固定订阅 | ✅ |
| Augment Code | \$100/月（≤50 席 固定） | 固定 | ✅ |
| Devin（Cognition） | \$20 平台费 + \$2.25/ACU | 按 Agent Compute Unit 付费 | ✅ |

---

## 三、编程模型 Token 价格（价格战全景，\$/百万 token，输入/输出）

| 模型 | 输入 | 输出 | 备注 |
|---|---|---|---|
| **Meta Muse Spark 1.1** | \$1.25 | \$4.25 | 7/9 发布，1M 上下文，US 预览/候补，Meta 首个付费模型 |
| **GPT-5.6 Luna** | \$1.00 | \$6.00 | 7/9，最快最便宜档 |
| **xAI Grok 4.5** | \$2.00 | \$6.00 | 7/8，500K 上下文，Cursor 数据训练 |
| **Gemini 3.1 Pro** | \$2.00 | \$12.00 | Google |
| **GPT-5.6 Terra** | \$2.50 | \$15.00 | 7/9，均衡档 |
| **Claude Sonnet 4.6** | \$3.00 | \$15.00 | Anthropic |
| **Claude Haiku 4.5** | \$1.00 | \$5.00 | 轻量 |
| **GPT-5.6 Sol** | \$5.00 | \$30.00 | 7/9，旗舰 |
| **Claude Opus 4.8** | \$5.00 | \$25.00 | Anthropic 旗舰 |
| **Anthropic Fable 5（API）** | \$10.00 | \$50.00 | 6/22 起退出订阅档，转为付费 API |

**关键结论**：输出 token 主导账单（模型要写代码、跑工具、叙述推理）；同一厂商内部价差可达 5×（如 GPT-5.6 Luna \$6 vs Sol \$30）。选错档位比选错厂商更贵。

---

## 四、是否可订阅 / 免费试用 一览

| 厂商 | 免费档 | 新用户试用 | 信用卡门槛 | 订阅方式 |
|---|---|---|---|---|
| Cursor | ✅ Hobby | Pro 一周试用 | 否（Hobby） | 官网直售（无授权经销商） |
| Claude Code | ❌（Free 不含） | — | 付费起 \$20 | claude.ai / API |
| GitHub Copilot | ✅ Free | — | 否 | github.com / 企业协议 |
| OpenAI Codex | ✅（限 Free/Go） | — | 否 | ChatGPT 套餐内含 |
| Windsurf/Devin | ✅ Free | — | 否 | 官网 |
| Trae | ✅ Free | Pro 7 天（绑卡） | 试用需卡 | 官网/IDE |
| Gemini Code Assist | ✅ 个人 | Standard/Enterprise 30 天（≤50 人） | 否 | Google Cloud / 插件 |

---

## 五、趋势总结与建议

1. **计费范式迁移完成**：从"按请求数"全面转向"按 Token / Credit 计费"。Copilot（AI Credits）、Cursor（credit + 用量倍数）、Codex（API token）、Trae（Token 套餐）殊途同归。
2. **订阅价只是起点**：重度用户的真实月支出常是标价的 2–10×（超额、Fast 模式、并行 Agent）。务必看"真实成本"而非"挂牌价"。
3. **模型路由 = 省钱关键**：同一工具内选便宜模型（如 Luna / Haiku / 自有模型）可省数倍；把重活留给 Opus/Sol，日常用轻量模型。
4. **厂商自研模型降本**：Microsoft MAI-Code-1-Flash、Cursor Auto、Trae 自有模型都在把高频 Agent 流量留在低成本通道。
5. **价格战利好用户**：7 月三款新模型把前沿输出价压到 \$4–6/MTok，长期看单位智能成本持续下降。
6. **选型建议**：个人轻度 → Copilot Free / Trae Free；日常主力 → Cursor Pro \$20 或 Copilot Pro \$10；重度 Agent → Cursor Ultra \$200 / Claude Max 20× \$200 / Codex Pro 20× \$200；团队 → 按 IDE 栈与合规选 Copilot Business / Cursor Teams / Gemini Enterprise。

---

*本文件为最新版，默认在仓库首页展示；历史版本见 `history/YYYY-MM-DD.md`。*
