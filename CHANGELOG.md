# Changelog

## v0.5.3 (2026-05-31)

### 变更

- 报价章程（business/quotation.md）：新增第四章基准价格，含客户分类、人员分级、差异化定价框架；全文条款重编号（第十二条至第十四条）

## v0.5.2 (2026-07-10)

### 新增

- 绩效章程（human/performance.md），含总则、基本原则、责任认定与处理、附则
- 定义条款，解释基本业务流程、工时无效认定、绩效扣减、公司治理机构

### 变更

- 离职工作章程（human/resignation.md）新增离职分类，重编号全部条款
- 统一术语"公司代表大会"为"公司治理机构"
- myst.yml toc 新增绩效章程入口

## v0.5.1 (2026-07-10)

### 新增

- 基本章程（index.md），定义公司治理机构（创始人、股东代表大会、公司代表大会）
- 代表退出机制（company-representative.md 第七章），含辞职与罢免程序

### 变更

- 统一全部 18 份章程的效力声明为"经公司治理机构审议通过，自发布之日起生效"
- 重写离职工作章程（human/resignation.md）为标准格式，新增离职分析、工作复盘、答疑机制
- 重命名 human_resources 目录为 human，更新所有引用
- myst.yml toc 入口从 README 更新为 index

## v0.5.0 (2026-06-15)

### 新增

- 工作章程写作章程（write/bylaw.md），标准化文档结构、格式、语言规范
- 文档格式标准（docs/format.md），基于 Google 文档风格指南的 Markdown 写作规范
- CONTRIBUTING.md 贡献指南，说明目录命名风格
- README.md 添加项目定位与完整目录结构

### 变更

- docs/format.md 升级为正式章程，采用条款式结构与规范用语
- AGENTS.md 升级为元认知层，去除与 CONTRIBUTING 重复的操作细节

## v0.4.1 (2026-06-15)

### 新增

- 沟通管理章程（communication/index.md）
- 客户关系管理章程（customer-relationship.md）
- 公司秘书章程（secretary.md）
- 代表资格与产生条款（representative/qualification.md）
- 商务报价章程（business/quotation.md）

### 变更

- 议事章程升级为正式章程文本，重构结构
- 客户分级章程重命名，适配文档标准
- 职级管理章程重构，补充发展身份与完整等级体系
- 量潮数据审计文档融合为统一审计章程
- 更新 myst.yml 目录结构

## v0.4.0 (2026-05-15)

### 新增

- 审计章程目录（audit/）：审计总纲、元审计、项目质量审计、量潮课堂业务审计、量潮数据审计
- AGENTS.md 审计章程维护原则

### 变更

- 审计文档全面整理：统一标题层级、清除 AI 生成残留、规范化文件名
- 按域拆分审计文件：audit/ → qtclass/audit.md、project/audit.md、qtdata/audit.md
- 吸收审计授权原则至审计总纲（audit/index.md）
- 精简数据契约审计章程，聚焦核心框架

### 移除

- 删除数据契约审计章程中的过时内容（具体人事、推进状态、阶段性信息）
- 删除 qtdata/integrated.md（非审计内容）
- 删除 audit/authorization.md（授权细节过时，原则已吸收至总纲）

## v0.3.1 (2026-05-12)

### 新增

- 项目交付章程（qtdata/project.md）
- 资产管理章程（qtdata/asset.md）

### 变更

- 框架协议重写为工作章程（qtdata/index.md）
- 岗位架构重构为项目经理、商务经理、数据工程师三类（qtdata/org.md）
- 客户支持文档重构（qtdata/custom_support.md → support.md）

### 移除

- 移除参考资料、版本信息和维护人信息

## v0.3.0 (2026-05-11)

### 新增

- 量潮数据业务章程全套文档（框架协议、定价规则、岗位权责、客户支持、工作流程、交付标准）
- MyST 文档站点配置（myst.yml、工作流、GitHub Pages 自动部署）

### 变更

- 目录结构调整：量潮数据前置、组织管理后移

## v0.2.1 (2026-05-08)

### 新增

- 职级管理章程（organization/rank/index.md）

### 变更

- 重组组织架构文档：议事制度移至 department/ 目录
- 法定代表人制度移至 position/ 目录

## v0.2.0 (2026-05-05)

### 新增

- 议事制度（deliberation-institution.md）
- 法定代表人制度（company-representative.md）
- ROADMAP.md 产品路线图
- 两院制模型

### 变更

- 扩展离职工作章程
- 更新章程文档，适配写作格式标准

### 移除

- 移除写作格式章程，移至写作格式规范仓库

## v0.1.0 (2026-04-01)

### 首次发布

- 写作格式章程（format.md）
- 客户支持章程（custom_support.md）
- 议事章程（deliberation.md）
