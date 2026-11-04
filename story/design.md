# Design

## Rules carried over from 0.4.0

- No combat, timer, jump or fail state. A wrong input resets only that mechanism’s current attempt.
- Every solution comes from something written, engraved or visible in the world.
- Every sound puzzle has a written or visual twin.
- The screen stays quiet: an aiming dot, prompts that name their key, act titles that appear once.
- The journal holds the rounds, every page read, and optional hints. The developer guide stays optional.

## Morning as progress

Each region is in rainy dusk until its round is finished. Then its sky turns to morning, the rain stops there, and the haze pulls back to its edges. From any high point — and on the camera obscura’s table — the player can see what is finished and what is still held.

This is the game’s main visual promise and its largest technical risk: weather, lighting and ambience have to be set per region and blend at the boundaries.

## The “let go” step

Every round ends with one small, plain action Elias could not take. It is the same idea as the shipped valve’s LET GO plaque.

| Region | Final act |
| --- | --- |
| The Baths | Turn the little valve for her tree |
| The Springs | Open the outflow chalked *not tonight* |
| The West Cliffs | Break the HOME bell out of its mould |
| The Cure | Water the seed beds |
| The Summit | Release the strap on the master clock’s pendulum |
| The Light | Put out the lamp |

## Motifs

- **7:42.** Every clock on the island, the tide boards, the last line in the guest book. The two minutes between the sailing at 7:40 and the rain are the whole story.
- **Mara’s song.** As rung in the Baths — REED SUN STAR REED MOON (F4 C4 G4 F4 D4) — it ends on D and sounds unfinished. The buoys carry it, the school gives its words, the orchestrion its waltz. The foundry’s fifth bell, HOME, is an F an octave above REED; it lets the song end at home, leading into the shipped ending theme, *After the rain*, which is already in F major. The score keeps withholding the song until the player has earned each appearance.
- **Seals.** Mara’s green leaf wax, on her letters, her seed tins and your envelope. Elias’s keeper stamp, on his letters and the Baths’ seal.
- **Brass discs.** Each region’s mechanisms carry their original keeper’s brass crest, with Elias’s disc riveted over it where he took the round on. The history of the island is readable in brass, using art the game already has.
- **Chalk.** Elias’s ticks on gauges and wheels: his rounds, done every evening to the last step and no further.

## Controls and carried things

Keep the shipped verbs: walk, look, E to use, Q to turn back, the journal. The player carries at most two things: the letter (unusable until the lamp room) and a lantern for the cistern and the caves. No collectibles and no inventory screen.

Haze is gaining gamepad support; every new puzzle must work with the same two actions on a controller.

## Sound and its twins

| Puzzle | By ear | Without sound |
| --- | --- | --- |
| Fountain bells (shipped) | The bells’ pitches | The drowned score; the journal’s written score |
| Telegraph tape | — | It is printed; the Morse chart is on the wall |
| Buoy tuning | Strike and compare with the fork | Chladni sand patterns on the plate |
| Sea caves | The shortest echo | Ripples in the rock pools |
| Orchestrion roll | Hear the waltz | The song’s words and the roll’s pitch rows |
| Heliograph | — | Visual Morse |
| Causeway | Follow the buoys in the song’s order | The obscura’s view of the sand bars; the pilot chart |

## Changes to the shipped bathhouse

- A prologue in front of it: the crossing and the landing cove.
- The envelope in the journal from the start.
- Mara’s seed tins carry the leaf seal; the north gate and Elias’s list of the island’s rounds are added behind the garden.
- The five 0.4.0 act titles become chapters within Act I.
- The ending text becomes the end of Act I: the headland has its morning, and the haze stands at the treeline.
- **Unchanged:** every puzzle, both letters, the slate, the score and the seal.

**Canon change:** `Docs/STORY.md` in the Unity project says the game never tells where Mara went. This plan does tell, and moves the quiet mystery to Elias’s crossing and to who the player is.

## Production notes

- The bathhouse is one building that took several art passes; forty rooms is roughly eight more regions of that size.
- Build the Village first as the first fully finished region. It is the hub, it carries the biggest reveals, and it is where per-region morning has to work.
- Reuse the existing kit: masonry, ironwork, fitted lamps, handwritten papers, wax seals and brass discs.
- Regions will need to load and unload rather than living in one scene.
- The save format will grow per-region state. Keep the save directory and application identity stable so 0.4.0 visits continue.
- Native verification should grow per region in the same style as today’s walkthrough: real movement, real interaction rays, screenshots and recorded audio.
