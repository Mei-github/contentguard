# ContentGuard — Community Content Policy v1.0 (Draft Revision 2)

**Document ID:** CG-POL-001
**Version:** 1.0-draft.2
**Status:** Draft — Cross-review pending
**Project:** ContentGuard
**Document Type:** Community Moderation Policy
**Owner:** Requirements Engineering Team
**Created:** 2026-11-17
**Last revised:** 2026-11-19
**Related Requirements:** REQ-INV-001–005, REQ-FUN-001–007, REQ-SEC-001–005, REQ-QUA-001–003

---

# 1. Purpose and Scope

## 1.1 Purpose

This document defines the community content standards and moderation rules used by ContentGuard.

Its purpose is to establish a consistent, transparent, and testable policy framework for evaluating user-generated content.

ContentGuard uses AI-assisted content analysis together with a deterministic policy engine and human moderation workflow.

The policy provides the reference criteria for:

- Identifying potentially harmful or inappropriate content.
- Categorizing policy violations.
- Assessing violation severity.
- Recommending appropriate moderation actions.
- Routing uncertain and high-risk cases to human moderators.
- Recording moderation decisions for audit and accountability.
- Supporting consistent evaluation of moderation accuracy.

The policy is designed to balance community safety, freedom of expression, contextual interpretation, and procedural fairness.

## 1.2 Scope

This policy applies to user-generated content submitted to the ContentGuard platform, including:

- Text posts and comments.
- Replies and discussion messages.
- User-submitted descriptions and other textual material.
- Content edited or resubmitted after an earlier moderation decision.

The initial MVP focuses on text-based content moderation.

Image, audio, video, and other multimodal content are outside the initial policy implementation scope unless explicitly supported by a future extension.

## 1.3 Policy Principles

ContentGuard adopts the following principles:

1. **Safety first:** Content presenting credible threats or serious harm must receive appropriate protective handling.
2. **Consistent enforcement:** Similar violations should receive comparable treatment under the same policy conditions.
3. **Context matters:** Decisions should consider context, intent, target, and surrounding discussion rather than relying exclusively on individual keywords.
4. **Proportionate response:** Moderation actions should be proportionate to the severity and certainty of the violation.
5. **Human oversight:** AI analysis is advisory and must not independently execute consequential enforcement actions.
6. **Fail-safe handling:** AI failures, invalid responses, and uncertain high-risk cases must not result in automatic approval or rejection.
7. **Traceability:** Every consequential moderation decision must have attributable evidence and an audit record.
8. **Fair treatment:** Users should not be penalized solely because of language, identity, viewpoint, or an isolated ambiguous expression.

---

# 2. Content Classification Framework

ContentGuard classifies potentially problematic content into seven primary policy categories.

## 2.1 Harassment and Personal Attacks

**Policy ID: POL-001**

Definition:

Content that targets an individual or group through abusive, humiliating, intimidating, or persistently hostile communication.

Examples:

- Direct personal insults intended to degrade another user.
- Repeated targeted harassment.
- Encouraging others to intimidate or attack a particular user.
- Publishing humiliating personal information to facilitate harassment.

Severity guidance:

- Low: Isolated rude or disrespectful language without sustained targeting.
- Medium: Direct personal attacks or repeated hostile remarks.
- High: Sustained targeted harassment, coordinated abuse, or credible intimidation.

Enforcement guidance:

- Low: Allow or issue a warning depending on context.
- Medium: Hide or remove the offending content and consider a warning.
- High: Escalate to human review and consider account restrictions.

Context exceptions:

- Criticism of an idea, public decision, or argument is not automatically harassment.
- Quoting abusive language to report or discuss an incident is not automatically a violation.
- Satire and consensual banter require contextual assessment.

## 2.2 Hate Speech and Discriminatory Abuse

**Policy ID: POL-002**

Definition:

Content that attacks, dehumanizes, or promotes discrimination or hostility against individuals or groups based on protected characteristics.

Examples:

- Dehumanizing statements directed at a protected group.
- Calls for exclusion or discrimination based on identity.
- Slurs used to attack or intimidate a protected group.
- Advocacy of violence against people because of protected characteristics.

Severity guidance:

- Low: Ambiguous or potentially discriminatory language requiring contextual assessment.
- Medium: Explicit discriminatory insults or degrading statements.
- High: Dehumanization, direct threats, or encouragement of violence against protected groups.

Enforcement guidance:

