# Idea Darwin — An Evolution Island for Your Ideas

> You don't lack ideas. You lack a place where they can grow on their own.

You're juggling multiple projects, you just read a great book, you had a fascinating conversation with a friend, a thought pops into your head on the commute home — ideas are scattered across every corner of your life. They don't only show up during scheduled brainstorming sessions. They appear anytime, anywhere — and vanish just as quickly.

**Idea Darwin gives you an island.** Your own evolution island.

Whenever a thought strikes, no matter how rough or fragmented, just toss it onto the island. Zero friction, no need to articulate it perfectly, no need to judge whether it's good. What happens next is the island's job.

## What Happens on the Island?

Your ideas are alive on this island. Like organisms, they follow three core laws of evolution:

### Evolution

Each round, the system identifies the most viable ideas and puts them through structured deep research — filling logical gaps, clarifying paths, identifying risks. Vague ideas become clear. Rough ideas become complete. Survival of the fittest — every idea gets stronger or gets left behind.

### Crossbreeding

Like biological reproduction. The system cross-pollinates your different ideas — a technical approach from work meets an observation from daily life, and they might produce a direction you never imagined. These cross-domain hybrids often yield the most valuable breakthroughs.

### Mutation

Beyond your own ideas, you can introduce "environmental variables" to the island — an industry headline, a theory you just learned, a conversation that struck a chord. These external stimuli trigger mutations in your ideas, spawning entirely new species that continue competing on the island.

## Species Cards: Every Idea Gets Its Own File

Every idea on this island — whether it's an original seed you tossed in, an offspring from crossbreeding, an evolved form after deepening, or a new species born from mutation — gets its own **species card**.

Each card records the idea's core question, full description, lineage, 6-dimensional scores, and change history. Starting from a handful of raw seeds and a few environmental variables, you'll end up with a rich, diverse island of species.

**These cards are what Idea Darwin ultimately produces.**

## You Are the God of This Island

The system runs the evolutionary machinery, but you are always the sovereign. You can:

- **Score and judge** — decide which ideas deserve to keep evolving, which should hibernate
- **Intervene** — change the course of evolution at any moment, wake dormant species, introduce new stimuli
- **Harvest** — take mature idea cards off the island and put them to work in your projects, products, or life

The system only recommends. It never kills an idea without your say. Every life-or-death decision is yours.

## How to Use It

### 1. Toss Your Ideas onto the Island

Create an `ideas.md` file, separate each idea with `##`. Write as rough as you want — a single sentence or a full paragraph, the system will structure it for you.

### 2. Initialize Your Island

```
/idea-darwin init
```

The system generates a species card for each idea, with 6-dimensional scores and a three-layer priority ranking.

### 3. Start Evolving

```
/idea-darwin round
```

Each round, the system automatically runs evolution, crossbreeding, mutation, critique, and validation. After the round, you get a briefing: who rose, who fell, who's a new species, and what needs your decision.

### 4. Add New Ideas and Environmental Variables Anytime

Append new ideas to `ideas.md`, add environmental variables to `stimuli.md`. They'll be absorbed into the next round automatically.

## All Commands

```
/idea-darwin init                    # Build the island
/idea-darwin round                   # Run one evolution round
/idea-darwin round 3                 # Run 3 consecutive rounds
/idea-darwin status                  # View species rankings
/idea-darwin dormant IDEA-0005       # Put a species into hibernation
/idea-darwin wake IDEA-0005          # Wake it up
```

### init Optional Parameters

| Parameter | Description | Default |
|---|---|---|
| `--budget <N>` | Max species to process per round | `12` |
| `--actions <N>` | Max actions per species per round | `2` |
| `--disruption <N>` | Introduce environmental mutation every N rounds | `3` |

## Scoring System

Each idea is scored across 6 dimensions (1-10), aggregated into three priority layers:

| Layer | What It Measures |
|---|---|
| **Survival** | The idea's standalone quality — can it survive? |
| **Development** | Its growth potential — how far can it still evolve? |
| **Priority** | Combined assessment — with freshness and diversity corrections to prevent species convergence |

## Who Is This For?

- **People juggling multiple projects** — let thinking from different domains collide
- **People with lots of ideas that always stall** — give your ideas a place where they won't be forgotten
- **Solo creators and founders** — systematic direction-finding, even as a team of one
- **Researchers** — structured exploration of thesis topics and research directions
- **Anyone who thinks "I have so much in my head but can't sort it out"**

## Installation

```bash
# English version (global)
cp -r en/ ~/.claude/skills/idea-darwin/

# English version (project-level)
cp -r en/ .claude/skills/idea-darwin/
```

## Language Versions

| Version | Path | Description |
|---|---|---|
| English | `en/` | All prompts and templates in English |
| 中文版 | `zh/` | All prompts and templates in Chinese |

## File Structure After Init

```
project/
├── ideas.md          # Your raw ideas (read-only, the system never touches it)
├── config.yaml       # Island configuration and state
├── stimuli.md        # Environmental variables (maintained by you)
├── cards/            # Species cards
├── rounds/           # Evolution round reports
├── reports/          # Species leaderboard
└── graph/            # Species relationship graph
```

## License

MIT
