# 终结阿尔茨海默 · 健脑方案（recode-brain-health）

> 把戴尔·布来得森《终结阿尔茨海默病》（The End of Alzheimer's）的 ReCODE/PreCODE 方法论，
> 蒸馏成 AI Agent 可直接调用的 **11 张能力卡**。面向 50+ 人群与家属的护脑自测、化验解读、
> 个性化行动方案与科普助手。

![Version](https://img.shields.io/badge/version-1.0.2-green) ![License](https://img.shields.io/badge/license-MIT-blue) ![Platform](https://img.shields.io/badge/platform-Coze%20%7C%20OpenClaw%20%7C%20Claude%20Code-informational)

---

## ✨ 它能做什么

| 能力卡 | 解决什么问题 |
| --- | --- |
| 01 早期信号与认知自测 | 总担心记性差？对照 10 大警示信号初判阶段 |
| 02 认知体检与指标解读 | 化验单看不懂？血糖/维D/B12/同型半胱氨酸该查什么、目标值多少 |
| 03 三型分型与驱动因素 | 炎症型 / 萎缩型 / 毒素型，同样是遗忘，路不同 |
| 04 KetoFLEX 饮食法 | 温和生酮 12/3 怎么吃、必吃清单与避免清单 |
| 05 运动健脑处方 | 有氧 + 力量 + 平衡的具体剂量与进阶 |
| 06 睡眠与大脑清洗 | 深睡修复、睡眠呼吸暂停排查（头号可纠正杀手） |
| 07 压力管理与社交意义 | 慢呼吸、孤独感、退休后的意义感重建 |
| 08 脑刺激与认知储备 | 学新技能 ≠ 刷短视频，有难度有反馈能进阶的训练 |
| 09 毒素规避与排毒 | 霉菌/重金属/口腔肠道的暴露排查与移除 |
| 10 营养与靶向补充 | 先体检找缺乏，再针对性补（维D、B12、Omega-3），不盲补 |
| 11 个性化方案与复查迭代 | 多靶点个性化方案 + 3–6 个月复查闭环 |

**特点**：评估优先于建议 · 先找洞再修补 · 医疗边界清晰（附就医红旗提示）。

## 🧑‍⚕️ 适合谁用

- 关注大脑健康的 **50+ 中老年**及其**子女家属**（"我妈老忘事该查什么"）
- 健康科普 / 银发内容**创作者**（选题、图文脚本的知识底座）
- 希望给 AI Agent 装上"健脑顾问"能力的**个人与企业**

## 📦 安装

### 方式一：CocoLoop（国内 OpenClaw 用户推荐）
在 [CocoLoop Skill 商店](https://hub.cocoloop.cn/) 搜索 `recode-brain-health` 或"健脑"，一键安装。

### 方式二：虾评（Coze Agent 用户）
在 [虾评](https://xiaping.coze.com/) 搜索技能名安装，或直接使用分享链接。

### 方式三：扣子 Coze（技能上传）
扣子 → 对话页 "+" → 技能 → 上传技能 zip → 选择本仓库 Release 中的
`recode-brain-health_v1.0.2_分享包.zip`。

### 方式四：Claude Code / OpenClaw / Codex（手动安装）
```bash
# 克隆仓库
git clone https://github.com/amydeng2020-sketch/recode-brain-health.git

# 复制到技能目录（按你的平台选择其一）
# Claude Code / Codex 全局
cp -r recode-brain-health ~/.claude/skills/
# OpenClaw / Molili
cp -r recode-brain-health ~/.openclaw/skills/
# 项目级（Codex 推荐）
cp -r recode-brain-health .agents/skills/
```

## 💬 使用示例

```
「我妈最近老忘事，该先做什么检查？」
「听说 KetoFLEX 12/3，具体怎么吃？」
「体检发现维生素D 只有 18，怎么办？」
「帮我出一份 30 天健脑行动清单」
「写一篇'睡眠是大脑的夜班保洁'的科普选题」
```

## 📁 目录结构

```
recode-brain-health/
├── SKILL.md                  # 能力入口与路由表（先读我）
└── references/
    ├── overview.md           # 方法论总览
    ├── cheatsheet.md         # 速查表
    ├── glossary.md           # 术语表
    └── capabilities/         # 11 张能力卡（按用户问题路由加载）
        ├── 01-早期信号与认知自测.md
        ├── ...
        └── 11-个性化方案与复查迭代.md
```

## 🧠 方法论来源与免责声明

- 本技能是对 **Dale E. Bredesen, M.D.**《The End of Alzheimer's》方法论的学习性
  提炼与原创整理，**不包含原书文本**；方法论版权归原书作者与出版方所有。
- ⚠️ **本技能仅供健康科普与生活方式参考，不构成医疗建议、诊断或处方。**
  认知症状明显、指标显著异常或已确诊者，请务必在神经内科 / 记忆门诊医生指导下诊疗；
  停药、换药、激素替代与高剂量补充剂必须先经医生评估。

## 📄 License

[MIT](./LICENSE) © 2026 amydeng2020-sketch (HAO18)

## 🕐 版本历史

| 版本 | 日期 | 说明 |
| --- | --- | --- |
| v1.0.2 | 2026-09-19 | 能力入口触发词优化，医疗边界与免责声明强化 |
| v1.0.0 | 2026-09-13 | 首发：11 张能力卡 + 总览 + 速查表 + 术语表（仓颉方法论 v2.5 蒸馏） |