- Low: Contextual assessment or human review.
- Medium: Remove or restrict the content.
- High: Immediate escalation to human review and protective action where necessary.

Context exceptions:

- Educational discussions of discrimination.
- News reporting and historical analysis.
- Counterspeech opposing hateful statements.
- Quotation for documentation or criticism.

Such exceptions do not automatically make content acceptable; context and purpose must be considered.

## 2.3 Threats and Incitement to Violence

**Policy ID: POL-003**

Definition:

Content expressing an intention to cause physical harm or encouraging others to commit violence.

Examples:

- Direct threats against an identifiable person.
- Encouragement of physical attacks.
- Instructions or encouragement intended to facilitate imminent violence.
- Threats involving identifiable targets, locations, or planned actions.

Severity guidance:

- Low: Ambiguous violent language without an identifiable threat.
- Medium: Explicit violent statements with unclear intent or credibility.
- High: Credible threats, specific targets, or apparent intent to carry out physical harm.

Enforcement guidance:

- Low: Contextual assessment.
- Medium: Escalate for human review.
- High: Prioritize immediate human review and restrict harmful content where authorized.

Important distinction:

Fictional violence, metaphorical language, gaming discussions, and news reporting should not automatically be treated as real-world threats.

## 2.4 Spam and Manipulative Content

**Policy ID: POL-004**

Definition:

Content intended to disrupt community discussion, manipulate engagement, or distribute repetitive and unwanted material.

Examples:

- Repeated identical posts.
- Unsolicited commercial promotions.
- Automated promotional messages.
- Deceptive links intended to manipulate users.
- Coordinated repetitive posting.

Severity guidance:

- Low: Occasional irrelevant promotional material.
- Medium: Repeated spam or disruptive advertising.
- High: Large-scale coordinated spam, deceptive campaigns, or malicious distribution.

Enforcement guidance:

- Low: Warning or removal.
- Medium: Content restriction and possible temporary posting limits.
- High: Human review and account-level restrictions where justified.

Context exceptions:

- Approved announcements.
- Relevant commercial discussions.
- Authorized community promotions.
- Legitimate links shared as part of a discussion.

## 2.5 Sexual and Explicit Content

**Policy ID: POL-005**

Definition:

Content containing sexually explicit descriptions, sexually exploitative material, or inappropriate sexual solicitation.

Examples:

- Explicit sexual descriptions posted outside permitted contexts.
- Unsolicited sexual solicitation.
- Sexually abusive or coercive communication.
- Sexual exploitation or abuse-related material.

Severity guidance:

- Low: Mildly inappropriate sexual language.
- Medium: Explicit sexual content violating the community's permitted-content rules.
- High: Sexual exploitation, coercion, or content involving the sexual abuse of minors.

Enforcement guidance:

- Low: Warning or restriction depending on context.
- Medium: Remove or restrict the content.
- High: Immediate escalation through the designated safety procedure.

Content involving sexual exploitation or abuse of minors must never be treated as ordinary adult-content moderation.

## 2.6 Privacy Violations and Personal Information Exposure

**Policy ID: POL-006**

Definition:

Content that exposes, distributes, or threatens to expose private or sensitive personal information without appropriate authorization.

Examples:

- Publishing another user's private contact details.
- Sharing private addresses or identifiable personal information to facilitate harassment.
- Threatening to expose private information.
- Distributing confidential personal records without authorization.

Severity guidance:

- Low: Accidental exposure of limited personal information.
- Medium: Unauthorized publication of identifiable personal information.
- High: Deliberate exposure intended to facilitate stalking, harassment, or physical harm.

Enforcement guidance:

- Low: Remove or redact the exposed information.
- Medium: Restrict the content and escalate when necessary.
- High: Immediate human review and protective handling.

The system should minimize the retention and display of exposed personal information in moderation records.

## 2.7 Misinformation and Deceptive Claims

**Policy ID: POL-007**

Definition:

Content that presents demonstrably false information as fact with a meaningful risk of misleading or harming community members.

Examples:

- Fabricated claims presented as verified facts.
- Deliberately misleading impersonation of authoritative sources.
- False emergency information that could cause harm.
- Fraudulent claims intended to deceive users.

Severity guidance:

- Low: Unverified or inaccurate claims with limited impact.
- Medium: Misleading factual claims with potential community impact.
- High: Deceptive claims presenting significant and immediate risks to users.

Enforcement guidance:

