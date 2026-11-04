# ✈️ Airline CEO

**A single-player airline management game that runs in your browser.**
You are the chief executive of one airline, competing against computer-controlled rivals in a living, believable market. Pick any year from 1946 to 2026, pick a home airport, and try to build something that lasts.

▶ **Play now:** https://utuhhhh.github.io/airline-ceo-play/ — no install, no account. Saves stay in your own browser.

---

## The idea
Most airline games are spreadsheets with planes on top, or arcade games with no real economy. Airline CEO aims for the middle: **a deep simulation of passengers, aircraft, money and people**, presented like a modern game — big cards, maps and charts instead of walls of numbers.

## At a glance
| | |
|---|---|
| Start years | **1946 – 2026**, history follows the real world |
| Airports | **658** in 79 countries, with runways, curfews, slots, fees, jet bridges, opening and closing years |
| Cities | **582** metro areas, plus ~10,000 population cells that decide which airport people drive to |
| Aircraft | **123** models from **33** manufacturers, from the DC-3 and Viscount to the A321neo and 787 |
| Rival airlines | ~**80** in a 2019 start (~5,500 aircraft, ~9,000 routes); ~35 in a 1960s start |
| Rival names | **3,200+** fictional airline names, a different line-up every game |
| History | **330** real aviation and world events, **460** planned events, **64** kinds of random events, **950** festivals and holidays |
| Trains | **76** high-speed rail links with opening years, competing with flights |
| Subsidised routes | **79** government-contract routes in 63 schemes |
| Progression | **10** levels (Air taxi → Global carrier), **39** achievements |

## How you play
**Starting out**
- Build an airline from nothing, or **buy a failing one for €1** — with its debts, staff and routes — and turn it around within two years.
- Choose a **low-cost, full-service hub, charter or regional** airline, or design your own product. Pick a name, colours, livery and logo.
- Choose who *you* are: your CEO background gives one lasting advantage, and your career can take you to other airlines later.
- Three difficulty levels and five named save slots.

**Network and schedule**
- Find routes on a map with demand, fares and rivals for every destination; win traffic rights, respect border rules (Schengen, blocs, closed airspace) and night curfews; buy slots at busy airports.
- Build timetables per aircraft across the week; flights to the same place are spread over the day; one click reorganises the whole fleet.

**Fleet**
- Buy new (with delivery queues and orders) or used, or lease from lessors; sell when aircraft age.
- Design cabins by seat pitch and class; register aircraft under your country's prefix.
- Maintenance checks by family, spare aircraft, boarding and cleaning times per type.

**Product and money**
- Fares per class, bag and seat fees (from 2006), catering, extras, marketing campaigns, passenger reviews.
- Cargo, tour-operator **charter contracts**, and **government contracts** for small and island airports.
- Full books: loans and a bank, depreciation, income statement and balance sheet; go public, pay dividends, buy back shares.

**People**
- Hire pilots, cabin crew, engineers and ground staff; set pay per role; watch for strikes.
- A board sets targets and can fire you. Run out of cash for three months and the game is over.

**The world around you**
- Rivals open and close routes, start fare wars, replace their bosses, get rescued by governments or go bankrupt; new airlines appear.
- Fuel shocks, recessions, COVID, wars and airspace closures, new airports opening (and old ones closing), seasons and festivals.
- A newspaper reports it all, including your own successes and failures.

## What makes the simulation believable
- **Passengers choose.** Every week, demand for tens of thousands of city pairs is split between business, leisure and budget travellers. They compare fares, times, frequency, connections through hubs, trains — and the option of not flying at all (nested-logit choice model). Passengers who don't fit spill to the next-best flight.
- **Real-world calibration.** Demand is built from real populations, incomes, tourism and ties between countries, then fitted to real 2019 airport and route traffic and to historical traffic since 1946. Every data row is marked *sourced*, *estimated* or *guess*.
- **Real costs.** Fuel by the year's real price, crew hours, maintenance per block hour, airport fees, ownership and lease costs, inflation and exchange rates.
- **Real accounting.** Double-entry books for every airline, checked every simulated day.

## The world
Playable today: **Europe, Turkey, the Caucasus, North Africa, the Middle East and South Asia**. East Asia (China, Japan, Korea, Taiwan) is being built on its own branch; Southeast Asia, Russia/Central Asia, North America, Latin America, Africa and Oceania follow. Data for every region is already drafted, and every country will have at least one airport.

## Technical specs
| | |
|---|---|
| Delivery | **One self-contained HTML file** (~1.2 MB), no server, no install; the internet is used only for the map library and map tiles |
| Code | Plain JavaScript (ES modules), no frameworks; ~19,500 lines in 45 engine and 4 interface modules; bundled with esbuild |
| Map | Leaflet 1.9 with built-in country borders |
| Threads | The simulation runs in a **Web Worker** (background thread), so the screen never freezes |
| Saves | Browser storage (IndexedDB), 5 slots; a 2019 game saves to ~16 MB |
| Starting a game | ~13 s (rivals build their networks and the market settles) |
| Speed | one quarter of play with ~80 rivals: ~24 s on a 2-core test machine (≈1.8 s a week) |
| Memory | ~200 MB of game data for a full 2019 market, under 1 GB for the browser tab |
| Recommended | Any recent desktop browser (Chrome, Edge, Firefox, Safari), 8 GB RAM |

**Architecture.** The engine (`engine/`) knows nothing about the screen: a daily tick runs flights, revenue and costs; once a week passengers choose their itineraries for every city pair; once a month airlines review their routes, prices and fleets. The interface (`web/`) only sends player actions and draws snapshots. Far regions you don't fly to are simulated monthly instead of weekly (same formula, so nothing jumps when you arrive). Data lives in readable CSV tables that are built into the game file. Results are deterministic: a saved and reloaded game continues exactly as one that never stopped (checked by an automated play test).

**Testing.** 49 design checks against real-world numbers (traffic, fares, margins, hub shares), regression tests, multi-year market runs with only computer airlines, and automated browser tests of the interface.

## Status
In active development and released often (r1–r13 so far; current: r13, 4 Nov 2026). Every release is kept, and the latest is always live at the link above.

