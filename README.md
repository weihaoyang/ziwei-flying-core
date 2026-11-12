# 紫微飞星 · ziwei-flying core

宫干飞化与河洛数。从 [知几排盘](https://github.com/weihaoyang/qimen-llm-chart) 提取 TypeScript 实现、共享依赖模块与回归测试；暂未发布 npm 包。

## 运行

需要 Node.js 20 或更高版本。

```sh
npm install
npm run patch:3meta
npm test
npm run typecheck
```

运行前的补丁会修正本地依赖中的计算口径。入口位于 `src/lib/ziwei-flying/`。

## 资料与案例

[研究论文：古籍、现代模型与待核事项](https://github.com/weihaoyang/qimen-llm-chart/blob/main/docs/research/calculation-audit-paper.md)

- ships the ten-stem four-transformation table（`src/lib/ziwei-flying/chart.test.ts`）
- ships the tian-yi noble table and the He-Luo numbers（`src/lib/ziwei-flying/chart.test.ts`）
- applies the Jielan Ren-year transformation rather than the Quanshu variant（`src/lib/ziwei-flying/chart.test.ts`）
- builds twelve flying rows and the native four transformations（`src/lib/ziwei-flying/chart.test.ts`）
- derives each palace（`src/lib/ziwei-flying/chart.test.ts`）

案例验证具体输出字段，不验证占断效果。

## 授权与来源

本仓代码按 [GPL-3.0-only](LICENSE) 发布，源自知几排盘。飞化与河洛数的口诀来源及本仓组合的边界见研究论文；本仓保留上游 iztro MIT 许可。 其他随仓代码及依赖许可见 `LICENSES/`。不附古籍影像，其授权另按[影像权利记录](https://github.com/weihaoyang/qimen-llm-chart/blob/main/docs/research/sources/RIGHTS.md)核查。
