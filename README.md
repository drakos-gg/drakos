# Drakos

Drakos runs crafting, gathering, retainers, and the market board. Just tell it what you want. It solves optimal, condition-dependent rotations, undercuts your competitors automatically, and has an intelligent scheduler that optimizes for the best route to completing your orders.

## Crafting

Drakos uses a custom solver, based on [raphael](https://github.com/KonaeAkira/raphael-rs), that takes Excellent and Good procs into account. This makes Drakos much more efficient than all publicly available solvers, as it does not rely on a single static, solved rotation, but adjusts based on procs to speed up your craft.

## Gathering

Drakos comes with multiple gathering solvers to optimize the amount of material it gathers. It solves for all types of nodes, but more importantly dynamically adjusts the GP budget it allocates to different nodes to maximize your efficiency. It doesn't just solve for the best rotation on a single node, but solves for the best *allocation* of time and GP on nodes.

## Orchestration

Drakos comes with an orchestration solver that solves for the optimal sequence of tasks to maximize your efficiency. You can also supply huge orders of items you want to craft and/or gather, and Drakos automatically figures out what it needs to purchase, gather, and craft, including intermediates, to finish the job. Just tell Drakos what you want and it figures out the rest.

## Retainers

Drakos comes with hooks, including automatic undercutting hooks, that lets Drakos check all the items you have listed and undercut your competitors while it's working on your order. It also refreshes ventures, and has the ability to retrieve and store items in retainers when it needs space to craft items.

## Combat

Drakos comes with an efficient combat routine that allows it to grind overworld mobs to fulfill orders. You don't need to separately purchase mob materials!

## Market board

You can also purchase items you need from the market board with Drakos. It hops cross-world, finds the best deals, and is even able to automatically purchase items from the market board for your orders.

## Current Status

Drakos is in closed alpha within our team and is not yet publicly available, as we're working on making sure that we eliminate as many bugs as we can find before our launch. If you're interested in early access or want to follow progress, check [drakos.gg](https://drakos.gg) or reach out at support@drakos.gg. You can also join our Discord at [https://discord.gg/sgKnHh8CRd](https://discord.gg/sgKnHh8CRd).

Note that Drakos is not publicly available, so there is no download link as of now.
