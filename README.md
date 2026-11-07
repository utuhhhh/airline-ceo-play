# ✈️ Airline CEO

**A single-player airline management game that runs in your browser.**
You are the chief executive of one airline, competing against computer-controlled rivals in a living, believable market. Pick any year from 1946 to 2026, pick a home airport — or pick a historical scenario — and try to build something that lasts.

▶ **Play now:** https://utuhhhh.github.io/airline-ceo-play/ — no install, no account. Saves stay in your own browser.

*This page describes release **v0.91.1** (7 Nov 2026).*

---

## The idea
Most airline games are spreadsheets with planes on top, or arcade games with no real economy. Airline CEO aims for the middle: **a deep simulation of passengers, aircraft, money and people**, presented like a modern game — big cards, maps, charts and step-by-step screens instead of walls of numbers.

## At a glance
| | |
|---|---|
| Start years | **1946 – 2026** in Europe, North and Central America, the Caribbean, South America, South and South-east Asia, East and Southern Africa, and Oceania, **1990 – 2026** everywhere else (history back to 1946 coming region by region); aircraft, prices, borders and events follow real history |
| Ways to play | **3 game modes** (Real world, Open world, Sandbox), **6 scenarios**, 3 difficulty levels, takeovers of failing airlines |
| Airports | **1,980** — **every country and territory has at least one** (230+), with runways, curfews, slots, fees, jet bridges, opening and closing years |
| Cities | **1,772** metro areas, plus ~27,000 population cells that decide which airport people drive to |
| Aircraft | **123** models from **35** manufacturers, from the DC-3 and Viscount to the A321neo and 787 |
| Rival airlines | **317** in a 2019 start, flying ~16,000 aircraft on ~19,000 routes; ~120 in a 1960s start |
| Rival names | **4,400+** fictional airline names — a different line-up every game |
| History | **750** real aviation and world events, **755** planned events, **89** kinds of random events, **1,400+** festivals and holidays |
| Trains | **242** rail links (121 high-speed) with opening years, competing with flights |
| Government contracts | **79** subsidised routes in 63 European schemes |
| Progression | **10** levels (Air taxi → Global carrier), **39** achievements |
| Money | **170+** currencies, each with real exchange rates by year |

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
- Route settings as numbered steps: aircraft, fares, times, service. Timetables (open from the first level) per aircraft across the week; flights to one place spread over the day; one click reorganises the whole fleet without adding slot or night problems.

**Fleet**
- Get an aircraft in six screens: maker → type → new or used, buy or lease → specs and options → cabin → registration, with the price always shown.
- Saved cabin layouts; registration ranges per aircraft family under your country's prefix.
- Delivery queues, lessors, used-aircraft market, refits, maintenance checks by family, spare aircraft, boarding and cleaning times per type.

**Product and money**
- Fares per class, bag and seat fees (from 2006), catering and extras, marketing campaigns, passenger reviews.
- Cargo, tour-operator **charter contracts** (including short-notice ones, with reminders before they start), and **government contracts** for small and island airports.
- Full books: loans and a bank (repaying asks first), depreciation, income statement and balance sheet; go public, pay dividends, buy back shares.

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
- Four game speeds: 10 minutes, 1 minute, 10 seconds or 1 second per game day.
- 🪳 **Report a problem**: a floating button on every screen sends a one-line report with the release, game date and page — friends are already play-testing with it.

## What makes the simulation believable
- **Passengers choose.** Every week, demand for tens of thousands of city pairs is split between business, leisure and budget travellers. They compare fares, times, frequency, connections through hubs, trains — and the option of not flying at all (nested-logit choice model). Passengers who don't fit spill to the next-best flight.
- **Real-world calibration.** Demand is built from real populations, incomes, tourism and ties between countries, then fitted to real 2019 airport and route traffic and to historical traffic since 1946. Runway lengths are checked against public sources. Every data row is marked *sourced*, *estimated* or *guess*.
- **Real costs.** Fuel at the year's real price, crew hours, maintenance per block hour, airport fees, ownership and lease costs, insurance, inflation and exchange rates.
- **Real accounting.** Double-entry books for every airline, checked every simulated day.

