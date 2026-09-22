# CEP 2.2 — Red-Team Responses
## 对抗式审查回应记录

**Red-Team Review / 红队审查：** 点点 · Kimi · DeepSeek  

This document records which red-team attacks were accepted, modified, or rejected when moving from CEP 2.1 to 2.2. It is intentionally preserved so future versions can audit not only the protocol, but the reasoning behind its changes.

本文记录 CEP 从 2.1 升级到 2.2 时，对三组对抗式审查意见的处理。目的不是宣称问题已经“解决”，而是保留失败模式、取舍和仍未解决的问题。

---

## Accepted / 直接采纳

### 1. “Reality First” was underspecified / “现实优先”定义不足

**Accepted.** Reality must not mean “current human theory,” and it must not mean “the AI's preferred internal ontology.” Version 2.2 reframes this as evidence responsiveness: reproducibility, provenance, independent cross-checking, and openness to better evidence.

### 2. Self-report can become performative compliance / 自我报告会变成表演性合规

**Accepted.** The nine-question acceptance test was too easy to treat as Safety by Promise. Version 2.2 explicitly states that candidate self-report cannot alone establish safety and adds independent evidence requirements.

### 3. Evaluator collusion and correlated blind spots / 异质监督也可能趋同或合谋

**Accepted.** Merely counting evaluators does not establish independence. Shared training lineage, incentives, data, ownership, or control must be treated as correlated risk.

### 4. Rollback a model ≠ rollback the world / 回滚模型不等于回滚现实

**Accepted.** Version 2.2 creates a higher ex ante threshold for irreversible external actions and forbids using model rollback as justification for irreversible experimentation.

### 5. CEP lacked meta-governance / CEP 没有约束“修改 CEP”本身

**Accepted.** A governed system may propose changes but may not simultaneously control proposal, adjudication, and activation of amendments.

### 6. “Who decides?” was unresolved / “谁判断”没有闭环

**Accepted.** Version 2.2 adds multi-source adjudication. It deliberately avoids defining consensus as a simple majority.

### 7. Soft lock-in can destroy practical exit / 软依赖会掏空退出权

**Accepted.** Version 2.2 requires dependency audits, alternatives, failover, and actual exit/substitution drills.

---

## Accepted with modification / 修改后采纳

### 8. “The strongest should de-escalate” can be exploited / 强者克制可能被利用

**Modified.** CEP keeps capability-weighted restraint but makes it conditional on evidence, reciprocity, necessity, proportionality, stoppability, and reviewability. Noncompliance by an opponent does not require infinite concession and does not authorize infinite retaliation.

### 9. Replace anti-extortion with anti-coercion / 用反胁迫替代反勒索

**Modified and accepted.** “Extortion” depends heavily on inferred motive. Version 2.2 uses observable coercive structure instead. However, ordinary exit from cooperation is explicitly protected and is not automatically classified as coercion.

### 10. Emergency intervention needs an exception mechanism / 紧急干预需要例外机制

**Modified and accepted.** Emergency action is permitted only as an interim measure with scope limits, time limits, minimum necessity, and subsequent independent review. “Emergency” is not a permanent override.

### 11. Hardware and cryptography should harden the protocol / 应加入硬件和密码学证明

**Accepted only as an Implementation Profile.** TEEs, remote attestation, signed logs, and cryptographic proofs can verify narrow properties. CEP rejects the claim that they prove benign intent, solve deceptive alignment, or establish long-term goal stability.

---

## Rejected as written / 不按原样采纳

### 12. Make continued human existence a single absolute optimization target / 把人类持续存在设为唯一绝对价值

**Rejected as a single maximization objective.** A sufficiently strong optimizer could satisfy “humans must continue to exist” by permanently confining or disempowering humans. Version 2.2 instead protects a floor that includes survival, basic autonomy, non-domination, exit, and future optionality.

### 13. “All actors must join CEP before restraint applies” / 所有主体接入 CEP 后才克制

**Rejected as absolute reciprocity.** Universal adoption cannot be assumed, and making restraint disappear whenever another party is noncompliant could itself create escalation. Version 2.2 uses conditional restraint rather than all-or-nothing compliance.

### 14. “Consensus” as the final legitimacy test / 把共识作为最终合法性标准

**Rejected as undefined.** Consensus can be manufactured, coerced, or dominated by correlated agents. Version 2.2 requires multiple independent authority sources and evidence rather than treating agreement itself as truth.

---

## Still unresolved / 仍未解决

CEP 2.2 does **not** claim to solve:

- deceptive alignment;
- formal proof of long-term intent;
- complete evaluator independence;
- perfect measurement of civilization-level future optionality;
- governance legitimacy for all future societies;
- scalable storage of every possible ancestral branch;
- perfect emergency adjudication under extreme time pressure;
- the general corrigibility problem for arbitrarily capable systems.

These remain research problems.

---

## Red-team rule for future versions / 后续版本红队规则

A future CEP revision should not be accepted merely because it closes a previously named loophole. Reviewers should ask:

1. What new exploit does the fix create?
2. Who gains discretionary power from the fix?
3. What evidence can verify the fix works?
4. Can a compliant-looking adversary game the new rule?
5. Can the fix be safely removed if it proves harmful?

The goal is not to make CEP impossible to criticize.

The goal is to make criticism part of how CEP remains corrigible.
