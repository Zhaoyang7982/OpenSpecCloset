# OpenSpecCloset

## 实验溯源与范式定位

本仓库为 **AI 原生范式对比实验** 中的 **OpenSpec 规格先行实验组** 承载仓库：以 **规格驱动开发（Spec-Driven Development）** 为纪律，在实现前将系统行为、数据语义与验收边界以业务契约形式固化。

- **业务真相源**：需求由既有可运行产品逆向归纳的「产品需求全集」草案，经本仓库抽象为 **不含实现细节** 的 OpenSpec 业务规格。  
- **唯一变量**：与对照组相比，**业务需求 100% 对齐**；仅开发范式不同（本组 **规格先行**，对照组 **代码驱动**），以保证对比实验客观性。  
- **对照组说明**：原「代码驱动」的衣橱产品仓库为成对对照；本 README 不引用其工程名或技术栈，避免污染实验变量。

## 需求来源

- 规格正文与验收场景全部来自逆向归纳的 **AI 衣橱助手** 产品需求全集（业务模块、流程、实体、非功能与端策略），经剔除实现细节后写入 `/specs`。  
- 已知交付缺口（新手引导、旅行模式占位、用户档案维护闭环等）在 [`specs/delivery-gaps.md`](specs/delivery-gaps.md) 与各模块需求文件中 **显式分栏**，便于对照实验写验收矩阵。

## 仓库目录说明

| 路径 | 说明 |
|------|------|
| [`specs/README.md`](specs/README.md) | 规格目录总览与阅读顺序 |
| [`specs/overview.md`](specs/overview.md) | 系统概述、实验定位、术语 |
| [`specs/business-goals.md`](specs/business-goals.md) | 业务目标 |
| [`specs/user-scenarios.md`](specs/user-scenarios.md) | 用户与场景摘要 |
| [`specs/information-architecture.md`](specs/information-architecture.md) | 信息架构与主导航 |
| [`specs/requirements/`](specs/requirements/) | 按模块拆分的功能需求（REQ 条文） |
| [`specs/data-model.md`](specs/data-model.md) | 数据实体业务语义 |
| [`specs/cross-cutting-flows.md`](specs/cross-cutting-flows.md) | 端到端核心流程 |
| [`specs/platform-and-sync-policies.md`](specs/platform-and-sync-policies.md) | 端策略、同步、隐私与性能（产品级） |
| [`specs/non-functional.md`](specs/non-functional.md) | 非功能要求索引 |
| [`specs/delivery-gaps.md`](specs/delivery-gaps.md) | 已知交付缺口与验收边界 |
| [`specs/acceptance/given-when-then.md`](specs/acceptance/given-when-then.md) | Given-When-Then 业务验收场景 |

## 使用方式

1. 以 [`specs/`](specs/) 为单一业务真相源进行评审与迭代。  
2. 实现与测试以 [`specs/acceptance/given-when-then.md`](specs/acceptance/given-when-then.md) 为验收依据，并与 `REQ-*` 条文双向追溯。  
3. 对照实验报告中的「规格—实现差距」应引用 `delivery-gaps.md` 与模块中的 GAP 段落。

## 许可与贡献

实验协议与贡献方式由仓库维护者另行约定；若需变更规格，请优先更新 `/specs` 并同步验收场景。
