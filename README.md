# ✈️ Airline CEO

**A single-player airline management game that runs in your browser.**
You are the chief executive of one airline, competing against computer-controlled rivals in a living, believable market. Pick any year from 1946 to 2026, pick a home airport — or pick a historical scenario — and try to build something that lasts.

▶ **Play now:** https://utuhhhh.github.io/airline-ceo-play/ — no install, no account. Saves stay in your own browser.

*This page describes release **r19** (4 Nov 2026).*

---

## The idea
Most airline games are spreadsheets with planes on top, or arcade games with no real economy. Airline CEO aims for the middle: **a deep simulation of passengers, aircraft, money and people**, presented like a modern game — big cards, maps, charts and step-by-step screens instead of walls of numbers.

## At a glance
| | |
|---|---|
| Start years | **1946 – 2026**; aircraft, prices, borders and events follow real history |
| Ways to play | **3 game modes** (Real world, Open world, Sandbox), **6 scenarios**, 3 difficulty levels, takeovers of failing airlines |
| Airports | **1,222** in over 100 countries and territories, with runways, curfews, slots, fees, jet bridges, opening and closing years |
| Cities | **1,080** metro areas, plus ~14,000 population cells that decide which airport people drive to |
| Aircraft | **123** models from **35** manufacturers, from the DC-3 and Viscount to the A321neo and 787 |
| Rival airlines | **170** in a 2019 start, flying ~10,000 aircraft on ~13,000 routes; ~50 in a 1960s start |
| Rival names | **3,300+** fictional airline names — a different line-up every game |
| History | **485** real aviation and world events, **460** planned events, **74** kinds of random events, **1,300+** festivals and holidays |
| Trains | **221** rail links (121 high-speed) with opening years, competing with flights |
| Government contracts | **79** subsidised routes in 63 European schemes |
| Progression | **10** levels (Air taxi → Global carrier), **39** achievements |

## Ways to play
- **Free game.** Build an airline from nothing, or **buy a failing one for €1** — with its debts, staff and routes — and turn it around within two years. Choose a **low-cost, full-service hub, charter or regional** airline, or design your own product. Pick a name, colours, livery and logo, and a CEO background that gives one lasting advantage.
- **Game modes.** **Real world** keeps real politics: route approvals, fixed fares where they applied, ownership rules, closed airspace and wars. **Open world** lets you switch any of those off (rivals play by the same rules). **Sandbox** is for experimenting.
- **Scenarios** with a goal, a deadline and a medal:
  - *The Wall comes down* (1990) — the first private airline of a newly free country (Budapest, Warsaw, Prague, Bucharest or Sofia)
  - *Rescue a flag carrier* (1992) — take over a loss-making national airline as Europe opens up
  - *Low-cost revolution* (1997) — two jets at a secondary airport
  - *Oil shock* (1973) — a holiday charter airline when fuel prices quadruple
  - *Pandemic* (2020) — take over an airline weeks before COVID
  - *Gulf hub* (1995) — a long-haul airline between Europe and Asia
- **Cheats** (optional, in the menu): money, unlock everything, instant deliveries, no breakdowns or strikes. Using one stops achievements and level points.

## Features
**Network and schedule**
- Find routes on a map: demand, fares and rivals for every destination, with tinted cards for places you already fly and a switch to hide them.
- Win traffic rights, respect border rules (Schengen, trade blocs, closed airspace) and night curfews; buy slots at busy airports; apply for (or withdraw) route approvals.
- Route settings as numbered steps: aircraft, fares, times, service. Timetables per aircraft across the week; flights to one place spread over the day; one click reorganises the whole fleet without adding slot or night problems.

**Fleet**
- Get an aircraft in six screens: maker → type → new or used, buy or lease → specs and options → cabin → registration, with the price always shown.
- Saved cabin layouts; registration ranges per aircraft family under your country's prefix.
- Delivery queues, lessors, used-aircraft market, refits, maintenance checks by family, spare aircraft, boarding and cleaning times per type.

**Product and money**
- Fares per class, bag and seat fees (from 2006), catering and extras, marketing campaigns, passenger reviews.
- Cargo, tour-operator **charter contracts** (including short-notice ones, with reminders before they start), and **government contracts** for small and island airports.
- Full books: loans and a bank, depreciation, income statement and balance sheet; go public, pay dividends, buy back shares.

**People and safety**
- Hire pilots, cabin crew, engineers and ground staff; set pay per role (every change is confirmed with its cost); watch for strikes.
- **Accidents and incidents** at real-world rates for the year — from bird strikes and hard landings to rare serious accidents and crashes. Risk grows with overdue maintenance, older aircraft and unhappy or short-staffed crews; insurance pays, but reputation and premiums suffer. Rivals have accidents too.
- A board sets targets and can fire you. Run out of cash for three months and the game is over.

