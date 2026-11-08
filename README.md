# Brickcress 1.0 TEST
Native Android Tawa supported-brick shading puzzle. Android 8+ (min26), target35. Package com.gg007.brickcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Tawa / Tawamurenga training puzzle on a staggered 4-row, 4-brick-per-row wall. Tap unnumbered bricks to shade or clear them. Numbered bricks remain light and count the shaded bricks sharing an edge, up to six neighbors: left/right, two above and two below where present. Every shaded brick above the bottom row needs at least ONE shaded brick touching its lower edge in the next row. Bottom-row bricks need no support. Never shade three consecutive bricks in any horizontal row. Separate supported dark groups ARE allowed; neither dark nor light connectivity is required. No wrapping at the wall edges. Twelve original uniquely solvable clue boards; auto-check after every tap, unlimited undo/reset, next and level selection. Saved palette and optional dots that repeat shaded marks. Unshaded cells may be left blank; no explicit light-note state or timer in this training edition.

## Download and status
https://mega.co.nz/#!0NUmwbYZ!xJD0dKDSGb9k5fdB9g6e27fFYDA2zY65guBEbpDWH38
APK SHA256 926d450dc072088d7c09b7a30445c3beff7767452b695858ff13492bb4dc6f49; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Independent physical brick-interval geometry and row-string oracle versus production integer-center adjacency passed 786,432 complete shade masks, all 65,536 masks on each of twelve boards, plus 65,536 shape-only comparisons. Each board has exactly one full-rule shading. Tests cover all 256 cell-pair adjacencies, six-neighbor counts, below-edge support, horizontal triples, bottom-row exemption, disconnected supported groups allowed, clue lock, invalid bounds, undo, solved lock, reset and replay. Portable generator with seed 490109 reproduces all twelve boards; archived Java oracle reruns. Actual drawing-adapter staggered hit targets, solve/undo/replay, next, levels, menu, privacy and saved palette/dark-mark settings pass. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 180 prior studio descriptions and web registry game/mechanic records. Sukima was rejected because Gapwillow already places circle-anchored trominoes with 2x2 gaps. Cloudball places one balloon and one iron ball per room on an aligned square grid. Brookmere counts shades around grid vertices and requires connected light cells. Brickcress instead shades staggered bricks with six-edge-neighbor clue counts, downward support by either overlapping lower brick, a horizontal dark-run limit and no connectivity requirement. Its offset-row hit geometry and support/count validator differ from those games. No Tawa match found in the reviewed corpus; recovered repository corpus remains partial. Known Tawa / Tawamurenga adaptation, not a global invention claim. Original generated boards, code and visuals; no source puzzle layouts, code or art copied.
Rules https://www.janko.at/Raetsel/Tawa/index.htm ; independent rules https://puzzles.twistymaze.com/help/bricks .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/brickcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.brickcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Brickcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, dark brick marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 181-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/mv7ofwm6kjch-brickcress-source-archive . Repository https://github.com/iLanis-agent/brickcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
