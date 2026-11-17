# ROADMAP

本路线图记章程建设的方向与待办，版本记录见 CHANGELOG.md。

## 方向

章程建设的方向由 [qtconsult/index.md](qtconsult/index.md)（量潮咨询工作章程）标定，两条线并行推进：

- **对外谈判**：章程作为框架合同的基础，随交易交付客户，客户确认后即受约束。qtconsult 是按此标准写成的范例——定价、支付与退费、服务边界、咨询流程都写给客户看。此后评价一篇章程的首要问题是：客户拿到它能不能据此签约付款。
- **内部管理迁出**：只约束内部的管理章程迁往 quanttide-bylaw 领域仓，本仓收敛为「基本章程 + 对外章程」。审计、商务、文档格式三批已按此迁出。

## 对外章程

- [ ] qtconsult 入站收尾：`myst.yml` 导航、README 目录树、CHANGELOG 三处均未收录
- [ ] qtconsult 计费占位（每小时、每半日 XXX 元）对外使用前定稿
- [ ] 按 qtconsult 模式梳理 qtcloud、qtdata 的对客条款（计量计费、销售管理、客户支持、项目交付），可独立交付客户的抽出为对外章程
- [ ] `write/bylaw.md` 增补对外章程体例：总则、定价、支付与退费、服务边界、流程、附则

## 内部管理迁出

已迁出：审计五篇至 quanttide-bylaw-of-audit-management，商务三篇至 quanttide-bylaw-of-business-development，文档格式至 quanttide-bylaw-of-document-engineering。

- [ ] `human/` 至 quanttide-bylaw-of-human-resources
- [ ] `devops/` 至 quanttide-bylaw-of-devops
- [ ] `write/` 至 quanttide-bylaw-of-document-engineering
- [ ] `connect/`、`customer/`、`project/` 归置待定：现有领域仓无对应项，逐篇确认归 market、product、meta 或新设领域仓后迁出
- [ ] `qtcloud/`、`qtdata/` 按对外/对内拆分，对内部分逐篇归 data、asset、human 等领域仓——业务单元级章程的迁出涉及《量潮科技基本章程》第六条的章程体系条款，需同步修订

## 仓内同步

- [ ] README 目录树补齐现况：缺根 `index.md`、`devops/`、`qtcloud/`、`qtconsult/`、`write/`，`human/` 缺 training.md
- [ ] CHANGELOG Unreleased 收敛后，按 `devops/release.md` 发布下一版本
