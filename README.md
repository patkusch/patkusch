
**I build the checks that stop AI agents doing what a bank would not allow, and I publish the experiments that failed as readily as the ones that worked.**

Most of what I build sits underneath AI agents: keeping their work safe when they crash,
checking that the notes they rely on are still true, and setting limits on what they may
do without asking a person first. I spent years delivering change inside banks, which is
where I learned that the failures that hurt are the quiet ones.

Everything here is public, free to reuse (MIT unless the repo says otherwise), and runs
from a fresh download.

---

### Selected work

| | What it is | Why it matters |
|---|---|---|
| **[apiary](https://github.com/patkusch/apiary)** | Keeps a team of AI agents working when one of them crashes | A worker that died used to take its job with it. Now the job goes to another worker, is retried a limited number of times, and is parked for a person if it keeps failing. |
| **[acta](https://github.com/patkusch/acta)** | A record of what an agent did that it cannot rewrite | A logbook the driver can write in but cannot tear pages out of, with an honest list of which tricks it catches and which it cannot. |
| **[cresco](https://github.com/patkusch/cresco)** | A radar for which tech skills employers will want next | Every prediction is written down with a date and later checked against what actually happened, misses published alongside hits. Six years of real job adverts behind it. |
| **[kontext](https://github.com/patkusch/kontext)** | Tells you which of your project notes are out of date | Compares each note with the code it describes and when each last changed, so nobody trusts a note that stopped being true. |
| **[remit](https://github.com/patkusch/remit)** | Rules for how much an AI agent may do on its own | Asks how much damage one action could do before it is allowed unattended, mapped onto the rulebooks banks and EU regulators actually use. |
| **[aurora](https://github.com/patkusch/aurora)** | Finds where two approved documents contradict each other | Two design documents, both signed off weeks apart, cannot both be true. It finds the clash in seconds and points at the exact lines. |
| **[hazlog](https://github.com/patkusch/hazlog)** | The same, for hospital IT safety | Catches contradictions that could harm a patient, and keeps patient data on site: only single words ever leave for the cloud model. |

---

### Things I got wrong, in public

This is the part I'd actually point a reviewer at. Anyone can publish the run that worked.

- **[A finding that died as the data grew.](https://github.com/patkusch/cresco#a-finding-that-died-as-the-data-grew)**
  I thought Wikipedia page views predicted hiring six months ahead, and the numbers looked
  convincing enough to go in the README. Then I fixed a bug that had been cutting off the
  job-advert history, added more years of data, and watched the effect vanish. The
  retraction is in the README with the table showing it disappear, because a project about
  grading its own predictions doesn't get to quietly delete one.

- **[Measuring whether my own instrument works.](https://github.com/patkusch/remit#why-this-exists)**
  I asked four people, separately and without the answers, to classify eight agent failures
  using my manual. They agreed with each other far more than chance would allow (κ = 0.83,
  where 0.61 counts as good). They also found two mistakes in the manual. Both are fixed,
  and both are written up.

- **[Separating what I wrote from what I inherited.](https://github.com/patkusch/apiary#what-is-inherited-and-what-is-not)**
  apiary started as a copy of someone else's project. Its test suite is 3,763 tests and
  green; 3,691 of them came with the copy and I did not write them. The badges say so, with
  the file and line counts to back it up.

---

### Background

Management consultant. I help banks and other regulated companies change how they work:
working out what the business needs, delivering the product, running large programmes.
Knowing the rulebooks (DORA, the EU AI Act, NIST's AI risk framework, ISO 42001) is why
the governance work above is grounded rather than theoretical.

