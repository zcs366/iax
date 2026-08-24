# IAX · 心跳体

openLLM 六体之一 —— **心跳/调度（Heartbeat）**。

## 职责
10 阶段心跳主循环 —— 六体的起搏器。感知（IAI）的事件经 IAX 心跳进入主循环，由 IOS 决策分发。

## 当前状态
**骨架仓** —— IAX 的实体代码目前活在主仓 `zcs366/openllm` 内：
- `src/openllm/pipeline.py` — 心跳管线（`BodyName.IAX` 事件发布）
- `src/openllm/core/` — 循环调度
- `src/openllm/__init__.py` — 六体总览："一循环：iax·10阶段心跳主循环"

待 IAX 从主仓剥离独立成模块后，此仓将承接实体代码。本仓先立名占位，保持六体家族在 GitHub 上的完整对称。

## 与六体的关系
IAI（感知）→ **IAX（心跳）** → IOS（决策）→ ISN（执行）/ IKO（输出），记忆沉淀于 ISA。

> 六体家族：`zcs366/openllm` · `iai` · `iax` · `isa` · `isn` · `iko` · `ios`
