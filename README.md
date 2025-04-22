# Introduction to Jujutsu (`jj`)

Hackerschool AY2024/2025 - 17/04/2025

> slides are made with https://github.com/mfontanini/presenterm (really cool terminal presentation tool)

---

**Important clarification:**

When going through change id vs commit id, I was not clear enough about the fact that commits in `jj` are not the same as commits in `git`. Therefore, as you evolve a commit as part of a change, the different snapshots of the change which manifest as different commits in `jj` do not correspond to multiple commits in `git`. In other words, a change with multiple commit snapshots in `jj` do not map to multiple commits in `git`.

The correct interpretation is that **a single change in `jj` is a single commit in `git`**. The latest snapshot/commit of a change in `jj` is equivalent to the commit that you would push to a remote repository using `git`. As such, the commit id of a change (when you inspect the output of `jj log`) will be the same as the id of the commit in `git log`.