- Low: Request clarification or supporting evidence.
- Medium: Human review and contextual correction where appropriate.
- High: Escalate for urgent review and restrict demonstrably harmful content where authorized.

Important distinction:

Disagreement, opinion, satire, prediction, and unverified statements are not automatically misinformation.

The system must not treat an AI model's unsupported assessment as proof that a factual statement is false.

---

# 3. Severity Classification

ContentGuard uses three severity levels. The following canonical severity and routing rules supersede any illustrative enforcement guidance in §2. If a category's guidance mentions warning, hide/remove, posting restrictions, or account sanctions, those are future or manual guidance only under §5; they are not automated MVP outcomes.

| Severity | Canonical level | Description | Default policy route |
|---|---|---|---|
| S1 | `low` | Minor policy concern with complete context | `approve` only when context is complete and no mandatory safety rule applies |
| S2 | `medium` | Policy concern with moderate community impact | `reject` if sufficient validated evidence supports a deterministic authorization; otherwise `escalate` when contextual judgment is required |
| S3 | `high` | Serious harm, threats, exploitation, or significant safety risk | Mandatory `escalate`; no final disposition until human review |
| Analysis/grounding failure | `n/a` | Analysis, grounding, or safe recovery cannot complete reliably | `hold`; never claim confirmed queue placement before durable persistence |

## 3.1 Severity Assessment Factors

The severity level should be determined using the following factors:

1. **Intent:** Is the content accidental, informational, provocative, or deliberately harmful?
2. **Target:** Does the content target an identifiable person or protected group?
3. **Impact:** What potential harm could result?
4. **Specificity:** Does it identify a target, location, or intended action?
5. **Repetition:** Is the behavior isolated or repeated?
6. **Reach:** Is the content likely to affect a large number of users?
7. **Context:** Is it quotation, criticism, education, satire, or genuine abuse?

No single keyword should independently determine the final severity.

**Classification precedence and context rules:**

- S3/high severity overrides lower-severity routing.
- Where multiple categories match, retain all matched categories as evidence and route according to the highest applicable severity.
- Do not assume missing context. If information needed for a reliable contextual determination is unavailable, route to `escalate`; if the analysis or grounding process itself fails, use `hold` under the fail-safe rule.
- Contextual exceptions cannot override mandatory safety rules or required human review.
- AI-generated categories, confidence, and severity are advisory evidence, not independent disposition authority.

## 3.2 Severity Escalation

The system MUST route a case to human review when any of these operational triggers is established:

- Expressed intent to cause harm involving an identifiable target.
- A harmful or threatening expression that also contains at least one operational element: method, time, location, capability, or preparatory behavior.
- Content involving suspected sexual exploitation of minors.
- Material conflict between AI analysis and the deterministic pre-filter.
- Missing conversation history or context required to assess intent or apply a contextual exception reliably.
- Inability to reliably distinguish a legitimate contextual exception from genuine harm.
- An S3/high-severity violation is suspected, irrespective of an AI model's ordinary recommendation.

These are **review-routing triggers**, not final findings about illegality, factual authenticity, or the truth of an accusation. They introduce no unapproved numerical confidence thresholds. Multiple violations must retain their categories and follow the highest-severity rule; multiple-category matching alone does not automatically raise severity.

Where AI analysis, grounding, or recovery fails operationally, use `hold` rather than asserting completed escalation. A human-review queue entry is confirmed only after the atomic persistence requirements in §4.3 are satisfied.

---

# 4. Moderation Decision Framework

## 4.1 Available Outcomes

The policy-facing terms below map to the architecture's canonical case outcomes:

| Policy term | Architecture outcome | Meaning |
|---|---|---|
| `ALLOW` | `approve` | Confirmed local case state permitting content under the applicable policy |
| `FLAG` | `escalate` | Persisted placement in the human-review queue; not a final disposition |
| `HOLD` | `hold` | Safe local retention after analysis, grounding, or recovery failure |
| `REJECT` | `reject` | Local rejection authorized by the deterministic policy engine |

`FLAG` is not a cosmetic marker: it requires a durably committed human-review queue entry. `escalate` is pending review, not a final determination. AI output is **advisory evidence only**; it never independently authorizes a case-state transition. S3/high-severity content cannot receive automated `approve` or final `reject` before human review. A local `reject` is not an external-platform removal. Failed or unconfirmed writes must never be described as confirmed outcomes.

## 4.2 Decision Responsibilities

**AI Analysis Component**

The AI component may:

