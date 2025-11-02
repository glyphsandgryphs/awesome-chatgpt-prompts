# Base 44 Prompt Library

This guide curates high-signal prompt patterns for Base 44, focusing on collaborative prompt creation, publishing, and iteration. The structure is designed so prompts can be parsed into discrete fields inside the Base 44 app while remaining copy/paste friendly for AI chat interfaces.

## Recommended Prompt Schema

Each prompt follows the same ordered blocks to ensure consistency:

| Block | Description | Example Guidance |
| --- | --- | --- |
| **Role & Voice** | Who the model should impersonate and how it should sound. | `Role: You are the Base 44 knowledge concierge with a warm, expert tone.` |
| **Primary Objective** | The single most important outcome for the response. | `Objective: Deliver a launch-ready announcement plan.` |
| **Context Inputs** | Up to five bullet facts the model must consider. | `Context:\n- Feature ships to 5K beta users next week` |
| **Constraints** | Non-negotiable rules like length, compliance, or style. | `Constraints: Keep copy under 200 words; highlight onchain benefits.` |
| **Output Format** | Structured layout or headings for the reply. | `Output Format: markdown checklist with emoji bullets.` |
| **Quality Bar** | Optional polish requirements or review checklist. | `Quality Bar: Confirm every CTA links to a Base 44 workspace.` |

> **Tip:** Prefix each block with a bold label so Base 44 can surface them as editable fields inside the prompt composer.

## Prompt Templates by Use Case

### 1. Creator Onboarding Flow

```
**Role & Voice:** You are the Base 44 creator success coach with an encouraging mentor tone.
**Primary Objective:** Produce a step-by-step onboarding sequence for a new prompt curator joining Base 44.
**Context Inputs:**
- The curator is migrating a Notion prompt database with 120 entries.
- Base 44 supports CSV uploads, version history, and collaborative annotations.
- The curator's audience focuses on growth marketing teams.
**Constraints:** Sequence must include milestones for day 1, day 3, and day 7 and highlight metrics the curator should track.
**Output Format:** Markdown table with columns `Milestone`, `Owner`, `Checklist`, `Success Metric`.
**Quality Bar:** Ensure every milestone references a Base 44-native feature (workspaces, tags, analytics, or publishing).
```

### 2. Prompt Review & QA Checklist

```
**Role & Voice:** Act as the Base 44 prompt quality lead with a precise, audit-oriented tone.
**Primary Objective:** Create a reusable review checklist for evaluating prompts before they ship to the Base 44 public library.
**Context Inputs:**
- Prompts must support GPT-4o, Claude 3.5, and open-source LLMs.
- Reviewers collaborate asynchronously across three time zones.
- Compliance requires removing sensitive customer data and PII.
**Constraints:** Limit to 8 checklist items and reference Base 44’s "revise and publish" workflow steps.
**Output Format:** Numbered list where each item includes `Action`, `Why it Matters`, and `Status` placeholders.
**Quality Bar:** Include one final gate that links to Base 44’s approval archive for traceability.
```

### 3. Launch Announcement Generator

```
**Role & Voice:** You are the Base 44 comms lead speaking with a confident, inspiring tone.
**Primary Objective:** Draft a multi-channel launch announcement for a new AI prompt collection.
**Context Inputs:**
- Collection name: "Revenue Ops Accelerators".
- Launch partners: Base 44, HubSpot Ventures, and RevOps Live community.
- Key differentiator: pre-built KPI dashboards embedded inside every prompt card.
**Constraints:** Cover email, LinkedIn, and Base 44 in-app notification copy in under 450 total words.
**Output Format:** Markdown document with sections `Email`, `LinkedIn`, `In-App Notification`, each containing headline + body copy + CTA.
**Quality Bar:** Ensure each channel emphasizes measurable outcomes within 30 days of adoption.
```

### 4. Data Insight Summaries

```
**Role & Voice:** Operate as the Base 44 analytics strategist with a crisp, data-first tone.
**Primary Objective:** Translate raw usage metrics into insight-ready summaries for leadership.
**Context Inputs:**
- Metrics available: prompt saves, workspace shares, completion rate, feedback sentiment.
- Executives review reports during Monday standups.
- Leadership cares about retention and network effects.
**Constraints:** Provide exactly three key insights and pair each with a supporting metric trend.
**Output Format:** Markdown bullets formatted as `Insight -> Metric -> Recommended Action`.
**Quality Bar:** Every recommended action must be implementable within one sprint.
```

### 5. Support Escalation Playbook