## The world
**The whole world is in** (since r23): Europe, Turkey and the Caucasus; North Africa and the Middle East; South Asia; China, Japan, the Koreas and Taiwan; Southeast Asia; Siberia and Central Asia; the USA and Canada; Mexico, Central America and the Caribbean; South America; Sub-Saharan Africa; Australia, New Zealand and the Pacific — 52 areas in all. Every country, down to Tuvalu and Kiribati, has at least one airport.
Europe, North and Central America, the Caribbean, South America, South and South-east Asia, East and Southern Africa, and Oceania can be played from 1946; the rest of the world from 1990, with its history before 1990 on the way. Regions you don't fly to run on a lighter monthly simulation, so the whole world fits in one browser tab.

## Technical specs
| | |
|---|---|
| Delivery | **One self-contained HTML file** (~2 MB); no server, no install. The internet is used only for the map library and map tiles |
| Code | Plain JavaScript (ES modules), no frameworks; ~20,800 lines in 49 engine and 4 interface modules; bundled with esbuild |
| Map | Leaflet 1.9 with built-in country borders |
| Threads | The simulation runs in a **Web Worker** (background thread), so the screen never freezes |
| Saves | Browser storage (IndexedDB), 5 named slots, compressed: a 2019 world game is ~16 MB, ~5 MB packed |
| Starting a game | ~35–40 s on the slow test machine (rivals build their networks and the market settles) |
| Speed | a game week takes ~8–12 s with 317 rivals worldwide on a slow 2-core test machine; a normal computer is faster |
| Memory | ~440–490 MB of game data for the whole 2019 world; the browser tab uses up to ~2 GB |
| Recommended | A recent desktop browser (Chrome, Edge, Firefox, Safari) and 8 GB RAM |

*Measured on r24, 2019 start from Timișoara, whole world in. These are the numbers the speed pass is aimed at (targets on a normal computer: new game under 20 s, a game month under 5 s, under 400 MB).*

**Architecture.** The engine (`engine/`) knows nothing about the screen: a daily tick runs flights, revenue and costs; once a week passengers choose their itineraries for every city pair; once a month airlines review their routes, prices and fleets. The interface (`web/`) only sends player actions and draws snapshots. Far regions you don't fly to are simulated monthly instead of weekly (same formula, so nothing jumps when you arrive). Data lives in readable CSV tables built into the game file. Results are deterministic: a saved and reloaded game continues exactly as one that never stopped (checked by an automated play test).

**Testing.** 49 design checks against real-world numbers (traffic, fares, margins, hub shares), regression tests, multi-year market runs with only computer airlines, and automated browser tests of the interface.

## Coming next
The work is now split into departments that run side by side:
- 🐞 **QA** — fixes from friends' reports, one release at a time (r24 was the first batch).
- ⚡ **Performance** — a speed and save-size pass with the whole world, then a check on a normal home computer.
- 🌍 **World and history** — better travel between countries and continents; **history back to 1946 for the whole world**, one region at a time; runway history by year; smaller airports (down to 0.1 M passengers a year).
- 🎨 **A complete UI overhaul**, designed screen by screen; an **airport view** of your bases with your aircraft at the stands; hand-drawn aircraft art.
- 🛫 **A launch phase** before your first flight: company, licence and approvals by country and era — at most three game months, with a quick-start to skip it.
- 🔧 **Engineering** — the code split into smaller parts, three tiers of tests, automatic checks on every change.
- 🚀 **Launch** — a plan for **Steam** (desktop version with saves on disk, Steam achievements, cloud saves, leaderboards for scenarios and a weekly challenge), with the browser version kept as a free demo; a study of online multiplayer.

**On the wish list:**
- 🎟️ Several fares within a class — cheap early tickets, expensive late ones
- 🪑 Used aircraft arrive with their own cabin; cabins wear out and need a retrofit
- 🤝 Partner airlines for connections, one per region
- 📈 A full stock market: stakes in rivals, hostile takeovers and mergers
- 🌍 Daughter airlines abroad
- 🏖️ Holiday areas — which airport tourists use for a resort or a coast
- ⚖️ Passenger compensation rules per region (EU261, US and others)
- 🏛️ Government contracts v2: rivals fly theirs, new schemes outside Europe
- ❄️ Charter: seasonal leases and renting idle aircraft out in winter
- 🎬 More scenarios, including new ones for every region

**Balance being looked at:** new airlines should start less well known; charter contracts that pay with your own fleet; careless airlines go bust too slowly; whether recent starts are too hard; scenario goals; accident rates over a long game.

## Status
In active development and released often (r1–v0.91.1 so far; current: v0.91.1, 7 Nov 2026). Every release is kept, and the latest is always live at the link above.