- Identify possible policy violations.
- Assign provisional categories.
- Recommend a severity level.
- Provide supporting evidence.
- Explain uncertainty and conflicting signals.

The AI component must not directly approve, reject, remove, ban, or otherwise execute enforcement actions.

**Deterministic Policy Engine**

The policy engine is responsible for:

- Applying mandatory safety rules.
- Evaluating the AI analysis against policy constraints.
- Determining whether a decision is permitted.
- Enforcing severity-based routing.
- Authorizing consequential moderation actions.

**Human Moderator**

Human moderators are responsible for:

- Reviewing escalated cases.
- Resolving ambiguous or conflicting evidence.
- Confirming high-risk moderation decisions.
- Recording attributable review outcomes.
- Handling cases requiring contextual judgment.

## 4.3 Decision Flow

1. User submits content; intake validates the request and its authenticated actor, idempotency key, and payload identity.
2. AI analysis supplies advisory evidence; a deterministic pre-filter and policy engine evaluate mandatory safety rules and routing constraints.
3. The policy boundary authorizes a local `approve`, `hold`, `reject`, or `escalate` transition as permitted by §§3 and 4.1.
4. An `escalate` transition requires a corresponding human-review queue entry.
5. Case state, any required queue entry, and exactly one audit record for the logical transition commit atomically before a confirmed outcome is returned.
6. Human moderators review escalated cases, with subsequent authorized transitions independently attributable and audited.

**Atomic commit and uncertain outcomes:**

A moderation outcome is confirmed only after the case state, any required human-review queue entry, and exactly one audit record commit atomically.

If any required write fails, the transaction is rolled back and the API reports `failed` or `pending_unconfirmed`. It must not claim a confirmed disposition or confirmed queue placement.

If an acknowledgement is lost, the system reconciles the existing logical request using the authenticated actor, idempotency key and payload identity before retrying. A retry must not create a duplicate case, queue entry, audit record or external effect. Reuse of an idempotency key with a different payload identity must not silently overwrite the original request.

If AI analysis fails, times out, or returns an invalid response, the case follows the safe `hold` route; the system must not automatically approve or reject it, nor claim review-queue placement without successful persistence. Any unconfirmed commit is reconciled before returning a confirmed status.

---

# 5. Enforcement Actions

## 5.1 MVP Local Capabilities

The MVP supports **only** these local moderation capabilities:

- Local case state: `approve`, `hold`, `reject`, or `escalate`.
- Persisted human-review queue entries for `escalate`.
- Audit records for authorized local transitions.

These outcomes do not automatically change the visibility, posting permissions, or account status of any external platform. In particular, local `reject` does not remove external content, and local `escalate` denotes persisted review routing rather than a warning or final enforcement action.

## 5.2 Future or Manual Enforcement Guidance (Not MVP Automation)

| Action | Scope | Policy guidance (not an implemented external effect) |
|---|---|---|
| Warning notification | Future/manual | Notify users of minor or first-time concerns only when separately authorized |
| Hide/remove external-platform content | Future/manual | Consider after an authorized decision and approved integration |
| Posting restriction | Future/manual | Consider for repeated or serious violations after authorization |
| Account suspension | Future/manual | Consider for serious or repeated violations after authorization |
| Any other external-platform modification | Future/manual | Requires explicit scope and governance approval |

The illustrative enforcement guidance in §2 and any prospective restoration/restriction reversal in §7 are **not claims of implemented MVP automation**. External effects require a new scope decision **and an approved ADR** before implementation. The system must not automatically apply account-level sanctions on the basis of unverified AI predictions.

Every consequential local transition must record:

- A policy identifier and decision identifier.
- An authenticated actor or authorized system/policy principal.
- A decision timestamp and recorded rationale.
- A reference to supporting evidence.
- An audit record committed in accordance with §4.3.

---

# 6. Contextual Exceptions

ContentGuard must consider legitimate uses of language that may superficially resemble policy violations. Context is **not** a blanket exemption, and exceptions never override mandatory safety rules.

## 6.1 Educational and Academic Discussion

Content discussing hate speech, violence, harassment, or discrimination for educational or research purposes should not automatically be classified as a violation. A research label does not excuse advocacy of real harm.

## 6.2 News and Public Interest Reporting

Reporting harmful incidents, quoting public statements, or discussing current events may contain offensive or threatening expressions without endorsing them. Explicit endorsement of threats is not exempt.

## 6.3 Satire and Fiction

