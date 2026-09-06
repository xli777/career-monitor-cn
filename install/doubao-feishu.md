# 豆包 + 飞书 — RC4 安装 / Beta 测试

优先测试当前账号实际可见的 Skill-native 入口，不预设旧产品名称。

建议顺序：

1. **飞书多维表格智能体**：当前最贴合 Career Monitor 的五表状态模型；官方支持通过上传或对话创建 Skill。
2. **飞书 aily SkillHub / 豆包工作相关 Skill 入口**：如账号可用，则上传 RC4 Skill 并记录真实 surface。
3. **Aily Agent / Workflow wrapper**：仅作为前两者不能满足时的 Adapter fallback，不得修改 Core 业务语义。

状态映射：

- 00_README → 飞书文档
- 01_Search Charter → 飞书文档
- 02_Monitoring DB → 多维表格：Sources / Jobs / Rules / Events / Channel Gaps
- 03_Reports → 云空间目录
- 04_Candidate Inputs → 云空间目录
- 05_Support Exports → 云空间目录

测试必须记录具体产品 surface、租户/版本能力、授权范围、初始化两次是否重复、跨会话状态与撤权行为。
