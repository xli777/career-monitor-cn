# Career Monitor CN — Public Beta

Career Monitor CN 是面向中国互联网 **产品 / 运营 / 营销等非技术岗位** 的 AI 辅助岗位监测与学习 Skill，覆盖应届与社招场景。

> 当前版本：`0.1.0-rc.4`  
> 发布状态：**Public Beta / Experimental**  
> 发布者：**@杰克 On The Road**

## 当前能做什么

- 按公司官网优先、第三方补充的方式组织岗位监测；
- 区分岗位事实、渠道发现、访问失败、关闭/重开/变化状态；
- 对重复岗位与镜像岗位做去重与状态归并；
- 在没有简历时仍可执行 M0 市场探索，未知信息显式标记 `UNKNOWN`；
- 从候选人反馈形成 Observation → Hypothesis → Trial → Approved Rule / Rollback 的学习链；
- 将候选人运行状态保存在候选人自己的 Google Drive 或飞书工作区，而不是上传到 GitHub。

## Public Beta 验证状态

| 层级 | 状态 |
|---|---|
| Package / Schema / anti-drift | ✅ PASS |
| Channel Pack + Ground Truth v0.2 | ✅ PASS |
| Monitoring / Learning / Recovery regression | ✅ PASS |
| RC4 T0 package validation | ✅ PASS |
| OpenAI T1–T8 | 🧪 Public Beta validation |
| Claude T1–T8 | 🧪 Public Beta validation |
| Doubao + Feishu T1–T8 | 🧪 Public Beta validation |
| T9 cross-platform semantic parity | 🧪 Pending runtime evidence |

Public Beta 的目的就是让作者和真实候选人共同完成三端实际安装验证。未完成的能力必须按 `TEST_REQUIRED / Experimental` 理解，而不是稳定承诺。

## 下载

**正式 ZIP 下载将通过 GitHub Release `v0.1.0-rc.4` 提供。** 当前仓库已经发布三端安装说明、SHA-256 和飞书单文件 Skill；四个 ZIP Release assets 仍需在 GitHub Release 页面完成一次手工上传。

计划中的 Release assets：

- OpenAI：`career-monitor-openai-plugin-0.1.0-rc.4.zip`
- Claude：`career-monitor-claude-0.1.0-rc.4.zip`
- 豆包 + 飞书：`career-monitor-doubao-feishu-0.1.0-rc.4.zip`
- Core：`career-monitor-core-0.1.0-rc.4.zip`

已可直接查看/下载：

- 飞书单文件 Skill：[`career-monitor-doubao-feishu-0.1.0-rc.4-SKILL.md`](./downloads/0.1.0-rc.4/career-monitor-doubao-feishu-0.1.0-rc.4-SKILL.md)
- SHA-256：[`checksums.txt`](./checksums.txt)

## 三端安装

- [OpenAI](./install/openai.md)
- [Claude](./install/claude.md)
- [豆包 + 飞书](./install/doubao-feishu.md)

## 推荐第一次使用

> 开始中国互联网产品、运营、营销岗位的 M0 市场探索。没有简历也继续，未知项标记 UNKNOWN。

简历、项目经历、Candidate Profile、Evidence Ledger、Resume Master 缺失都不能阻断 M0。

## 安全与边界

Career Monitor CN 不会：

- 自动投递；
- 自动联系 HR；
- 自动向作者发送报告；
- 保存密码、Cookie 或验证码；
- 绕过 CAPTCHA / 风控 / 反自动化限制；
- 把访问失败解释成“没有岗位”。

详见 [Privacy](./PRIVACY.md) 与 [Known Limitations](./KNOWN_LIMITATIONS.md)。

## 反馈

优先使用本仓库 GitHub Issues 报告：安装失败、授权异常、重复岗位、关闭岗位误报、渠道失败、跨端语义差异等。

**不要在公开 Issue 上传简历、手机号、邮箱、身份证明、密码、Cookie、Token 或完整候选人运行数据库。**

公开支持身份：**@杰克 On The Road**。当前不提供公开产品邮箱。

## 版本策略

`0.1.0-rc.x` = Public Beta / Release Candidate。发现问题后在私有研发仓库修复、全量回归，再发布新的 RC。

Stable `v0.1.0` 才要求 OpenAI / Claude / 豆包+飞书三端 T1–T9、关键语义一致性以及最终 Go/No-Go 通过。
