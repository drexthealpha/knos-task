# knos-task

A repository for one piece of paid work, made from this template by the "task with no repository" form on the
[Knos](https://github.com/drexthealpha/Knos) site.

What happens here:

1. You open an issue that says what you want built, and add the acceptance files the form made
   (`.knos/acceptance/<issue>/`): pairs of an input and the answer it must get.
2. You fund the issue with a comment, `/knos fund <amount> tests`. The money goes into an escrow on Solana, and the
   terms are fixed at that moment.
3. Anyone opens a pull request that solves it. Knos runs the solution on every recorded input in a sandbox. When every
   answer matches, GitHub signs that it did, and the escrow pays the author. No merge and no decision of yours is
   needed, and nobody can change the terms afterwards.

The two files in `.github/workflows/` are Knos's callers, copied from
[drexthealpha/Knos/examples](https://github.com/drexthealpha/Knos/tree/main/examples). Their comments say what each
trigger does and what the file can and cannot do in this repository. They need no secret.

On Solana devnet today, in test USDC.
