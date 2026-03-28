---
title: "About LocoLab"
---

LocoLab is an applied AI research lab at Curtin University's School of Marketing and Management. We study what local AI can actually do on modest hardware -- and build tools that put that capability in the hands of educators, students, and organisations that can't or won't send their data to the cloud.

The work is deliberate. The hardware is secondhand. The models are small. The questions are serious.

---

## Where This Started

It didn't start with a research grant or a GPU cluster. It started with a restriction.

Curtin University, like many institutions, prohibited the use of frontier cloud AI models for teaching and assessment. No ChatGPT. No Claude. No API calls with student data. The reasons are legitimate: student privacy obligations, data sovereignty requirements, ethics approvals that don't contemplate third-party processing, and the straightforward governance problem of sending assessment work to a commercial provider whose data practices you don't fully control.

The obvious response was to stop. The response that produced LocoLab was to build alternatives.

The first outputs were privacy-first desktop applications -- local, offline, built around Ollama for inference, with BYOK (Bring Your Own Key) options for users who wanted to make their own choices about cloud access. No data leaves the machine by default. No institutional exposure. No API costs. The student controls the tool; the institution controls the policy.

Building those tools surfaced something more interesting than a technical solution. Working with small local models -- genuinely constrained, genuinely imprecise compared to frontier alternatives -- forced a rethink of what AI was actually for in an educational context.

The answer became **Conversation, not Delegation**.

---

## Why Local AI Matters

The gap between frontier AI and local AI is widening. GPT-4, Claude, Gemini -- powerful, accessible, and for many users and institutions, unavailable in practice.

The barriers are not always financial. They are often principled:

**Data sovereignty** -- governments, health organisations, and defence-adjacent institutions operate under data residency requirements that prohibit cloud processing of sensitive information regardless of cost. Local inference is not a workaround; it is the only compliant path.

**Student and research privacy** -- assessment submissions, conversation transcripts, interaction logs, and unpublished research findings carry privacy obligations. Many institutional ethics approvals do not contemplate third-party cloud processing. Running inference locally keeps that data on-premises by design.

**Institutional governance** -- an institution that sends student work to a commercial AI provider has made a policy decision with legal and reputational implications. Local inference makes that decision unnecessary.

**Economic access** -- ongoing API costs are real for individuals, small organisations, and institutions in lower-income contexts. Local inference removes the per-query cost entirely once hardware is in place.

We are not mapping the floor of what AI can do because we cannot afford the ceiling. We are mapping the floor because most people live there, and nobody is documenting it honestly.

---

## The Projects

| Project | Domain | Site |
|---------|--------|------|
| **LocoLLM** | Routed swarm of tiny specialist models | [locollm.org](https://locollm.org) |
| **LocoBench** | VRAM tier benchmarking across GPU generations | [locobench.org](https://locobench.org) |
| **LocoConvoy** | Multi-GPU parallelism on consumer hardware | [lococonvoy.org](https://lococonvoy.org) |
| **LocoEnsayo** | Authentic rehearsal environments for education | [locoensayo.org](https://locoensayo.org) |
| **LocoAgente** | Agentic scaffolding for small local models | [locoagente.org](https://locoagente.org) |
| **LocoPuente** | Student-facing local AI deployment layer | [locopuente.org](https://locopuente.org) |

---

## The Philosophy

The institutional restriction that started this was not an obstacle. It was a clarification.

It forced the question: what is AI actually for in an education context? The answer -- amplifying thinking, not replacing it -- turned out to be better served by local small models than by frontier alternatives. Not because the small models are better. Because the constraint produced a better question.

Constraints surface optimisations that comfortable resources conceal. Secondhand hardware, small models, and honest baselines produce research that the A100 crowd is not doing -- not because they could not, but because the question only becomes visible from the floor.

We are not claiming small models match frontier models. We are claiming that for a large class of genuinely useful tasks -- educational brainstorming, professional rehearsal, domain-specific assistance, privacy-sensitive applications -- they are sufficient, local, and free to run. Documenting that honestly, at scale, and reproducibly is a contribution worth making.

Loco by name. Serious by intent.

---

*LocoLab -- Information Systems, School of Marketing and Management, Curtin University, Perth, Western Australia.*
