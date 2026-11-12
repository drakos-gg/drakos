<div align="center">

<a href="https://drakos.gg/"><img src="assets/hero.webp" width="880" alt="Drakos, an FFXIV crafting bot. Tell me what you want."></a>

<a href="https://drakos.gg/installation/"><img src="assets/btn-get-started.png" height="56" alt="Get started"></a><a href="https://www.youtube.com/watch?v=ZSbmGxxZPAw"><img src="assets/btn-demo.png" height="56" alt="Watch demo"></a><a href="https://drakos.gg/features/"><img src="assets/btn-features.png" height="56" alt="Features"></a><a href="https://drakos.gg/pricing/"><img src="assets/btn-pricing.png" height="56" alt="Pricing"></a><a href="https://discord.gg/sgKnHh8CRd"><img src="assets/btn-discord.png" height="56" alt="Discord"></a>

</div>

# Drakos

Drakos [helps you automate crafting, gathering, market board, and far more](https://drakos.gg/ffxiv-crafting-bot/). It runs as a Dalamud plugin for Final Fantasy XIV. Give Drakos the orders, whether it's levequests or GC deliveries or Cosmic tool progress, and Drakos figures out everything for you, at mach speed.

<a href="https://www.youtube.com/watch?v=ZSbmGxxZPAw"><img src="assets/demo-orders.webp" width="880" alt="Watch the Drakos Orders Demo on YouTube"></a>

<p align="center"><a href="https://drakos.gg/ffxiv-crafting-bot/"><img src="assets/btn-crafting-bot.png" height="56" alt="About the crafting bot"></a><a href="https://drakos.gg/ffxiv-undercutting-bot/"><img src="assets/btn-undercutting-bot.png" height="56" alt="About the undercutting bot"></a><a href="https://drakos.gg/updates/"><img src="assets/btn-updates.png" height="56" alt="Changelog"></a></p>

<br>

<img src="assets/h-orders.webp" width="880" alt="Orders">

Drakos comes with an intelligent planner and scheduler that counts the materials you already have, and decides how to schedule the work to fulfill your requests. Unlike traditional planners and schedulers, Drakos's scheduler actually *solves* for an optimal schedule for your tasks. You will see Drakos farming mobs for materials while GP regenerates, then burn that GP on timed nodes.

- **Automatic timed node scheduling**: You don't need to keep an alarm on or write down a schedule with Drakos! Drakos knows which timed nodes it needs to visit to complete your requests. It intelligently creates tasks for those timed nodes and visits them when they spawn.
- **Automatic HQ materials**: Don't have the best gear? Never fear! Drakos automatically calculates how much HQ materials it needs to ensure that you can HQ your orders, every time!
- **Intelligent GP management**: GP is a scarce resource, and Drakos is aware of that! When scheduling, it finds the optimal way to use your GP by forecasting your GP (cordial usage included!) and then solving for the best set of tasks to do to maximize the mileage you get out of your GP.
- **Import and export (including Teamcraft)**: Need to share a long list of orders with a friend? Just export it as a .JSON! Or, you can also import and export orders from Teamcraft, and let Drakos take care of the rest!

<img src="assets/drakos-order-and-plan.gif" width="880" alt="Drakos plans an order for HQ Stuffed Peppers and Hi-Cordials">

<br>

<img src="assets/h-crafting.webp" width="880" alt="Crafting">

Drakos solves a rotation for your stats, starting quality, and HQ or collectability target, and adjusts it when the condition turns Good or Excellent. Our crafting solver, Rapidium, is based on [raphael-rs](https://github.com/KonaeAkira/raphael-rs), with custom optimizations and speedups that make it even better and faster! And, you no longer have to worry about turning in collectables to buy scrip items! Just order that scrip item directly!

- **Guaranteed optimal solution**: Find the *minimum-step* rotation every single time with Rapidium!
- **Automatic caching**: Already solved the rotation before? Drakos automatically caches the results so you don't have to spend time solving it again!
- **Take advantage of Good and Excellent procs**: Rapidium also re-solves when it sees a Good or Excellent proc, shaving more steps from your rotation! This makes crafting faster by around 15% compared to crafting automations that do not take procs into account.
- **Purchase scrip items automatically**: Need a lot of scrip items to make raid food? Don't worry! Just order the food, and Drakos will craft collectables and buy the scrip items itself!

<img src="assets/drakos-hq-craft.gif" width="880" alt="Drakos crafts HQ Stuffed Peppers">

<img src="assets/drakos-scrip-exchange.gif" width="880" alt="Drakos buys order materials at the Scrip Exchange">

<br>

<img src="assets/h-gathering.webp" width="880" alt="Gathering and fishing">

Drakos also solves rotations for gathering! Unlike other automations, Drakos does not rely on hard-coded strategies to gather your items. It solves for item yield, collectability, or aethersand yield based on your stats, current GP, and the node's bonuses. For timed scrip routes and aethersands, it also *chooses* which nodes to visit based on how much it expects that node to provide per GP and time spent. It also catches fish and reduces collectables into aethersands automatically.

- **Automatic aethersand reduction**: You don't need to manually reduce your collectables. Drakos takes care of that automatically!
- **Lightning-fast gathering scrip grinding**: Unlike other automations, Drakos actually weighs the expected benefit from each timed collectable node to visit. Against Lisbeth, [Drakos is 20.8% faster at getting hi-cordials](https://drakos.gg/comparelisbeth/)!
- **Automatic fishing**: You don't need to pilot your character to a spot to fish. Drakos goes to a fishing spot for you automatically!
- **Node bonus-aware**: Drakos dynamically adjusts its rotation based on the node bonuses it sees. It takes advantage of those bonuses, leading to greater yield per hour.
- **Intelligent cordial usage**: Because Drakos's scheduler takes cordial usage into account when forecasting your GP usage, you will find that Drakos seems to always use cordials just in time... that's intended!

<br>

<img src="assets/h-retainers.webp" width="880" alt="Retainers and inventory">

Hate dealing with retainers? Let Drakos deal with them for you. Drakos undercuts your competitors on your retainers, send out ventures as needed, and even use your retainer inventory as space when it needs a lot of space to handle your orders! Drakos's inventory model means you no longer have to worry about cleaning up space before using Drakos! All these options are, of course, manually adjustable in the Settings.

- **Automatic repricing**: Conquer the market board, and let Drakos automatically undercut your competitors on the market board! Set a selling list so that it never goes below a certain price. You can also set this as a scheduled task that triggers every once in a while while you work on orders!
- **Automatic listing**: Need to restock the items you're selling on the market board? Drakos automatically lists anything you put on your selling watchlist on your retainers, whereever that is (should you allow it through the Settings.)
- **Saddlebag usage**: Drakos can automatically use the saddlebag for space and for retrieving materials for crafting.
- **Retainer usage**: Drakos can automatically use retainers for space and for retrieving materials for crafting.
- **FC chest**: Drakos can automatically dump items into your FC chest. **Drakos does not retrieve items from your FC chest for safety reasons.**
- **Automatic deposits and retrievals**: Short on inventory space? Do not worry! Drakos automatically deposits and retrieves items as needed from your retainers and saddlebag! (Note: this feature is not turned on by default for safety reasons.) You can also set which retainers Drakos should have access to and which it should never use for inventory!

<br>

<img src="assets/h-market.webp" width="880" alt="Market board and vendors">

Need tome mats for crafting? Tired of hopping over worlds to find what you need? Let Drakos buy materials for you!

- **Automatic world hopping**: Let Drakos visit other worlds to buy the materials it needs, if it cannot find it on your home world.
- **Price ceilings for purchases**: Set a ceiling, and Drakos will never exceed that amount when buying the items you need.
- **Automatic inventory awareness**: Drakos checks your inventory, saddlebag, and retainers to buy exactly the items you need to restock to a certain amount. (Note: this feature is not turned on by default.)
- (coming soon) **Intelligent world hopping**: Drakos solves for the best worlds to visit by checking prices on Universalis. It takes into account possible staleness and dynamically adjust worlds if the prices it sees are different from what it saw on Universalis!

<br>

<img src="assets/h-deliveries.webp" width="880" alt="GC and Custom Deliveries">

Drakos also comes with a whole gamut of utilities that a player might need when they're crafting!

- **Grand Company deliveries**: Just tell Drakos what you'd like to turn in for the day, and Drakos crafts, gathers, and turns in on your behalf!
- **Custom Deliveries**: Tell Drakos what clients you'd like to rank up with for the week, and Drakos crafts, gathers, and turns in on your behalf! (Note: Drakos currently does not do Custom Delivery quests for you, so you will need to do intro quests by yourself. We're working on that!)
- **Melding**: Supply Drakos with an etro.gg link of melds, and Drakos melds the character for you automatically with the materias you have in your inventory.

<img width="880" height="414" alt="Drakos hands in Grand Company supply deliveries" src="https://github.com/user-attachments/assets/1c0765d9-57b0-45b2-9f37-a017da0b747a" />

Drakos also makes and hands in each Custom Deliveries recipient's weekly deliveries.

<img width="880" height="430" alt="Drakos hands in Custom Deliveries" src="https://github.com/user-attachments/assets/db7a3a3e-94ff-4616-8da8-4a0b1d8683ee" />

<br>

<img src="assets/h-combat.webp" width="880" alt="Combat and FATEs">

Drakos also farms materials for your orders, or use bicolor gemstones if you allow it. You can also use Drakos to grind bicolor gemstones or raise Shared FATE ranks!

- **All combat jobs supported**: You don't need to install a separate combat routine. Drakos has its own internal combat engine that uses powerful spells and skills when farming or doing FATEs.
- **Avoidance logic**: Drakos automatically avoids AoEs when farming mobs or doing FATEs.
- **Chocobo support**: Drakos automatically summons chocobos when farming mobs or doing FATEs.
- **Run away!** Drakos runs away from mobs when it has no way of fighting back, like if you were on a gatherer!
- **Hunt avoidance**: Drakos avoids S, A, and B-rank hunt mobs when farming mobs.
- **Grind bicolor gemstones**: You can set Drakos to grind bicolor gemstones.
- **Raise Shared FATE ranks**: You can set Drakos to raise Shared FATE ranks in various zones.

<br>

<img src="assets/h-chores.webp" width="880" alt="Chores during a run">

Optional hooks repair your gear, and keep your food, medicine, and FC buffs active. You can also set up a restocking list that tops up supplies, like dark matter or medicine, before every order.

- **Stocking list**: Set up a restocking list that you want Drakos to run before every order! Don't worry about needing to buy hi-cordials or Dark Matter anymore!
- **Automatic repairs**: Drakos is able to either use self-repair (if you have the dark matter) or visit a vendor to repair, whenever it needs to.
- **Automatic manuals**: Drakos is able to use manuals for EXP automatically.
- **Materia extraction**: Drakos automatically extract materia from spiritbonded gear while working on orders.
- **FC buff activation and purchases**: Drakos can automatically activate FC buffs or purchase FC buffs while working on orders. (Note: this feature is turned off by default for safety reasons.)
- **Inventory storage**: Drakos can automatically store items in retainers and saddlebags if it is running out on space. (Note: this feature is turned off by default for safety reasons.)
- **Home spot**: You can set a home spot for Drakos to use for crafting and when it has nothing to do. If you set it in your house, it automatically knows to enter your house to craft! (Note: Drakos may struggle to reach certain spots in your house if it's blocked by too much furniture.)
- **Automatic resting**: Drakos can automatically pause and rest for the day after a certain amount of work.
- **Scheduled undercuts and ventures**: While working on orders, you can also let Drakos undercut or manage ventures every X minute that you set.

<p align="center"><a href="https://drakos.gg/features/"><img src="assets/btn-all-features.png" height="56" alt="All Drakos features"></a></p>

<br>

<img src="assets/h-how.webp" width="880" alt="How it works">

<img src="assets/how-it-works.png" width="880" alt="The Drakos plugin runs on your PC inside FFXIV and Dalamud. It sends each order to the Drakos planning server, gets a plan back, and checks your license key with the license server.">

1. **Just add items to your orders.** The Drakos plugin runs inside the game through Dalamud. Drakos.exe is a desktop app that controls the same plugin.
2. **The planning server plans the order.** The plugin sends the order to the Drakos planning server, which answers with what to gather, buy, and craft, and in what order. If the server does not answer, the order waits and carries on once it does.
3. **The plugin does the work on your PC.** It solves each crafting and gathering rotation on your PC and moves your character with [vnavmesh](https://github.com/awgil/ffxiv_navmesh).
4. **The license server checks your key.** While Drakos runs, it checks in with the license server every 10 seconds. If it loses the server for 30 seconds, it finishes its current step and stops.

<br>

<img src="assets/h-start.webp" width="880" alt="Getting started">

1. **Set up Dalamud.** Install XIVLauncher and enable Dalamud.
2. **Install the plugins.** Follow the [installation guide](https://drakos.gg/installation/) to add vnavmesh and Drakos.
3. **Sign in with your key.** Find your license key on your [account page](https://drakos.gg/accounts/). Open `/drakos`, save your key, and sign in.
4. **Add your first order.** Choose what you want to craft or gather, then start the order.

Drakos currently officially supports Windows 10 or 11 (64-bit). Users on Linux or MacOS may see occasional bugs.

<p align="center"><a href="https://drakos.gg/installation/"><img src="assets/btn-install-lg.png" height="64" alt="Installation guide"></a><a href="https://drakos.gg/pricing/"><img src="assets/btn-pricing-lg.png" height="64" alt="Pricing"></a><a href="https://drakos.gg/accounts/"><img src="assets/btn-account-lg.png" height="64" alt="Your account"></a></p>

<br>

<img src="assets/h-support.webp" width="880" alt="Support">

Ask questions and report bugs on [Discord](https://discord.gg/sgKnHh8CRd). For account and purchase help, email [support@drakos.gg](mailto:support@drakos.gg). Check [status.drakos.gg](https://status.drakos.gg) for service status.

<p align="center"><a href="https://discord.gg/sgKnHh8CRd"><img src="assets/btn-discord-lg.png" height="64" alt="Join the Discord"></a></p>

<sub>Drakos is not affiliated with or endorsed by Square Enix or the Dalamud team.</sub>
