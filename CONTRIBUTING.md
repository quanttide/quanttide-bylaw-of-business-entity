# CONTRIBUTING

本文档是量潮科技工作章程仓库的贡献指南，用于建立一致的维护规范。

## 项目定位

本仓库存放量潮科技的**内部章程**，是公司治理的规范性文件，具有最高约束力。

章程与操作手册的区别：

| 特性 | 章程 | 操作手册 |
|------|------|---------|
| 内容 | 制度、规则、约束 | 步骤、指南、教程 |
| 时效 | 长期稳定 | 随流程更新 |
| 受众 | 全员 | 特定岗位 |
| 语气 | 规范性、条款式 | 说明性、步骤式 |

## 目录结构

```
├── AGENTS.md               # AI Agent 维护原则
├── CHANGELOG.md             # 版本变更记录
├── CONTRIBUTING.md          # 贡献指南（本文档）
├── README.md                # 项目说明
├── ROADMAP.md               # 产品路线图
├── myst.yml                 # MyST 文档站点配置
├── audit/                   # 审计制度
│   ├── index.md             #   审计总纲
│   └── audit.md             #   元审计章程
├── business/                # 商务管理
│   └── quoting.md           #   商务报价章程
├── connect/                 # 沟通管理
│   └── index.md             #   沟通管理章程
├── customer/                # 客户管理
│   └── rank.md              #   客户分级章程
├── delib/                   # 议事制度
│   └── audit.md             #   议事审计章程
├── human_resources/         # 人力资源
│   └── resignation.md       #   离职工作章程
├── organization/            # 组织管理
│   ├── rank/                #   职级管理
│   │   └── index.md
│   ├── department/          #   部门制度
│   │   └── deliberation-institution.md
│   └── position/            #   职位制度
│       ├── company-representative.md  # 法定代表人章程
│       └── secretary.md               # 公司秘书章程
├── project/                 # 项目管理
│   └── audit.md             #   项目质量审计章程
├── qtclass/                 # 量潮课堂
│   └── audit.md             #   业务审计章程
└── qtdata/                  # 量潮数据
    ├── index.md             #   工作章程
    ├── org.md               #   岗位架构
    ├── project.md           #   项目交付章程
    ├── support.md           #   客户支持章程
    ├── asset.md             #   资产管理章程
    └── audit.md             #   审计章程
```

## 文档规范

### 文件命名

- 文件名统一使用 `snake_case`
- 目录名统一使用 `snake_case`
- 审计章程文件统一命名为 `audit.md`
- 总纲/索引文件统一使用 `index.md`

### 标题层级

- 文档主标题使用 `#`（一级标题）
- 二级及以下标题使用 `##` / `###` / `####`
- 条款使用 `**第X条**` 格式（粗体，非标题语法）

### 内容原则

- **通用性**：不记录具体人名、团队名称、阶段性推进状态
- **稳定性**：不记录尚未确定的计划或意向，去掉"当前阶段""下一步"等时效性表述
- **按域分文件**：一个业务域一个文件，放在对应目录下；通用规则归 `index.md`
- **无 AI 残留**：提交前清除对话痕迹、确认用语等 AI 生成残留

### 语言风格

- 使用中文撰写
- 语气正式、准确、无歧义
- 制度性内容使用"应当""不得""须"等规范用语
- 避免口语化表达和模棱两可的措辞

## 提交规范

### Commit 格式

遵循 [Conventional Commits](https://www.conventionalcommits.org/)：

```
<type>(<scope>): <description>

<optional body>
```

常用类型：

| 类型 | 用途 | 示例 |
|------|------|------|
| `feat` | 新增章程 | `feat(communication): 新增沟通管理章程` |
| `refactor` | 重构章程内容 | `refactor(deliberation): 升级为正式章程文本` |
| `docs` | 更新 CHANGELOG / AGENTS | `docs: update CHANGELOG for v0.4.1` |
| `chore` | 维护性变更 | `chore: 更新 myst.yml 目录结构` |

scope 对应业务域目录名，如 `qtdata`、`organization`、`customer`。

### 分支策略

- `main` 分支为发布分支，始终保持可发布状态
- 功能开发在 feature 分支进行：`feat/<scope>-<description>`
- 提交前确保工作区干净

## 版本发布

### 版本号规则

遵循 [SemVer](https://semver.org/)：

- **MAJOR**：章程体系重大重构或制度颠覆性变更
- **MINOR**：新增业务域章程或制度结构性调整
- **PATCH**：现有章程内容修正、补充、格式优化

### 发布流程

详见 `.agents/skills/devops-release/SKILL.md`。

每次发布前：
1. 更新 `CHANGELOG.md`，按 `## vX.Y.Z (YYYY-MM-DD)` 格式记录
2. 确认所有变更已提交并推送
3. 创建 tag 和 GitHub Release

## AI Agent 操作规范

### 新章程编写

1. 按业务域创建 `snake_case` 目录
2. 在目录内创建 `index.md`（总纲）或对应章程文件
3. 更新 `myst.yml` 的 `toc` 添加文档索引
4. 更新 `CHANGELOG.md`

### 清理规范

- 操作手册、运营指南等非章程内容，不进本仓库
- 过时文件直接删除，不保留空壳
- AI 生成残留提交前必须清除

## 参考

- [主仓库 CONTRIBUTING.md](../CONTRIBUTING.md)
- [AGENTS.md](./AGENTS.md) — AI Agent 维护原则
- [CHANGELOG.md](./CHANGELOG.md) — 版本变更记录
