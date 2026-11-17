# crafting-coherent-deliverables

用于演讲稿、幻灯片、报告和提案的 Agent Skill。适合一个简报里出现多个主题、草稿转折生硬，或重要结论找不到依据的时候。

它用三道检查帮助成稿经得起受众阅读。先用删除与替换测试判断主题为什么要放在一起。写作前提出足以推翻提纲的反对意见。成稿后只看作品和原始要求，重新检查过渡、证据及硬性指标。

## 安装

### Codex

需要 Git。在项目根目录运行以下命令。跨项目使用时，可将目标放在 `~/.agents/skills/crafting-coherent-deliverables`。安装后打开新的 Codex 会话。

```sh
git clone --branch v1.3 https://github.com/lh0314/crafting-coherent-deliverables.git .agents/skills/crafting-coherent-deliverables
```

路径与安装方式见 [OpenAI 官方文档](https://developers.openai.com/api/reference/cli#use-the-cli-from-a-coding-agent)。

### 其他 AI 环境

支持 [Agent Skills](https://agentskills.io/specification) 的环境可按平台说明导入整个 `crafting-coherent-deliverables` 目录，保留其中的 `SKILL.md` 和相对路径。有些平台提供技能目录，有些要求上传技能包。

普通对话也可以附上 [SKILL.md](SKILL.md)，在同一条消息里提供原始要求和材料，并请模型按文件里的方法制作或审查。核心流程可直接从该文件读取。

## 使用

> 请用 crafting-coherent-deliverables 写一篇展览开幕致辞。观众是初次参观的社区居民。开幕恰逢机构周年，主要目的是邀请居民提交街区口述史线索。只用我附上的素材，400 字以内，直接给稿。

在支持显式调用的 Codex 会话中也可用 `$crafting-coherent-deliverables`。语气、个人素材、材料范围和引用方式可以直接写进任务要求。编辑现有作品时，可加上需要保留的段落或文件元素。

## 文件与案例

- [SKILL.md](SKILL.md) 包含完整工作流程。
- [演讲正反例](examples/anniversary-speech.md) 展示如何处理周年场合与活动目标。
- [提案正反例](examples/pilot-proposal.md) 展示证据如何支撑一次有限的试行。
- [CHANGELOG.md](CHANGELOG.md) 记录公开版变动。

## 验证状态

v1.3 已检查 YAML、目录名和相对链接，并在一个模拟写作任务中用显式读取的方式做了模型对照。文档中的安装方式按所引平台文档编写。各平台的安装、自动触发、更多写作场景和文件操作仍待逐项验证。
