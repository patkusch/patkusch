
**I build agentic systems for regulated environments — and I publish the findings that didn't hold up.**

Most of what I build is infrastructure for AI agents: making them durable when they crash,
giving them context that can prove it isn't stale, and governing what they're allowed to do
without asking anyone. I come at it from a career delivering change inside banks, which is
mostly where I learned that the interesting failures are the silent ones.

Everything here is public, MIT unless the repo says otherwise, and runs from a clean clone.

---

### Selected work

| | What it is | Why it matters |
|---|---|---|
| **[apiary](https://github.com/patkusch/apiary)** | Durable multi-agent orchestration | A crashed worker no longer loses its task: leases, bounded retries and a real terminal state, in code rather than in a prompt. |
| **[acta](https://github.com/patkusch/acta)** | Tamper-evident record of what an agent did | A record of everything an agent did that the agent cannot quietly rewrite afterwards, with an honest table of which kinds of tampering it catches and which it cannot. |
| **[cresco](https://github.com/patkusch/cresco)** | Skill-demand radar that grades its own predictions | Every verdict is a dated, falsifiable claim, and it publishes its own hit rate, misses included, over 72 months of real hiring data. |
| **[kontext](https://github.com/patkusch/kontext)** | Give your markdown a lifecycle | A doc is a claim about code, and git checks it: staleness proved from commit history with no LLM in the verdict, so CI can gate on it. |
| **[remit](https://github.com/patkusch/remit)** | Agentic skills framework for AI governance | Asks how large one action's blast radius is, not whether the model is fair: autonomy tiers over EU AI Act, NIST AI RMF, ISO 42001 and DORA. |
| **[aurora](https://github.com/patkusch/aurora)** | Cross-document requirements conflict engine | Finds where two separately approved design documents contradict each other, and cites both lines. |
| **[hazlog](https://github.com/patkusch/hazlog)** | Cross-document clinical hazard detection for DCB0160 | The same idea for clinical safety: a local model reads the corpus, the cloud model only ever sees isolated terms. |

---

### Things I got wrong, in public

This is the part I'd actually point a reviewer at. Anyone can publish the run that worked.

- **[A finding that died as the data grew.](https://github.com/patkusch/cresco#a-finding-that-died-as-the-data-grew)**
  Wikipedia pageviews looked like a six-month leading indicator for hiring — hold-out
  correlation **+0.440**, only 2.3% of shuffled nulls beating it. That number went into the
  README. Then I fixed a bug that had been silently truncating the hiring archive, kept
  extending the data, and watched it collapse. The retraction is in the README with the
  table showing it die, because a project about grading your own predictions doesn't get to
  quietly delete one.

- **[Measuring whether my own instrument works.](https://github.com/patkusch/remit#why-this-exists)**
  A blind panel of four independent assessors, eight traces, ground truth withheld:
  **Fleiss' κ = 0.83** against a conventional bar of 0.61. It also surfaced two defects in
  the manual itself. Both are fixed, and both are written up.

- **[Separating what I wrote from what I inherited.](https://github.com/patkusch/apiary#what-is-inherited-and-what-is-not)**
  apiary is a hard fork. The suite is 3,751 tests and green — 3,691 of those came with the
  upstream import and I didn't write them. The badges say so, with the file and line counts
  behind both.

---

### Background

Management consulting — AI, product, and financial services
transformation. Large-scale change in regulated environments: business analysis, product
delivery, agile ways of working, operating-model modernisation across enterprise
programmes. Regulatory literacy (DORA, EU AI Act, NIST AI RMF, ISO 42001) is why the
governance and financial-services work above is grounded rather than theoretical.


### Get in touch
- Open an issue on any repo above. Bug reports and disagreement both welcome — the
  repos are built to be argued with.