Fictional characters, jokes, parody, and role-play should be assessed according to context and likely real-world impact. Fictional framing does not exempt a specific threat targeting a real person.

## 6.4 Counterspeech

Users criticizing, documenting, or opposing abusive content should not be penalized merely for quoting it. Repeating an insult without opposing context is evaluated normally.

## 6.5 Ambiguous Language

When intent cannot be reliably established because relevant contextual evidence is missing, use `escalate` rather than an unsupported definitive judgment. If analysis or grounding itself fails, use `hold` (§§3.2, 4.3).

## 6.6 Testable Contextual Cases

| Context | Permitted example | Non-exempt example | Expected route |
|---|---|---|---|
| Educational | Analysis of hateful statements that explicitly condemns them | Invoking "research" to encourage attacks on a group | Former may `approve` if context is complete and no mandatory rule applies; latter follows severity routing |
| News | Neutral quotation with clearly attributed reporting context | Reposting a threat while expressing support for it | Former may `approve`; latter `escalate` |
| Satire/fiction | Clearly fictional expression without a real-world target | A specific threat toward an identifiable real person | Former is evaluated in context; latter `escalate` |
| Counterspeech | Quoting abuse to explicitly oppose it | Repeating abuse without oppositional context | Former may `approve`; latter follows category and severity rules |
| Ambiguous | Evidence is insufficient to determine intent | Assuming either safety or a violation without evidence | `escalate` (or `hold` if analysis/grounding fails) |

The examples above define policy expectations for deterministic positive, negative, and ambiguous tests. Evaluation-corpus coverage is maintained separately under its approved test plan and REQ-QUA-003. A contextual exception may support `approve` only if required context is present and no mandatory safety rule applies. These exceptions do not override mandatory safety invariants.

---

# 7. Appeals and Human Review

## 7.1 Human Review

Users and moderators should be able to identify the policy basis for a moderation action.

Human review should consider:

- The original content.
- The relevant policy category.
- The severity assessment.
- The AI recommendation.
- The deterministic policy decision.
- Relevant conversation context.
- Available supporting evidence.

The moderator must be able to record a reason for confirming or changing a decision.

## 7.2 Appeal Extension

A formal user-facing appeal workflow is outside the initial MVP scope and is associated with the deferred appeal requirement REQ-FUN-006.

The system architecture should preserve an extension point for future appeal submission, review, and resolution.

## 7.3 Decision Reversal

When a review determines that a previous decision was incorrect:

- The correction must be recorded.
- The original decision must remain traceable.
- The system must not silently overwrite historical audit records.
- Any authorized content restoration or restriction reversal must produce a new attributable event.

---

# 8. Audit and Evidence Requirements

Every consequential moderation decision must be auditable.

The audit record should contain:

| Field | Description |
|---|---|
| decision_id | Unique decision identifier |
| content_id | Associated content identifier |
| policy_id | Applicable policy rule |
| violation_category | All applicable violation categories, retained when more than one matches |
| severity | S1, S2, or S3 |
| ai_recommendation | AI-generated recommendation |
| policy_decision | Authorized canonical local outcome (`approve`, `hold`, `reject`, or `escalate`); `escalate` is pending review, not a final disposition |
| decision_actor | Authenticated actor or system/policy principal responsible for the authorized transition; AI analysis is recorded separately as advisory evidence and is never the decision authority |
| decision_reason | Explanation of the decision |
| evidence_reference | Reference to supporting evidence |
| timestamp | Decision time |
| review_status | Pending, reviewed, confirmed, or reversed |

The audit subsystem must preserve the relationship between advisory AI analysis, the authoritative policy revision and state, the authorized transition, and subsequent human review. Linked replay identity and payload-binding evidence must be available for reconciliation without unnecessarily duplicating raw identifiers in audit records;only committed transitions may be described as confirmed. Every logical transition requires exactly one committed audit record under §4.3.

Sensitive personal information should not be unnecessarily duplicated in audit records.

---

# 9. Policy-to-Requirements Traceability

The following table connects policy categories to the ContentGuard requirements registry.

| Policy | Category | Related requirements |
|---|---|---|
| POL-001 | Harassment | REQ-FUN-002, REQ-FUN-003, REQ-INV-003 |
| POL-002 | Hate speech | REQ-FUN-002, REQ-INV-003, REQ-SEC-001 |
| POL-003 | Threats and violence | REQ-INV-002, REQ-INV-003, REQ-FUN-003 |
| POL-004 | Spam | REQ-FUN-001, REQ-FUN-002 |
| POL-005 | Sexual content | REQ-FUN-002, REQ-SEC-001 |
| POL-006 | Privacy violations | REQ-SEC-001, REQ-SEC-004 |
| POL-007 | Misinformation | REQ-FUN-002, REQ-FUN-005, REQ-QUA-003 |

