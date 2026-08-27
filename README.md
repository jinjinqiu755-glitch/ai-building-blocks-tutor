# AI Building Blocks Tutor

一个面向 AI 产品经理、产品运营和非算法岗位的 Codex Skill。

它使用知识地图、自适应讲解、检索练习、迁移题和持续学习档案，帮助学习者形成能够独立调用的 AI 技术框架，而不只是记住术语。

## 主要特点

- 6 个学习阶段、41 个 AI 产品技术 Building Blocks。
- 根据知识类型选择系统拆解、机制讲解、最小实验、工程计算或方案判断。
- 一次只推进一个 Block，避免课程边界不断漂移。
- 用无提示复述和新情境迁移判断是否真正掌握。
- 自动维护 Markdown 学习档案，记录校准后的答案和掌握证据。
- 不依赖 MCP、API Key、第三方服务或额外脚本。

## 安装

### 通过 Git 克隆

将仓库克隆到 Codex 的 skills 目录：

~~~bash
git clone https://github.com/jinjinqiu755-glitch/ai-building-blocks-tutor.git ~/.codex/skills/ai-building-blocks-tutor
~~~

Windows：

~~~powershell
git clone https://github.com/jinjinqiu755-glitch/ai-building-blocks-tutor.git "$env:USERPROFILE\.codex\skills\ai-building-blocks-tutor"
~~~

### 下载 ZIP

1. 下载并解压仓库。
2. 将整个 ai-building-blocks-tutor 文件夹放入 ~/.codex/skills/。
3. 确认 ~/.codex/skills/ai-building-blocks-tutor/SKILL.md 存在。
4. 新建一个 Codex 任务。

## 使用

显式调用：

~~~text
$ai-building-blocks-tutor 我是 AI 产品经理，请诊断我的技术基础，并开始第一个适合我的 Building Block。
~~~

也可以直接提出自然语言请求：

~~~text
我想系统补齐 AI 产品技术知识，从我当前的水平开始教。
继续上次的 AI 学习。
检查我是否真的掌握了 RAG。
今天只学习 Token，不需要展开后面的主题。
~~~

## 默认知识地图

1. 看懂 AI 产品
2. 看懂模型
3. 看懂训练
4. 看懂知识与工具
5. 看懂工程与成本
6. 做出产品判断

知识地图是默认路线，不是强制课程。Skill 会根据岗位、已有基础和实际工作问题调整起点、顺序和深度。

## 工作方式

每个 Block 会经历：

~~~text
确定学习边界
→ 建立定义与机制
→ 区分相邻概念
→ 观察实验或分析案例
→ 闭卷复述
→ 新场景迁移
→ 判定掌握层级
→ 更新学习档案
~~~

掌握层级分为：未开始、跟随理解、框架复述、独立应用、诊断与设计。

## 仓库结构

~~~text
ai-building-blocks-tutor/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── curriculum.md
│   ├── teaching-modes.md
│   └── mastery-and-record.md
└── assets/
    └── learning-record-template.md
~~~

## 信息时效

模型规格、API、价格和许可证可能变化。Skill 要求在教授这些内容时优先核验官方一手资料并记录核验日期；无法核验时，只讲稳定机制并明确不确定部分。

## License

MIT

---

## English Quick Start

AI Building Blocks Tutor is a Codex Skill for learning practical AI product technology through adaptive explanations, retrieval practice, transfer exercises, and a persistent learning record.

Install the repository under ~/.codex/skills/ai-building-blocks-tutor, open a new Codex task, and invoke:

~~~text
$ai-building-blocks-tutor Assess my current AI product knowledge and start the next suitable learning block.
~~~
