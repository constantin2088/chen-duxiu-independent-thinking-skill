# 陈独秀·让主张接受科学检验

让主张接受科学检验：有资料依据、有使用边界、可复核的中文 Agent Skill。

**把熟悉的思想，变成下一次任务可用的方法。**

适合：观点来自权威或习惯、需要检查自主判断与实际用途。

交付：写正在接受的主张与实际问题 → 区分权威声望、传统习惯和可检验依据 → 核主张改善谁的生活、忽略什么代价 → 写可反驳的条件 → 允许独立提出不同方案 → 交付证据审查与可执行改进。

**一分钟看懂**：主管仅凭名人推荐采购高价软件。

本 Skill 会这样处理：核具体任务、试用表现和总成本；权威意见作线索，不替代适用性证据。

[用途与同类差异](references/positioning.md)。人物知名度提供发现入口，实际价值来自工作流与可复核产物；不保证星标增长。

## 安装与使用
公开仓库直接提供 Skill，不依赖 GitHub Release。
```sh
npx skills add constantin2088/chen-duxiu-independent-thinking-skill
```
也可将仓库内容复制到支持该格式的客户端 Skill 目录，保留以 `chen-duxiu-independent-thinking-skill` 命名的文件夹和根目录 SKILL.md。客户端支持范围以其文档为准。安装后提出具体任务，由客户端按描述加载。

**试用任务**：主管仅凭名人推荐采购高价软件。

## 内容
- [执行说明](SKILL.md)
- [资料卡](references/sources.md)、[工作表](references/frameworks.md)、[边界](references/boundaries.md)
- [三个示例](examples/demo.md)、[十个行为评测场景](evals/test-cases.md)

## 验证与贡献
```sh
python scripts/check_skill.py . --release
python -m unittest discover -s tests -v
python scripts/check_links.py
```
`--release` 是完整性检查参数，不创建 GitHub Release。CI 在每次提交运行上述检查。独立客户端模型行为评测尚未执行；用例、结构检查与实际模型能力分开报告。
修改时提供来源和定位，区分原文与转译；运行检查后直接提交到仓库。不要创建发布附件作为必需安装步骤。系列标识、链接和推荐由总仓库 catalog/skills.json 同步，避免手工修改受管理区块。

## 许可
项目原创内容使用 [MIT](LICENSE)。链接所指第三方作品保留原权利，本仓库不重新许可它们。
