
**I build agentic systems for regulated environments — and I publish the findings that didn't hold up.**

Most of what I build is infrastructure for AI agents: making them durable when they crash,
giving them context that can prove it isn't stale, and governing what they're allowed to do
without asking anyone. I come at it from a career delivering change inside banks, which is
mostly where I learned that the interesting failures are the silent ones.

Everything here is public, MIT, and runs from a clean clone.

---

### Selected work

| | What it is | Why it might interest you |
|---|---|---|
| **[apiary](https://github.com/patkusch/apiary)** | Durable multi-agent orchestration | A crashed worker used to lose its task with no lease, no attempt counter and no requeue path. Replaced the prose instruction telling an LLM to clean up afterwards with an actual state machine — leases, bounded retries, a real terminal state. |
| **[cresco](https://github.com/patkusch/cresco)** | Skill-demand radar that grades its own predictions | Writes every verdict down as a dated, falsifiable claim, then publishes its own hit rate — including the calls it got wrong. 22 months of real hiring data, six sources, weighted so chatter can't impersonate demand. |
| **[kontext](https://github.com/patkusch/kontext)** | Give your markdown a lifecycle | A document is a *claim about code*, and git can check it. Proves staleness from commit history with no LLM in the verdict path, so CI can gate on it. |
| **[remit](https://github.com/patkusch/remit)** | Agentic skills framework for AI governance | Existing frameworks ask whether a model is fair. None ask how large a single action's blast radius is. Autonomy tiers and a diagnostic manual over EU AI Act, NIST AI RMF, ISO 42001 and DORA. |
| **[aurora](https://github.com/patkusch/aurora)** | Cross-document requirements conflict engine | Two design documents, both approved, five weeks apart, mutually exclusive. Nobody noticed, because nobody reads every document. Finds it in 30 seconds and cites both lines. |

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

- Or open an issue on any repo above. Bug reports and disagreement both welcome — the
  repos are built to be argued with.