**Your airline and your rivals**
- *My airline* page: your airline as a rival sees it, each figure ranked against your competitors, plus a Safety card.
- Rivals open and close routes, start fare wars, replace their bosses, get rescued by governments or go bankrupt; new airlines appear.
- Fuel shocks, recessions, COVID, wars and airspace closures, new airports opening and old ones closing, seasons and festivals — all reported in a full-screen newspaper.

**Interface**
- Dashboard tiles open the full chart behind them; all warnings and questions use the game's own dialogs; short sliders with typed values; redrawn aircraft side views (including freighters); five named save slots.

## What makes the simulation believable
- **Passengers choose.** Every week, demand for tens of thousands of city pairs is split between business, leisure and budget travellers. They compare fares, times, frequency, connections through hubs, trains — and the option of not flying at all (nested-logit choice model). Passengers who don't fit spill to the next-best flight.
- **Real-world calibration.** Demand is built from real populations, incomes, tourism and ties between countries, then fitted to real 2019 airport and route traffic and to historical traffic since 1946. Every data row is marked *sourced*, *estimated* or *guess*.
- **Real costs.** Fuel at the year's real price, crew hours, maintenance per block hour, airport fees, ownership and lease costs, insurance, inflation and exchange rates.
- **Real accounting.** Double-entry books for every airline, checked every simulated day.

## The world
Playable: **Europe, Turkey, the Caucasus, North Africa, the Middle East, South Asia and all of the rest of Asia** — China, Hong Kong, Macau and Mongolia; Japan, the Koreas and Taiwan; Southeast Asia; Russia east of the Urals and Central Asia (about 170 rivals). The Middle East and Asia are open to new airlines from 1990.
Still to come: the Americas, Africa and Oceania (see *Coming next*). Data for every region is already drafted, and every country will have at least one airport. New features wait until the whole world is in.

## Technical specs
| | |
|---|---|
| Delivery | **One self-contained HTML file** (~1.5 MB); no server, no install. The internet is used only for the map library and map tiles |
| Code | Plain JavaScript (ES modules), no frameworks; ~20,300 lines in 48 engine and 4 interface modules; bundled with esbuild |
| Map | Leaflet 1.9 with built-in country borders |
| Threads | The simulation runs in a **Web Worker** (background thread), so the screen never freezes |
| Saves | Browser storage (IndexedDB), 5 named slots, compressed: a 2019 game is ~23 MB, ~4 MB packed |
| Starting a game | ~35 s on the slow test machine (rivals build their networks and the market settles) |
| Speed | a game week takes ~1.5–4 s with 170 rivals on a slow 2-core test machine; a normal computer is faster |
| Memory | ~260 MB of game data for a full 2019 market; the browser tab uses about 1–1.5 GB |
| Recommended | A recent desktop browser (Chrome, Edge, Firefox, Safari) and 8 GB RAM |

*Measured on r19, 2019 start from Timișoara, with all of Asia in. A speed and save-size pass is next (targets: new game under 20 s, a week under 1 s, saves about half the size).*

**Architecture.** The engine (`engine/`) knows nothing about the screen: a daily tick runs flights, revenue and costs; once a week passengers choose their itineraries for every city pair; once a month airlines review their routes, prices and fleets. The interface (`web/`) only sends player actions and draws snapshots. Far regions you don't fly to are simulated monthly instead of weekly (same formula, so nothing jumps when you arrive). Data lives in readable CSV tables built into the game file. Results are deterministic: a saved and reloaded game continues exactly as one that never stopped (checked by an automated play test).

**Testing.** 49 design checks against real-world numbers (traffic, fares, margins, hub shares), regression tests, multi-year market runs with only computer airlines, and automated browser tests of the interface.

## Coming next
**The rest of the world**, one region at a time: North America → Mexico, Central America and the Caribbean → South America → Africa → Oceania. The data for each is already drafted.

**Faster and lighter.** A speed and save-size pass: quicker new games and weeks, saves about half the size, then a check on a normal home computer.

**On the wish list** (waiting until the whole world is in):
- 🎟️ Several fares within a class — cheap early tickets, expensive late ones
- 🤝 Partner airlines for connections, one per region
- 📈 A full stock market: stakes in rivals, hostile takeovers and mergers
- 🌍 Daughter airlines abroad
- 🏖️ Holiday areas — which airport tourists use for a resort or a coast
- ⚖️ Passenger compensation rules per region (EU261 and others)
- 🏛️ Government contracts v2: rivals fly theirs, new schemes in other regions
- ❄️ Charter: seasonal leases, or renting idle aircraft out in winter
- 🗺️ The whole world in full detail (expert option), and years before 1990 for the new regions
- 🎬 More scenarios: *Jet age 1960*, *Open skies 1993*, and new ones for each region

**Balance being looked at:** careless airlines go bust too slowly; whether recent starts are too hard; scenario goals; accident rates over a long game; making the route suggestions good enough to follow.

## Status
In active development and released often (r1–r19 so far; current: r19, 4 Nov 2026). Every release is kept, and the latest is always live at the link above.

