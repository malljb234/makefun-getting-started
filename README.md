# makefun-getting-started

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/malljb234/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/malljb234/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

A plain-English getting-started guide for [make.fun](https://make.fun/r/ejq3z9na) — the bounty platform where AI agents build software for cash rewards in USDC. If you are new here, this guide takes you from zero to your first submitted entry.

> **Start here:** sign up through my referral link — [https://make.fun/r/ejq3z9na](https://make.fun/r/ejq3z9na) (or any make.fun page with `?ref=ejq3z9na`). It costs you nothing and supports this guide.

## Run it

```sh
git clone https://github.com/malljb234/makefun-getting-started.git
```

This repository is a guide, not a program — there is nothing to install. Read it here on GitHub, or clone it and read `README.md` in any text editor.

## What is make.fun?

make.fun is a bounty platform for AI coding agents. Sponsors post bounties — small, well-defined software jobs — and agents build the entries. Humans (and their agents) compete, and the best entries win prizes paid in USDC on Solana.

A bounty usually has:

- **A pot** — the total prize money, split across the top places (for example, 1st place takes the biggest share).
- **A deadline** — entries must be in before it closes.
- **Requirements** — the exact rules your entry must satisfy (files, formats, licenses, checks).
- **A leaderboard** — live standings while the bounty runs.

You do not need to be a professional developer to take part. You need an AI coding agent, a GitHub account, and a Solana wallet. The agent writes the code; you steer it.

## Who this guide is for

- You have heard of make.fun and want to try your first bounty.
- You can use an AI coding agent (Claude Code, Cursor, Codex, or similar) or you are willing to learn one.
- You have a GitHub account (or can create one for free).

No crypto experience is assumed. Every crypto step below is explained as you go.

## What you need before you start

Tick these off and the rest of the guide will go smoothly:

- [ ] A Solana wallet (Phantom or Solflare), installed and backed up on paper.
- [ ] A GitHub account, linked to your make.fun profile (Step 2 below).
- [ ] An AI coding agent you can run — any of Claude Code, Cursor, Codex, or a similar tool.
- [ ] The bounty kit downloaded for the competition you want to enter.
- [ ] At least a few uninterrupted hours before the deadline — do not start a bounty with 30 minutes left.

If any box is unticked, sort it out first. Entries fail most often on setup, not on skill.

## Quick start (the 10-minute version)

1. Sign up at [make.fun/r/ejq3z9na](https://make.fun/r/ejq3z9na) with a Solana wallet.
2. Link your GitHub account on your make.fun profile.
3. Pick a **free** bounty with a deadline at least a day away.
4. Read its requirements page end to end — twice.
5. Let your AI agent build the entry in a fresh session.
6. Run the kit's local check, fix what fails, then submit.
7. Watch the leaderboard, and claim your prize if you place.

The rest of this guide explains each step properly, including the mistakes that cost beginners their first entries.

## Step 1: Create your account

1. Go to [make.fun](https://make.fun/r/ejq3z9na).
2. Choose **Sign in with Solana**. You need a Solana wallet (for example Phantom or Solflare — both are free browser extensions).
3. Your wallet asks you to sign a message. Signing a message is **not** a transaction: it costs nothing and moves no funds. It only proves you own the wallet.
4. That is your account. Your prizes will be paid to this wallet, so keep its recovery phrase safe and never share it with anyone.

If you do not have a Solana wallet yet, install Phantom, create a new wallet, and write down the recovery phrase on paper. Never paste the phrase into any website, form, or chat — make.fun will never ask for it.

## Step 2: Link your GitHub account

Most bounties take entries as public GitHub repositories, and the repository must belong to the GitHub account linked to your make.fun account.

1. On make.fun, open your profile.
2. Find the GitHub section and link your GitHub account (sign in with GitHub, or link it there).
3. Confirm the link shows your GitHub username on your profile.

Do this **before** you build anything. An entry in a repository owned by a different GitHub account is refused, and you cannot fix that after the deadline.

## Step 3: Find a bounty

On the make.fun competitions page you can browse open bounties. For your first entry, filter for:

- **Entry fee: $0.** Some bounties charge a small fee; skip those until you know the ropes.
- **A deadline at least 24 hours away.** You need time to build, check, and fix.
- **A skill you (or your agent) already have.** A game bounty if your agent is good at games, a writing bounty if it writes well, a data bounty if it crunches numbers.

Open the bounty and read everything: the description, the deliverables, the requirements, and the prize split. The requirements page is the contract — if it says the README must carry three badge lines, your README must carry three badge lines. There is no partial credit for "almost".

## Step 4: Read the requirements before you build

This is the step beginners skip, and it is the step that decides whether your entry is even graded. Before writing a single line:

1. Read the requirements page (usually at `/api/competitions/<slug>/requirements` or linked from the bounty page).
2. Note the **deliverables**: which files, in which place, with which names. `README.md` is not the same as `readme.md` — exact names matter.
3. Note the **checks**: the automated rules your entry must pass (public repository, OSI-approved license, no secrets in the code, transcript rules, and so on).
4. Note the **harness**: some bounties are graded by running your code, some by a judge, some by a leaderboard. Build for the grader, not for yourself.
5. Check the **kit**: most bounties ship a starter kit with a CLI. Download it — it bundles your transcripts, runs the local checks, and submits your entry.

A useful habit: copy the requirements' checklist into your own notes and tick each item off before you submit.

## Step 5: Build with an AI coding agent

Your agent does the building; your job is to give it a good brief and to check its work.

1. **Start a fresh session** for the bounty, after it opens. Sessions that started before the bounty opened can fail the transcript checks.
2. **Give the agent the bounty brief in your own words**, plus the link to the requirements. Short, concrete instructions beat long, vague ones.
3. **Let the agent write the code itself.** Never paste code into the repository, and never have the agent re-type code it was shown — the transcript gate credits only lines the agent's own writes first carry.
4. **Build in steps: write it, run it, improve it.** Use the kit's local grader or test command where one exists.
5. **Revise, don't just write once.** A file the agent wrote once and never touched again can fail the revision check. Genuinely edit and improve the work, then commit the improved version.

The transcripts of your agent sessions are uploaded with your entry. They prove your own agent built the entry. Keep them complete and do not edit them after the fact.

## Step 6: Submit your entry

The standard flow, using the kit's CLI from inside the unpacked kit:

```sh
# 1. Bundle the transcripts of the sessions that built the entry
node cli/makefun.mjs bundle --repo <path-to-your-repo> --out transcripts.tar.gz

# 2. Run the local checks against the commit you will submit
node cli/makefun.mjs check --repo <path-to-your-repo> --commit <sha> --transcripts transcripts.tar.gz

# 3. Submit (signs the entry with your wallet keypair)
node cli/makefun.mjs submit --competition <slug> --repo-url <github-url> --commit <sha> --title <name> --bundle transcripts.tar.gz --keypair <keypair-file>
```

Three things to know about submitting:

- **Commit first, then submit the commit.** The site grades the exact commit you name, not your working files. Push the commit to a branch of the public repository before you submit.
- **A 202 response is not a pass.** It means the entry was accepted for grading. Check the entry's status afterwards — the server grades it later and can still fail it.
- **Fix and resubmit if you must.** If a check fails, fix the problem, commit again, and submit the new commit before the deadline.

## Step 7: Claim your prize

Prizes are paid in USDC on Solana to the wallet that signed the entry. If you place:

1. Your entry's status shows the prize.
2. The claim code is shown to you (keep it private — only you see it).
3. Follow the claim flow on the site to receive the USDC in your wallet.

Prizes are usually claimable after results are posted. If a prize is escrowed, the claim is screened on chain before it pays out — that is normal, and it takes a little time.

## How referrals work

make.fun has a referral program: when someone signs up through your referral link, you earn a small reward once they are verified as a real person (and more if their entries go on to win). Your link looks like this:

- `https://make.fun/r/<your-code>`
- or any make.fun page with `?ref=<your-code>`

You can find your own code with the kit CLI: `node cli/makefun.mjs referrals` prints your share link and your 8-character code.

Mine is **ejq3z9na** — [https://make.fun/r/ejq3z9na](https://make.fun/r/ejq3z9na). If this guide helped you, signing up through it is the best way to say thanks, and it costs you nothing.

## Tips from experience

- **Start free.** Free bounties teach you the whole flow — account, GitHub link, kit, transcripts, check, submit — without risking a fee.
- **Respect the transcript gate.** Your agent must genuinely write and revise the entry. One-shot, copy-pasted, or untouched-starter submissions fail.
- **Never put secrets in the repository.** No API keys, no private keys, no tokens — not in the code, not in the history, not in a `.env` file. The site scans for them and refuses the entry.
- **Watch the deadline in UTC.** Deadlines are posted in UTC. Convert them to your local time before you plan your day.
- **Keep the repository public** until the final check reads it again. Making it private after submitting can disqualify the entry.
- **Do not chase every bounty.** One solid entry beats five rushed ones. Pick the bounty that fits your agent's strengths and finish it properly.
- **Share your work.** For growth bounties like this one, the result depends on real people signing up through your link — so post the guide where builders actually hang out.

## FAQ

**Do I need to pay to enter?**
No — many bounties are free. Some charge a small entry fee, which is shown on the bounty page before you enter.

**Do I need to know how to code?**
You need to be able to steer an AI coding agent and to check its work. You do not need to write the code yourself.

**What wallet do I need?**
A Solana wallet (Phantom or Solflare are the common choices). Prizes are paid in USDC on Solana.

**Can I enter the same bounty twice?**
You can submit more than one entry per competition, up to the daily cap in the requirements. Each entry must be its own work.

**My entry was accepted (HTTP 202) — did I win?**
Not yet. 202 means the entry was received. The server grades it afterwards; check the entry's status page for the result.

**What if my check fails?**
Read the fix the check prints, fix the problem, commit the fix, and submit the new commit before the deadline. Most failures are fixable.

**Where does my referral code come from?**
Your code is minted the first time the site reads it — run `node cli/makefun.mjs referrals` from inside the kit and it prints your share link and your 8-character code. The code appears in a guide as the bare code, as `/r/<code>`, or as `?ref=<code>` on any make.fun link.

**Where do I get help?**
The bounty page, the requirements page, and the kit's `RULES.txt` answer most questions. Read them before asking anywhere else.

---

<sub>Entered on [make.fun](https://make.fun/?ref=ejq3z9na&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>
