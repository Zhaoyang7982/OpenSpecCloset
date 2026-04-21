# OpenSpec 规格目录说明

本目录存放 **AI 衣橱助手** 的业务规格（Business Specification），遵循规格先行（Spec-Driven）思路：**先约定可验收的系统行为与数据契约，再进入实现**。

## 阅读顺序建议

1. [`overview.md`](overview.md) — 实验溯源、范围与规格原则  
2. [`business-goals.md`](business-goals.md) — 业务目标  
3. [`user-scenarios.md`](user-scenarios.md) — 用户与场景摘要  
4. [`information-architecture.md`](information-architecture.md) — 信息架构与主导航  
5. [`requirements/`](requirements/) — 按模块拆分的功能需求（规范性条文）  
6. [`data-model.md`](data-model.md) — 数据实体业务语义  
7. [`cross-cutting-flows.md`](cross-cutting-flows.md) — 端到端核心流程  
8. [`platform-and-sync-policies.md`](platform-and-sync-policies.md) — 端策略、同步与数据归属  
9. [`non-functional.md`](non-functional.md) — 非功能要求（产品级）  
10. [`delivery-gaps.md`](delivery-gaps.md) — 已知交付缺口与「约定能力 / 待补齐」边界  
11. [`acceptance/`](acceptance/) — Given-When-Then 业务验收场景  

## 文档性质

- 规格为 **纯业务契约**：不绑定具体平台、运行时、存储形态或工程结构。  
- 与对照实验另一仓库的 **业务需求 100% 对齐**；实验唯一变量为 **AI 原生开发范式**（规格先行 vs 代码驱动），以保证对比客观性。

## 需求标识

模块需求条文中使用 `REQ-模块-序号` 形式标识，便于与验收场景交叉引用。
