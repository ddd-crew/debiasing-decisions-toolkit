# Debiasing Decisions Toolkit

> A community toolkit of checklists, canvases, and facilitation tools to help you recognise and counter cognitive bias in design, architecture, and leadership decisions.

Created by **Evelyn van Kelle**,  **Gien Verschatse**, and **Kenny Schwegler**, co-authors of [Collaborative Software Design](https://collaborative-software-design.com) (Manning, 2024).

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

## Why this toolkit exists

Every significant decision, a bounded context boundary, an architectural style, a hiring choice, a team structure, has a moment where one option *just feels right*. That powerful gut feeling is sometimes a genuinely good signal. But it is also sometimes a cognitive bias in disguise.

Research consistently shows that **awareness of cognitive bias is not enough to counter it**. Simply knowing about anchoring, overconfidence, or status quo bias does not reduce their influence on your decisions. What works is **structured behavioural intervention**: habits and prompts embedded directly into your workflow at the moment a decision is being made.

This toolkit is grounded in two independent research streams that reach the same conclusion:

- Morewedge et al. demonstrated that targeted training interventions significantly reduce the effect of cognitive bias.
- Soll, Milkman & Payne translated this into a practical five-step framework for everyday decision-making.

See: [Choiceology's Guide to Better Decisions](https://www.schwab.com/learn/story/choiceologys-guide-to-better-decisions-with-guests-james-korris-carey-morewedge-jack-soll) and [Outsmart Your Own Biases](https://hbr.org/2015/05/outsmart-your-own-biases) (HBR, 2015).

We adopted their framework and extended it for design, architecture, and technical leadership decisions in the IT industry.

---

## How to use this toolkit

Each tool in this toolkit is **standalone and context-independent**. You do not need to adopt everything — pick what fits your team's current workflow.

The most effective integration point is wherever your team already formalises decisions: Architecture Decision Records, design sessions, planning meetings, hiring panels, or team retrospectives. The goal is to embed the prompts into your existing process rather than adding a separate debiasing step.

Work through the checklist **as a team**, not individually. Cognitive bias is a collective problem as much as a personal one, and the habits work best when they create shared permission to slow down and question a decision together.

---

## What currently exists

| Tool | Description | Format |
|---|---|---|
| [Five-Step Debiasing Checklist](#the-five-step-debiasing-checklist) | A checklist for recognising and countering cognitive bias across design, architecture, and leadership decisions | Markdown (below) |
| [ADR Template Snippet](#adr-template-snippet) | A copy-paste block to embed the debiasing check directly into your Architecture Decision Records | Markdown (below) |

More tools are in development — canvases, facilitation guides, and domain-specific extensions. Contributions are warmly welcomed.

---

## The Five-Step Debiasing Checklist

### 1. Be Decision-Ready

Check that you are in the right mental state to make a good decision.

| Question | Bias addressed |
|---|---|
| Am I / are we deciding under emotional stress? | Myopic Misery → Action Bias |
| Am I / are we defaulting to "keep it as-is" without genuinely evaluating alternatives? | Status Quo Bias |
| Is the perceived cognitive load so high that doing nothing has become the path of least resistance? | Status Quo Bias |

---

### 2. Broaden the Frame

Check that you have explored the full solution space.

| Question | Bias addressed |
|---|---|
| Did we consider *removing* something instead of only adding? | Additive Bias (Subtraction Neglect) |
| Did we explore unconventional uses of existing tools or concepts? | Functional Fixedness (Golden Hammer) |
| Instead of asking "what is this?", did we ask "what is it made of, and what could those parts do?" | Functional Fixedness |
| Did we ask "what does this concept actually *know* and *do*?" when we heard "service", "manager", or "handler"? | Functional Fixedness |

---

### 3. Seek Independent Advice

Check that the information you acted on was genuinely diverse.

| Question | Bias addressed |
|---|---|
| Did we get input from people who formed their opinions *independently* of each other? | Correlation Neglect |
| Can we trace this decision back to multiple *independent* sources, or are we following repeated echoes of a single opinion? | Correlation Neglect |
| Did we genuinely consider contradicting views rather than dismissing them? | Overconfidence Bias |
| Is this option driven by overconfidence in our own skills, abilities, or expertise? | Overconfidence Bias |
| If a junior team member had suggested this, what questions would we ask? | Authority Bias |

---

### 4. Test Your Assumptions

Check that you have stress-tested the decision against reality.

| Question | Bias addressed |
|---|---|
| Are we accepting this because of *who* or *what* suggested it, rather than evaluating it on its merits? (AI, senior architect, vendor) | Authority Bias |
| What problem was this pattern, tool, or technology *designed* to solve — and do we actually have that problem? | Authority Bias |
| What is our plan when this goes wrong? *(Not if — when.)* | Illusion of Control |
| Are we designing around confidence rather than designing for failure? | Illusion of Control |

---

### 5. Establish Simple Rules

Check that your decision process was proportional to what is actually at stake.

| Question | Bias addressed |
|---|---|
| Is this a Two-Way Door? If it is reversible, have we delegated it rather than seeking group consensus? | Law of Triviality (Bikeshedding) |
| Did we spend time proportional to how hard this decision is to reverse? | Law of Triviality |
| What would make this conversation a waste of time? Have we avoided that? | Law of Triviality |
| Did we check as a group rather than leaving debiasing to individuals alone? | False Consensus Effect |

---

## ADR Template Snippet

Copy this block into the **Decision** section of your ADR:

```markdown
### Debiasing Check

> Before finalising, work through the following as a team.
> Given our current mental state and cognitive load — should we be making this decision today?

**1. Be Decision-Ready**
- [ ] Are we deciding under time pressure or stress? (Myopic Misery)
- [ ] Are we defaulting to "keep it as-is" without evaluating alternatives? (Status Quo Bias)
- [ ] Is cognitive load making inaction the path of least resistance? (Status Quo Bias)

**2. Broaden the Frame**
- [ ] Did we consider removing something instead of only adding? (Additive Bias)
- [ ] Did we explore unconventional uses of existing tools? (Functional Fixedness)
- [ ] Did we ask what existing concepts actually know and do? (Functional Fixedness)

**3. Seek Independent Advice**
- [ ] Did we get input from people who formed opinions independently? (Correlation Neglect)
- [ ] Are we acting on diverse sources or repeated echoes? (Correlation Neglect)
- [ ] Did we genuinely consider contradicting views? (Overconfidence Bias)
- [ ] If a junior suggested this, what questions would we ask? (Authority Bias)

**4. Test Your Assumptions**
- [ ] Are we accepting this because of who/what suggested it vs. its merits? (Authority Bias)
- [ ] What problem was this designed to solve — do we actually have it? (Authority Bias)
- [ ] What is our plan when this goes wrong? (Illusion of Control)

**5. Establish Simple Rules**
- [ ] Is this a Two-Way Door? If so, have we delegated it? (Law of Triviality)
- [ ] Did we spend time proportional to reversibility? (Law of Triviality)
- [ ] What would make this conversation a waste of time? (Law of Triviality)
- [ ] Did the full group check collectively, not just individuals? (False Consensus Effect)
```

---

## Cognitive Biases Reference

| Bias | What it does | How it shows up in decisions |
|---|---|---|
| **Myopic Misery** | Sadness or stress creates short-sighted focus on immediate resolution | Rushing decisions during pressured sprints or incident response |
| **Status Quo Bias** | Strong preference for current state when cognitive load is high | "We've always done it this way" — avoiding refactoring or boundary redesign |
| **Additive Bias** | Defaulting to adding rather than removing when solving problems | Solving every challenge by adding a new service, layer, or process |
| **Functional Fixedness** | Limiting tools and concepts to their traditional use | Always reaching for the same pattern regardless of context (Golden Hammer) |
| **Overconfidence Bias** | More confidence in skills and estimates than data supports | Underestimating complexity, overestimating team familiarity with a technology |
| **Correlation Neglect** | Mistaking frequency of an opinion for its accuracy | Echo chambers in architecture guilds, Slack threads, or pull request reviews |
| **Authority Bias** | Attributing greater accuracy to authority figures or AI | Blindly trusting AI-generated code or senior architect proposals without scrutiny |
| **Illusion of Control** | Overestimating ability to control chance-driven outcomes | Assuming a design will behave as intended under real production conditions |
| **Law of Triviality** | Disproportionate focus on trivial issues while ignoring complex ones | Long debates on naming conventions while system boundaries go unexamined |
| **False Consensus Effect** | Overestimating how widely your views are shared | Assuming the team agrees on an approach without making disagreement safe |

---

## The Core Heuristic

When **"this just feels right"** appears in your decision-making — pause and ask:

> *Is this a genuinely good decision, or a bias in disguise?*

---

## Contributing

This toolkit is a living resource. We actively invite contributions from practitioners across software design, architecture, technical leadership, and beyond.

**What we welcome:**
- Additional debiasing questions from your own practice
- Domain-specific extensions (event-driven systems, AI-assisted development, platform engineering, hiring, team design)
- New tools: canvases, facilitation guides, workshop formats
- Translations
- Experience reports of bias patterns you have observed in the wild

**How to contribute:**
Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

The guiding principle for contributions: **short, habit-forming questions or tools grounded in research or documented practice**. We curate to keep the toolkit usable rather than exhaustive.

---

## References

- Kahneman, D. — *Thinking, Fast and Slow*
- Soll, J., Milkman, K. & Payne, J. — *Outsmart Your Own Biases* (HBR, 2015)
- Morewedge, C. et al. — debiasing training research
- Lerner, J., Li, Y. & Weber, E. — *The Financial Costs of Sadness* (2013)
- Adams, G., Converse, B., Hales, A. & Klotz, L. — *People Systematically Overlook Subtractive Changes* (Nature, 2021)
- McCaffrey, T. — *Innovation Relies on the Obscure* (2012)
- Logg, J., Minson, J. & Moore, D. — *Algorithm Appreciation* (2019)
- Langer, E. — *The Illusion of Control* (1975)
- Enke, B. & Zimmermann, F. — *Correlation Neglect in Belief Formation* (2017)
- van Kelle, E., Verschatse, G. & Baas-Schwegler, K. — [*Collaborative Software Design*](https://collaborative-software-design.com) (Manning, 2024)
- Harmel-Law, A. — *Facilitating Software Architecture* (O'Reilly, 2023)

---

## License

<a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/">
  <img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" />
</a>

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).

**You are free to:**
- Share — copy and redistribute the material in any medium or format
- Adapt — remix, transform, and build upon the material for any purpose, including commercially

**Under the following terms:**
- **Attribution** — You must give appropriate credit to Evelyn van Kelle and Kenny Baas-Schwegler, provide a link to the license, and indicate if changes were made.
- **ShareAlike** — If you remix, transform, or build upon the material, you must distribute your contributions under the same CC-BY-SA 4.0 license.
