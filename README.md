#Game QA Portfolio: Bug Reporting & Analysis
Candidate: Sivanesh A
Role: Junior QA Tester / Intern
Focus: Functional, Logic, and Visual Regression Testing

##📌 Overview
This repository contains a collection of professional bug reports for various titles, including Boom Beach, Albion Online, Valorant, Minicraft, and Chained Together. These reports demonstrate my ability to identify reproduction steps, analyze root causes, and provide user-side workarounds.

##🏝️ Bug Report 1: Boom Beach (Mobile)
Title: Gameplay / UI — Attack Screen Button Unresponsive

Type: UI / Interaction
Severity: Medium
Summary: The "Attack" button on the raid screen becomes unresponsive after scouting, preventing battle start and causing troop loss or wasted energy.
System Info: Android 14 (mid-range device) | 6GB RAM
Key Finding: Touch event fails to register due to animation overlap and UI thread lock.
Workaround: Restart the app or switch to another base before confirming attack.

##⚔️ Bug Report 2: Albion Online (PC/Mobile)
Title: Progression / UI — Crafting Menu Soft-Lock

Type: Progression / Sync
Severity: Medium
Summary: After successful crafting, items do not register in inventory, causing the crafting menu to freeze or show incorrect status.
System Info: Windows 11 | Mid-range PC + Android cross-play
Key Finding: Client-server inventory sync delay fails to update post-craft event.
Workaround: Relog or wait 1–2 minutes before crafting again.

##🔫 Bug Report 3: Valorant (PC)
Title: Gameplay / Visual — Agent Model Texture Streaming Glitch

Type: Visual / Asset Streaming
Severity: Low
Summary: Agent models appear invisible or low-poly for 2–3 seconds at round start due to delayed texture loading.
System Info: Intel i5-11300H | GTX 1650 (82°C during occurrence)
Key Finding: Asset streaming budget throttled by thermal load and high FPS.
Workaround: Enable Multithreaded Rendering and ensure game is on SSD.

##⛏️ Bug Report 4: Minicraft (Java/PC)
Title: World Generation / Gameplay — Chunk Disappearance on Respawn

Type: Logic / Persistence
Severity: High
Summary: Newly generated chunks (caves/structures) reset or disappear after player death and respawn.
System Info: Windows 11 | Java Edition latest
Key Finding: Chunk save fails to update correctly on death/respawn event.
Workaround: Manually save and reload world after respawn.

##⛓️ Bug Report 5: Chained Together (Steam/PC)
Title: Multiplayer / Physics — Chain Desync During Co-op Jumps

Type: Multiplayer / Physics
Severity: High
Summary: Chain connection breaks when one player lags during jumps, causing the second player to fall through the map.
System Info: Windows 11 | Mid-range hardware
Key Finding: Netcode fails to sync chain physics and player position in the same tick.
Workaround: Restart the full session or coordinate exact simultaneous jumps.

##🛠️ Technical Skills Demonstrated

Reproduction Testing: 100% success rate in defining clear, actionable steps.
Environment Logging: Capturing hardware specs and session details.
Root Cause Analysis: Hypothesizing on sync delays, state persistence, and netcode issues.
Communication: Writing clear Expected vs. Actual results for developer hand-off.
