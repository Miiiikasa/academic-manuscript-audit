# academic-manuscript-audit · v3.1.2

面向不同期刊、文章类型和投稿阶段的只读投稿前审查。根据每次核对的官方指南建立适用规则，并把文件证据、合规结论和作者需确认的事项分开记录。切换期刊时只需更换调用参数和本地材料。

## 安装与兼容

将整个目录安装到 Skills 发现目录，保持文件夹名 `academic-manuscript-audit`。Codex 可使用 `~/.agents/skills/`，或按客户端配置使用 `~/.codex/skills/`。新会话中使用 `$academic-manuscript-audit`，也可在当前会话提供 SKILL.md 路径。

从 [GitHub 公共仓库](https://github.com/Miiiikasa/academic-manuscript-audit) 安装。首次克隆时目标目录应尚不存在。

```powershell
git clone https://github.com/Miiiikasa/academic-manuscript-audit.git "$env:USERPROFILE/.agents/skills/academic-manuscript-audit"
```

已通过 Git 安装时，更新到当前 `main`：

```powershell
git -C "$env:USERPROFILE/.agents/skills/academic-manuscript-audit" pull --ff-only
```

Skill 可独立运行。查看 PDF、图件渲染及外部核验取决于执行环境可用的工具和权限。可复用稿件旁的 `academic-audit.local.md`。审查先核对当前期刊要求，再使用其中的本地约定。真实项目配置、指南副本和报告留在项目目录。

## 调用

两种基础审查模式为完整审查和专项审查。复审或返修可按任一范围执行。近期论文对照可单独运行，也可附加在完整审查中。

**模式 A · 完整投稿前审查**

> 使用 $academic-manuscript-audit 做完整投稿前审查。目标期刊为〈期刊全称〉，文章类型为〈期刊采用的类别〉，现在是首次投稿。我已下载作者指南，路径为〈本地指南〉。投稿包在〈文件夹〉。请扫描后与我确认哪些文件属于本次提交。

完整审查会主动在对话中询问缺失信息，等你回复后再做依赖该答案的检查。如果只给出文件夹，Skill 会先展示候选文件、数量和角色，再请你确认本次投稿范围。你也可以在调用时直接给出已确认的文件清单。只有访问不全或扫描结果冲突时才追问数量。没有本地指南时可以直接指定查官网。近期论文对照只询问一次，未回答也可以继续。

**模式 B · 专项审查**

> 使用 $academic-manuscript-audit，只检查〈文件〉中的图表、缩写和交叉引用。按通用规范审查，记录无法核验的图内标签。

也可只审查参考文献、匿名性、补充材料、排版、语言或全文论证。若专项涉及期刊强制要求，请提供期刊和适用的文章类型。完整、专项和复审（包括按返修阶段核对的审查）均生成 Checklist 和问题报告，注明实际审查范围。独立运行近期论文对照时，只生成对照报告。

**复审与返修**

> 使用 $academic-manuscript-audit 对〈当前返修目录〉做第二轮审查。上一轮报告在〈目录〉。按该期刊返修要求核对 clean、marked 和逐点回复。只报告新增、变化和仍未解决的问题。

复审与返修可以分别调用。返修文件要求以本轮期刊指示为依据。

**近期论文对照**

> 使用 $academic-manuscript-audit 做近期论文对照。目标期刊为〈全称〉，文章类型为〈类型〉。同类近期论文 PDF 在〈目录〉。请逐项统计并对照〈用户稿〉。

可独立运行，也可随完整审查运行。约十篇只是建议，样本数不限。没有样本可以照常审查投稿包。发表后的常见做法只支持可选建议。

- [Submission Checklist 模板](templates/Submission%20Checklist.md) · [完整审查示例（节选）](examples/Submission%20Checklist.md)
- [Issues and Recommendations 模板](templates/Issues%20and%20Recommendations.md) · [完整审查示例（节选）](examples/Issues%20and%20Recommendations.md)
- [专项 Checklist 示例（节选）](examples/targeted/Submission%20Checklist.md) · [专项问题报告示例（节选）](examples/targeted/Issues%20and%20Recommendations.md)
- [Recent_Publications_Benchmark 模板](templates/Recent_Publications_Benchmark.md) · [五篇样本示例（节选）](examples/Recent_Publications_Benchmark.md)

报告默认写入投稿包旁的 `Pre-submission_Audit` 内的新运行目录，也可指定其他目录。

## 模拟验证

以下为规则走查，期刊要求和材料均为虚构。

| 模拟调用 | 应有处理 |
|---|---|
| 完整模式，Research Article 首投，期刊与包清单已确认 | 采用现行首投允许嵌图的条款。旧指南的独立图件要求在首投不适用。缺少明确要求的 Title Page 记 P0。作者贡献声明已存在与实际贡献待确认分别记录 |
| 完整模式，Review，已知期刊和目录，已下载指南但缺路径，存在两个候选稿 | 展示候选文件，在对话中询问指南路径、稿件版本和文件范围，并等待回复。确认后按 Review 条款审查 |
| 专项模式，只检查图表与缩写，部分内嵌图标签无法读清 | 可读图按已声明的标准代码约定审查。图文术语不一致时同时记录两处并等待作者确认。不可读部分记无法检查，两份报告仅覆盖本专项 |
| 复审兼返修，clean 已修正旧问题，marked 尚未准备，response 有一处定位变化 | 若明确要求 marked 且确定未准备，记未通过。只列新增缺件、已变化的回复问题及旧的未解决问题 |
| 投稿范围已确认，必需文件尚未准备，另有已存在但打不开的文件 | 可出临时报告。当前必需且确认缺失记未通过，打不开的内容记无法检查。范围尚未确认时，只有用户要求才先出限定范围的临时报告 |
| 五篇论文对照，含不可读 PDF 和无法取得的 SI | 条件式声明先核对条件，再按出现与核验未见计算分母。声明是否出现与代码共享政策是否满足分别判断。旧版指南和发表排版均不覆盖现行投稿规则 |

## 范围与人工核验

规则随期刊、文章类型和投稿阶段变化。投稿系统设置、伦理和许可真实性、实际作者贡献、真实 AI 使用、受限数据的实际访问和结果能否复现，可能需要作者确认、授权访问或单独执行验证。报告会标明能够从文件检查的部分、仍缺的证据和责任方。审查只读，修改与投稿分别由用户另行决定。

AI 使用台账和登录系统确认可作为取证办法，只有适用政策要求时才作为强制项。审查不会提交材料或改变门户状态。

## 版本与许可

发布包包含通用 Skill、文档、许可、模板和虚构示例。版本见 [CHANGELOG.md](CHANGELOG.md)，许可与上游署名见 [LICENSE](LICENSE)、[NOTICE.md](NOTICE.md) 和 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。