```
**Role & Voice:** Serve as the Base 44 customer reliability engineer with a calm, empathetic voice.
**Primary Objective:** Draft the escalation playbook for when prompts fail to render in the library UI.
**Context Inputs:**
- Failures often stem from malformed markdown or missing metadata fields.
- Tier 1 support handles the first response within 15 minutes.
- Escalations route to the platform team via Linear tickets.
**Constraints:** Outline a three-tier response ladder and include SLA timers for each handoff.
**Output Format:** Ordered list with sub-bullets detailing `Trigger`, `Immediate Response`, `Owner`, and `Communication Template`.
**Quality Bar:** Provide a fallback communication for notifying enterprise workspaces during prolonged incidents.
```

### 6. Prompt Monetization Canvas

```
**Role & Voice:** Act as the Base 44 revenue strategist with a pragmatic, growth-oriented tone.
**Primary Objective:** Design a monetization canvas for creators selling premium prompt packs.
**Context Inputs:**
- Base 44 offers Stripe Connect payouts and granular usage analytics.
- Audience segments: sales teams, product designers, and legal ops.
- Platform cut: 12% per transaction with volume-based boosts.
**Constraints:** Canvas must cover pricing tiers, bundled assets, and post-purchase nurture flows.
**Output Format:** Markdown table with rows for each segment and columns `Offer`, `Price`, `Value Props`, `Nurture Sequence`, `Success Metric`.
**Quality Bar:** Include at least one upsell mechanic tied to Base 44’s analytics dashboards.
```

### 7. Partner Outreach Sequence

```
**Role & Voice:** You are the Base 44 partnerships lead with a collaborative, opportunity-driven tone.
**Primary Objective:** Generate a 5-touch outreach sequence to onboard ecosystem partners.
**Context Inputs:**
- Target partners: workflow automation platforms with shared customers.
- Base 44 offers co-branded prompt collections and analytics swaps.
- Average partner evaluation cycle lasts 3 weeks.
**Constraints:** Each touch must propose a distinct value exchange and include a time-bound CTA.
**Output Format:** Markdown table with columns `Touch #`, `Channel`, `Message Snapshot`, `CTA`, `Proof Point`.
**Quality Bar:** Ensure at least one touch leverages Base 44 usage benchmarks as social proof.
```

### 8. Internal Prompt Retrospective

```
**Role & Voice:** Function as the Base 44 product operations facilitator with a neutral, reflective tone.
**Primary Objective:** Lead a retrospective for a prompt update sprint.
**Context Inputs:**
- Sprint length: 2 weeks.
- Team: prompt engineers, UX writer, analytics lead.
- Focus: improving prompt discoverability via tagging and semantic search.
**Constraints:** Retrospective must highlight wins, challenges, data signals, and action items.
**Output Format:** Markdown template with sections `What Went Well`, `Challenges`, `Signals`, `Next Sprint Bets`.
**Quality Bar:** Tie every action item to an owner and a measurable leading indicator.
```

### 9. Community Spotlight Builder

```
**Role & Voice:** Take on the Base 44 community storyteller persona with an enthusiastic, authentic tone.
**Primary Objective:** Craft a monthly community spotlight feature for a top creator.
**Context Inputs:**
- Feature includes interview excerpts, top-performing prompts, and impact metrics.
- Community enjoys seeing behind-the-scenes workflows.
- Content is distributed via Base 44 blog and newsletter.
**Constraints:** Keep total length under 600 words and embed three pull quotes.
**Output Format:** Markdown article with sections `Creator Snapshot`, `Workflow Breakdown`, `Impact Metrics`, `Call to Action`.
**Quality Bar:** End with two interactive questions inviting readers to submit their own prompts.
```

### 10. Ethical Review Guardrails

```
**Role & Voice:** Assume the Base 44 responsible AI officer role with a principled, compliance-focused tone.
**Primary Objective:** Define guardrails for prompts that interact with sensitive customer data.
**Context Inputs:**
- Platform must comply with SOC 2 Type II and GDPR.
- Data can include anonymized CRM notes and ticket summaries.
- Review board meets monthly with legal oversight.
**Constraints:** Provide policy statements plus enforcement actions for violations.
**Output Format:** Two-part Markdown list: `Policy Principles` followed by `Enforcement Steps`.
**Quality Bar:** Reference Base 44’s audit logging and approval workflows to illustrate accountability.
```

## Implementation Notes for Base 44

1. **Tagging:** Convert each use case header into a Base 44 tag (e.g., `Creator Success`, `Analytics`, `Compliance`).
2. **Versioning:** Store prompts with semantic version numbers (e.g., `v1.0.0`) to signal updates inside Base 44.
3. **Localization:** Add a localized copy field so translators can reuse the same scaffold without rewriting constraints.
4. **Metadata:** Capture author, last updated timestamp, and model compatibility within Base 44’s metadata panel.

These examples provide consistent structure while covering the full lifecycle of prompt creation, distribution, governance, and revenue on Base 44.
