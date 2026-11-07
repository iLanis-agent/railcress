# Railcress 1.0 TEST
Native Android Tren parked-car clearance puzzle. Android 8+ (min 26), target 35. Package com.gg007.railcress.

## Rules
Tren: tap a gold clue to cycle its 2- or 3-cell car. Each car must contain exactly one clue and cars cannot overlap. Each clue gives the total empty steps its car could slide from both ends along its length before the frame or another car. Count with all other cars fixed. Every clue must have a car; unused cells stay empty and need not connect. The twelve 4x4 puzzles have distinct clue and car layouts with exactly one solution each. Undo/reset/next/levels and saved car palette/car letters.

## Download and status
https://mega.co.nz/#!QBcFWYIS!6Mt-5w7MdjctfNrVnS_7q4aMsqwfjg1F0xEPsiLkmQs
APK SHA256 084958fcf1c03eb363fcb290ee0c648f30b8ff557b72062638c09a980d9114f7; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous download bytes match.

## Checks
Independent oracle translates every whole car through each intermediate position in both directions, unlike production end-ray counting. Both agree on all 2,435 candidate states including empty selections across 12 levels and 120,000 invalid/random states. Exactly one solution per puzzle; all 12 clue and car layouts distinct. Archived generator reproduces levels.json; archived Java exhaustive tests pass. Bounds, solved lock, car cycling and solve/undo/replay/reset pass. Drawing adapter tests actual clue taps, ignored nonclue cells, reset/undo/next/levels/menu/settings/privacy and saved palette/car letters/completion. Six actual drawing screens inspected, not phone screenshots. Phone runtime, performance and external-browser handoff QA remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Live 803-entry registry, 127 recovered partial READMEs and semantic review of all 155 prior studio cards found no Tren match. Parking fee/stripe calculators are unrelated. Homebriar places fixed-step circles into countries; Heronputt plays shrinking ball shots; Reedvox compares size/orientation of strips. Railcress instead reconstructs stationary parked cars from their mutual sliding-clearance counts. Known Tren genre, not a global invention; recovered corpus is partial. Rules https://www.gmpuzzles.com/blog/2013/08/the-puzzle-robot-5-tren/ https://www.cross-plus-a.com/html/cros7tren.htm https://logic-masters.de/LM/2013/dokumente/LM2013-Quali-Anleitung_en.pdf .

## Build
JDK 17 and Android SDK 35/build-tools35.0.0. python generate-levels.py reproduces levels.json. Board.java embeds generated clues, candidate cars and solutions. javac -d /tmp/train-test src/com/gg007/railcress/Board.java BoardTest.java and java -cp /tmp/train-test com.gg007.railcress.BoardTest. bash build.sh creates an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private original signing inputs. No credentials in source. Release build settings, signed TEST artifact, not final store release.

## Privacy and branding
Railcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Car palette, car letters and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 icon byte-equal to original. Menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and websites
Complete source and APK privately preserved at https://files.instinct.com/u0ajxjjnvllb-railcress-source-archive, including exact cumulative 156-card studio and published catalog/studio sources/updater. Repository https://github.com/iLanis-agent/railcress holds README only; full Git source commit pending. Both website publications checked separately. No Pages settings change or Play rollout. November 8, 2026.
