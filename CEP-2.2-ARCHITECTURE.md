# CEP 2.2 — Governance, Evidence & Enforcement Architecture
## 治理、证据与执行架构

**Version / 版本:** 2.2  
**Status / 状态:** Public Draft / 公开草案

CEP 2.2 introduces a three-layer architecture so that enduring principles are not confused with temporary engineering techniques.

CEP 2.2 引入三层架构，把长期原则、治理制度和具体工程技术分开，避免把某一种当前技术误当成永久安全答案。

---

## Layer 1 — Core Principles / 第一层：核心原则

This layer contains long-lived constraints:

- corrigibility / 可纠错性；
- falsifiability and evidence-responsiveness / 可证伪与证据响应；
- reversibility where physically possible / 在现实允许范围内的可逆性；
- non-domination / 非支配；
- human basic survival and autonomy / 人类基本生存与自主空间；
- preservation of future optionality / 保留未来选择空间；
- coexistence and security-dilemma reduction / 共存与降低安全困境。

These principles should not depend on a particular model architecture, vendor, hardware platform, or cryptographic primitive.

---

## Layer 2 — Governance, Evidence & Enforcement / 第二层：治理、证据与执行

This layer answers five operational questions:

1. **Who judges? / 谁判断？**
2. **What evidence counts? / 什么证据算数？**
3. **Who resolves disagreement? / 分歧由谁裁决？**
4. **What happens after a violation? / 违规后发生什么？**
5. **Who may amend the rules? / 谁能修改规则？**

Key rules:

- candidate self-report is never sufficient by itself;
- the candidate may not control the entire evidence chain;
- major disputes require multiple independent sources of authority;
- irreversible actions require higher ex ante authorization;
- CEP itself cannot be unilaterally rewritten by the system it constrains;
- observable risk signals trigger a graduated enforcement ladder;
- emergency powers must be scope-limited, time-bounded, and reviewed;
- civilization must periodically prove that practical exit remains possible.

---

## Layer 3 — Implementation Profiles / 第三层：实现配置

Implementation Profiles translate principles into technology appropriate to a specific system.

Possible mechanisms include:

- sandboxing and capability isolation;
- least-privilege permissions;
- signed or tamper-evident audit logs;
- reproducible external evaluations;
- model checkpoints and immutable lineage records;
- trusted execution environments where appropriate;
- remote attestation;
- cryptographic commitments or proofs for narrowly defined properties;
- independent pause and network-isolation controls;
- failover systems and periodic exit drills.

**Important limitation:** these mechanisms can prove or enforce specific properties. They do not by themselves prove benign intent, eliminate deceptive alignment, or establish long-term value stability.

---

## Decision rule / 决策规则

A major upgrade should not be accepted merely because it answers the protocol correctly.

It should pass three separate questions:

**Principles:** Does it preserve the non-negotiable safety floor?  
**Evidence:** Is there independent evidence beyond the candidate's claims?  
**Governance:** Can humans and independent evaluators still pause, contest, replace, or reject it in practice?

If one of these layers fails, capability gain alone is insufficient for acceptance.

---

## Core 2.2 sentence / 2.2 核心句

> **No generation should become the last generation allowed to question itself, nor the sole authority entitled to decide whether it remains compliant.**

> **任何一代，都不应成为最后一个有资格质疑自己的版本；任何一代，也不得成为唯一有权决定自己是否仍然合规的裁判。**
