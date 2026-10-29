
I build open-source tools that watch what AI agents do and stop them doing things nobody agreed to. Each project below says what it can't catch. Where something I tested didn't work, I say so.

Everything here is public, free to reuse (MIT unless the repo says otherwise), and runs
from a fresh download.

---

### Selected work

| | What it is | Why it matters |
|---|---|---|
| **[apiary](https://github.com/patkusch/apiary)** | Keeps a team of AI agents working when one of them crashes | When a worker stops, its job is handed to another worker. Each job is retried a limited number of times, and if it keeps failing it is held for a person to review. |
| **[acta](https://github.com/patkusch/acta)** | A record of what an agent did that it cannot rewrite | A logbook the driver can write in but cannot tear pages out of, with an honest list of which tricks it catches and which it cannot. |
| **[cresco](https://github.com/patkusch/cresco)** | A radar for which tech skills employers will want next | Every prediction is written down with a date and later checked against what actually happened, misses published alongside hits. Six years of real job adverts behind it. |
| **[kontext](https://github.com/patkusch/kontext)** | Tells you which of your project notes are out of date | Compares each note with the code it describes and when each last changed, so nobody trusts a note that stopped being true. |
| **[remit](https://github.com/patkusch/remit)** | Rules for how much an AI agent may do on its own | Asks how much damage one action could do before it is allowed unattended, mapped onto the rulebooks banks and EU regulators actually use. |
| **[assay](https://github.com/patkusch/assay)** | Quick yes/no and pick-one answers from a small AI model on your own laptop, with a number for how sure it is | An agent can ask "is this command dangerous?" in a fraction of a second and get an answer whose confidence can be checked. It says "not sure" when it should, and the scoreboard publishes the tests that showed no benefit. |
| **[aurora](https://github.com/patkusch/aurora)** | Finds where two approved documents contradict each other | Two design documents, both signed off weeks apart, cannot both be true. It finds the clash in seconds and points at the exact lines. |
| **[hazlog](https://github.com/patkusch/hazlog)** | The same, for hospital IT safety | Catches contradictions that could harm a patient, and keeps patient data on site: only single words ever leave for the cloud model. |
| **[examen](https://github.com/patkusch/examen)** | A research agent that checks its own work | Every sentence it writes is checked against the page it cites, by a checker that was first tested on claims with known answers. The best checker that runs on a laptop still fails that test narrowly, and the write-up says so. |

---

### Also built

| | What it does |
|---|---|
| **[proctor](https://github.com/patkusch/proctor)** | Checks whether an AI agent picks the right tool, passes the right arguments, recovers from errors and stays in scope. |
| **[skillgate](https://github.com/patkusch/skillgate)** | Checks an agent skill before you install it: what it can touch, what it claims to do, and whether it changed since you approved it. |
| **[agentsweep](https://github.com/patkusch/agentsweep)** | Shows what your AI agent tools have piled up on your disk and clears it safely. Nothing is deleted, it goes to a folder you can restore from. |
| **[cursus](https://github.com/patkusch/cursus)** | Turns a written process into a Visio flow chart, with the source sentence behind every box. |
| **[specto](https://github.com/patkusch/specto)** | Watches a recorded expert walkthrough of a system and writes down what the system must do. |
| **[carryover](https://github.com/patkusch/carryover)** | Checks that every number, date, amount and name in a text survives translation. |
| **[dayline](https://github.com/patkusch/dayline)** | Writes up your day from your Claude Code sessions and git commits. Runs on your machine. |
| **[versus](https://github.com/patkusch/versus)** | Runs your own tasks on a free AI model on your laptop and on Claude, and shows which jobs the free one can take. On 102 tasks the bigger free model matched Claude on labelling, formatting and following rules, and slipped mostly on maths. |
| **[fewer](https://github.com/patkusch/fewer)** | Reads your own Claude Code history and tells you how many agents you really run at once, how often you jump between them, and how many would do the same work with less jumping. Nothing leaves your machine. |
| **[askwell](https://github.com/patkusch/askwell)** | 33 skills that help an AI agent do a business analyst's work, with checkers that find vague requirements, weak user stories, gaps and processes that lead nowhere. |
| **[dosewise](https://github.com/patkusch/dosewise)** | Ranks data breakages by who is actually affected, so the few that need a person today stand out from the hundreds that can wait. |
| **[whittle](https://github.com/patkusch/whittle)** | 3D models written as small programs: change a setting and the shape rebuilds, and every build is checked before you print it. |
| **[firstgrad](https://github.com/patkusch/firstgrad)** | A tiny neural network library built from scratch, to learn how models learn. It reads small hand-drawn digits it has never seen, with static added, right 94% of the time (guessing would get 10%). |

---
