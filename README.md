
**I build the checks that stop AI agents doing what a bank would not allow, and I publish the experiments that failed as readily as the ones that worked.**

Most of what I build sits underneath AI agents: keeping their work safe when they crash,
checking that the notes they rely on are still true, and setting limits on what they may
do without asking a person first. 

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
| **[assay](https://github.com/patkusch/assay)** | Quick yes/no and pick-one answers from a small AI model on your own laptop, with a number for how sure it is | An agent can ask "is this command dangerous?" in a fraction of a second and get an answer whose confidence can be checked. It says "not sure" when it should, and the scoreboard publishes the tests that showed no benefit. |
| **[aurora](https://github.com/patkusch/aurora)** | Finds where two approved documents contradict each other | Two design documents, both signed off weeks apart, cannot both be true. It finds the clash in seconds and points at the exact lines. |
| **[hazlog](https://github.com/patkusch/hazlog)** | The same, for hospital IT safety | Catches contradictions that could harm a patient, and keeps patient data on site: only single words ever leave for the cloud model. |

---


