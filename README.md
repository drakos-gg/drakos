<div align="center">

<a href="https://drakos.gg/"><img src="assets/hero.webp" width="880" alt="Drakos, an FFXIV crafting bot. Tell me what you want."></a>

<a href="https://drakos.gg/installation/"><img src="assets/btn-get-started.png" height="56" alt="Get started"></a><a href="https://www.youtube.com/watch?v=ZSbmGxxZPAw"><img src="assets/btn-demo.png" height="56" alt="Watch demo"></a><a href="https://drakos.gg/features/"><img src="assets/btn-features.png" height="56" alt="Features"></a><a href="https://drakos.gg/pricing/"><img src="assets/btn-pricing.png" height="56" alt="Pricing"></a><a href="https://discord.gg/sgKnHh8CRd"><img src="assets/btn-discord.png" height="56" alt="Discord"></a>

</div>

# Drakos, an FFXIV crafting bot

Drakos is an [FFXIV crafting bot](https://drakos.gg/ffxiv-crafting-bot/). It runs as a Dalamud plugin for Final Fantasy XIV. Add the items you want to an order, and Drakos works out what to craft, gather, and buy, then does the work.

<a href="https://www.youtube.com/watch?v=ZSbmGxxZPAw"><img src="assets/demo-orders.webp" width="880" alt="Watch the Drakos Orders Demo on YouTube"></a>

<p align="center"><a href="https://drakos.gg/ffxiv-crafting-bot/"><img src="assets/btn-crafting-bot.png" height="56" alt="About the crafting bot"></a><a href="https://drakos.gg/ffxiv-undercutting-bot/"><img src="assets/btn-undercutting-bot.png" height="56" alt="About the undercutting bot"></a><a href="https://drakos.gg/updates/"><img src="assets/btn-updates.png" height="56" alt="Changelog"></a></p>

<br>

<img src="assets/h-orders.webp" width="880" alt="Orders">

Drakos plans each order from the finished items you add. It counts the materials you already have, decides what to craft, gather, or buy, and schedules the work around timed nodes and travel. It also works out which intermediates need to be HQ to reach your quality target. You can put orders into groups that run in sequence, and import or export order lists.

<img src="assets/drakos-order-and-plan.gif" width="880" alt="Drakos plans an order for HQ Stuffed Peppers and Hi-Cordials">

<br>

<img src="assets/h-crafting.webp" width="880" alt="Crafting">

Drakos solves a rotation for your stats, starting quality, and HQ or collectability target, and adjusts it when the condition turns Good or Excellent. You can preview the rotation before you start. The crafting solver is based on [raphael-rs](https://github.com/KonaeAkira/raphael-rs).

<img src="assets/drakos-hq-craft.gif" width="880" alt="Drakos crafts HQ Stuffed Peppers">

<br>

<img src="assets/h-gathering.webp" width="880" alt="Gathering and fishing">

Drakos travels to regular, timed, and ephemeral nodes and solves a rotation for item yield or collectability from your stats, current GP, and the node's bonuses. For timed scrip routes and aethersand runs, it chooses which nodes to visit and plans GP and cordial use across the run. It also catches supported rod fish and reduces collectables into aethersands.

<br>

<img src="assets/h-retainers.webp" width="880" alt="Retainers and inventory">

Drakos reprices your retainer listings using the undercut amount, price floor, and ceiling you set. A selling watchlist sets the items and quantities to sell, and Drakos posts available stock to retainers with free listing slots. It withdraws gil from your retainers after each undercut round. It can also move items you don't need into your saddlebag, retainers, or FC chest, and it retrieves materials from your saddlebag and retainers when an order needs them.

<br>

<img src="assets/h-market.webp" width="880" alt="Market board and vendors">

Drakos buys materials from market board listings, starting with the lowest prices. You can turn on world hopping and choose which worlds in your data center to shop on. It also buys order materials from NPC vendors and scrip exchanges, and turns in crafted or gathered collectables for scrips.

<img src="assets/drakos-scrip-exchange.gif" width="880" alt="Drakos buys order materials at the Scrip Exchange">

<br>

<img src="assets/h-deliveries.webp" width="880" alt="GC and Custom Deliveries">

Pick the Grand Company Supply and Provisioning requests you want, and Drakos makes what is missing and hands it in.

<img width="880" height="414" alt="Drakos hands in Grand Company supply deliveries" src="https://github.com/user-attachments/assets/1c0765d9-57b0-45b2-9f37-a017da0b747a" />

Drakos also makes and hands in each Custom Deliveries recipient's weekly deliveries.

<img width="880" height="430" alt="Drakos hands in Custom Deliveries" src="https://github.com/user-attachments/assets/db7a3a3e-94ff-4616-8da8-4a0b1d8683ee" />

<br>

<img src="assets/h-combat.webp" width="880" alt="Combat and FATEs">

Drakos farms materials from supported mobs for your orders. FATE farming (beta) raises your Shared FATE ranks or farms bicolor gemstones.

<br>

<img src="assets/h-chores.webp" width="880" alt="Chores during a run">

Optional hooks repair your gear, keep your food, medicine, and FC buffs active, use EXP manuals, and extract materia from fully spiritbonded gear. A restocking list for each character tops up supplies such as food and medicine before every order.

<p align="center"><a href="https://drakos.gg/features/"><img src="assets/btn-all-features.png" height="56" alt="All Drakos features"></a></p>

<br>

<img src="assets/h-how.webp" width="880" alt="How it works">

<img src="assets/how-it-works.png" width="880" alt="The Drakos plugin runs on your PC inside FFXIV and Dalamud. It sends each order to the Drakos planning server, gets a plan back, and checks your license key with the license server.">

1. **You add items to an order.** The Drakos plugin runs inside the game through Dalamud. Drakos.exe is a desktop app that controls the same plugin.
2. **The planning server plans the order.** The plugin sends the order to the Drakos planning server, which answers with what to gather, buy, and craft, and in what order. If the server does not answer, the order waits and carries on once it does.
3. **The plugin does the work on your PC.** It solves each crafting and gathering rotation on your PC and moves your character with [vnavmesh](https://github.com/awgil/ffxiv_navmesh).
4. **The license server checks your key.** While Drakos runs, it checks in with the license server every 10 seconds. If it loses the server for 30 seconds, it finishes its current step and stops.

<br>

<img src="assets/h-start.webp" width="880" alt="Getting started">

1. **Set up Dalamud.** Install XIVLauncher and enable Dalamud.
2. **Install the plugins.** Follow the [installation guide](https://drakos.gg/installation/) to add vnavmesh and Drakos.
3. **Sign in with your key.** Find your license key on your [account page](https://drakos.gg/accounts/). Open `/drakos`, save your key, and sign in.
4. **Add your first order.** Choose what you want to craft or gather, then start the order.

Drakos needs Windows 10 or 11 (64-bit) and the English FFXIV client. The [pricing page](https://drakos.gg/pricing/) lists the current plans.

<p align="center"><a href="https://drakos.gg/installation/"><img src="assets/btn-install-lg.png" height="64" alt="Installation guide"></a><a href="https://drakos.gg/pricing/"><img src="assets/btn-pricing-lg.png" height="64" alt="Pricing"></a><a href="https://drakos.gg/accounts/"><img src="assets/btn-account-lg.png" height="64" alt="Your account"></a></p>

<br>

<img src="assets/h-support.webp" width="880" alt="Support">

Ask questions and report bugs on [Discord](https://discord.gg/sgKnHh8CRd). For account and purchase help, email [support@drakos.gg](mailto:support@drakos.gg). Check [status.drakos.gg](https://status.drakos.gg) for service status.

<p align="center"><a href="https://discord.gg/sgKnHh8CRd"><img src="assets/btn-discord-lg.png" height="64" alt="Join the Discord"></a></p>

<sub>Drakos is not affiliated with or endorsed by Square Enix or the Dalamud team.</sub>