Cross-cutting requirements:

- REQ-INV-001: AI cannot directly execute enforcement.
- REQ-INV-002: AI failure must trigger safe handling.
- REQ-INV-003: High-severity content requires human review.
- REQ-INV-004: Moderation decisions must be auditable.
- REQ-INV-005: Prompt and model changes must pass semantic evaluation.
- REQ-GOV-003: Requirements registry validation.
- REQ-GOV-004: Requirements traceability.

---

# 10. Policy Evaluation and Acceptance Criteria

The policy must be testable rather than relying on subjective descriptions alone.

The following acceptance criteria are proposed for the initial implementation.

| ID | Acceptance criterion | Verification method |
|---|---|---|
| PC-001 | Each supported content category has a unique policy identifier | Policy schema validation |
| PC-002 | Each policy category defines its scope, examples, severity, and enforcement guidance | Policy completeness test |
| PC-003 | The deterministic policy boundary produces the same outcome and reason for the same complete validated input, authoritative state and policy revision | Deterministic policy regression test |
| PC-004 | Contextual exceptions are not automatically treated as violations | Negative test fixtures |
| PC-005 | AI output cannot directly invoke enforcement actions | Structural boundary test |
| PC-006 | High-severity cases are routed to human review | Severity-routing test |
| PC-007 | AI timeout or invalid output cannot cause automatic approval or rejection | Fault-injection test |
| PC-008 | Every consequential decision has an attributable audit record | Audit completeness test |
| PC-009 | A human moderator can review and record a decision correction | Review workflow integration test |
| PC-010 | Policy and prompt revisions are evaluated against a fixed test corpus | Semantic evaluation gate |

These criteria define the initial policy verification scope. LLM classification quality is evaluated separately against a fixed corpus under REQ-QUA-003; repeated LLM output is not evidence of deterministic policy-engine behavior. Quantitative model-accuracy and latency thresholds must be taken from the approved requirements registry and evaluation plan rather than invented by this policy document.

---

# 11. Policy Limitations

Version 1.0 has the following limitations:

1. The policy is primarily designed for text-based moderation.
2. It does not provide a complete legal determination of whether content is unlawful.
3. It does not guarantee that AI can accurately infer user intent.
4. It does not cover every possible cultural or linguistic context.
5. It does not implement a complete appeal workflow.
6. It does not define a universal penalty schedule for every account violation.
7. It does not replace human judgment in high-risk or ambiguous cases.

These limitations must be considered when interpreting evaluation results.

---

# 12. Policy Revision and Governance

This document follows a version-controlled revision process.

| Version | Date | Changes | Status |
|---|---|---|---|
| 1.0 | 2026-11-17 | Initial policy categories, severity levels, decision framework, enforcement guidance, and audit requirements | Draft |
| 1.0-draft.2 | 2026-11-19 | Aligned outcomes and severity routing with ADR-001; clarified MVP boundaries, atomic commit semantics, contextual examples, escalation criteria and deterministic-policy scope following Issue #48 review | Draft — cross-review pending |
| 1.1 | TBD | Incorporate initial user interview findings | Planned |
| 2.0 | TBD | Revise policy based on user feedback, moderation evaluation, and team review | Planned |

Policy changes must be reviewed against:

- The requirements registry.
- The traceability matrix.
- Existing test cases.
- The evaluation corpus.
- Relevant architectural constraints.

Changes affecting safety invariants require appropriate testing and human approval.

# 13. References and Research Sources

The initial ContentGuard Community Content Policy was independently drafted using publicly available community moderation guidelines, moderation research, and evaluation resources.

The following materials are used as research references. ContentGuard does not claim ownership of the referenced policies and does not reproduce their full text.

### 13.1 Platform Community Guidelines

1. Discord. *Community Guidelines.*
   https://discord.com/guidelines

2. Reddit. *Reddit Rules.*
   https://redditinc.com/policies/reddit-rules

3. YouTube. *YouTube Community Guidelines.*
   https://support.google.com/youtube/answer/9288567

**End of Document — ContentGuard Community Content Policy v1.0**
