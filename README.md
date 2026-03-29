# Drakos

**Full-pipeline FFXIV automation: from raw materials to market board listings, handled as one operation.**

Drakos is a Dalamud plugin for Final Fantasy XIV that treats crafting, gathering, and selling as a single integrated pipeline rather than three separate tools. Tell it what you want to end up with, and it figures out what to gather, what to craft, and where to sell.

## Orchestration

Drakos operates on *orders*: "I need 40 HQ Integral Armguards of Casting listed on the market board." From that, it:

- Expands the order into a full material tree (intermediates, sub-combines, raw materials)
- Checks your inventory and retainers for what you already have
- Plans gathering routes across nodes, timed nodes, and scrip exchanges
- Solves crafting rotations per recipe, per character stats
- Executes the full chain in dependency order
- Lists the finished product and manages undercuts

The best part is, you don't need to install a million plugins to get everything working together. Other than vnavmesh, Drakos has no other dependency.

## Capabilities

### Gathering
- Automated route execution across regular, timed, and ephemeral nodes
- GP-optimal yield solving: Drakos calculates the best ability sequence for your stats, not a static rotation or heuristics.
- State-of-the-art collectable gathering with quality target optimization
- Multi-zone optimization for gatherer scrip farming

### Crafting
- Per-recipe rotation solving tuned to your exact stats and buffs
- Automatic consumable management (food, potions)
- Condition-aware: Drakos uses an optimized version of raphael-xiv that computes the optimal solution on the fly.

### Market Board
- Automated purchasing across items and quantities with world travel
- Undercut monitoring and repricing
- Market intelligence: estimate the profit per unit time cost of each item you sell.
- [PLANNED] Demand estimation of market

### Orchestration
- Order-based planning: just specify end goals, not individual steps. Drakos automatically figures out what blocks what.
- Orchestration-level optimizer: Drakos uses multiple solvers to optimize sub-task scheduling to minimize the total time taken to complete the tasks.
- Full material tree expansion with inventory netting
- Automatic inventory management
- Automatic scrip exchange
- Retainer management hooks
- Automatic repairs

### Interface
- External GUI: monitor and control outside the game overlay
- API access for custom integrations

### Bayesian Layer
- Drakos learns by doing: it updates its priors about travel speed, yield curves, and is tightly integrated with the solvers.
- [PLANNED] Multi-armed bandit execution layer to more aggressively map out the optimal policies.

## Current Status

Drakos is in closed alpha within our team and is not yet publicly available. If you're interested in early access or want to follow progress, check [drakos.gg](https://drakos.gg) or reach out at support@drakos.gg. We expect to begin open beta in *May 2026*.

## FAQ

**How is this different from using Artisan + GBR or GBR Vulcan?**
Drakos doesn't compete with them on individual features. It replaces the manual coordination layer between them. Instead of running a gathering session, checking your inventory, switching to crafting, then posting on the market board, Drakos treats the full chain as one operation. It also provides QoL hooks like automatically storing items on a retainer when your inventory gets full.

**How is this different from Lisbeth?**
Drakos runs as a native Dalamud plugin and uses customized solvers that are more efficient than Lisbeth's. Many of Lisbeth's current features are planned in the roadmap.

**Is this a bot?**
Drakos automates in-game actions. Use it at your own risk.

**What jobs/classes are supported?**
All Disciples of the Hand (crafters) and Miner/Botanist.

**Does it work with the current patch?**
Drakos is being developed against the current patch cycle and will be kept up to date.

## Roadmap

[April 2026]

- Combat and FATE farming for materials
- Fisher, except big fishing
- Level DoH/DoL to 100

[May 2026]

- Cosmic exploration
- Rapid expert recipe solver