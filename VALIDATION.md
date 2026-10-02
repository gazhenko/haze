# Haze 0.4.0 validation

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS | Apple M1 Pro, Metal, 1600 × 1000 | 690 checks passed; zero failures or runtime errors |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | 690 checks passed; zero failures or runtime errors |
| macOS environment | Apple M1 Pro, Metal, 1600 × 1000 | 195 checks passed; zero failures or runtime errors |
| Linux fallback | NVIDIA RTX 3080, OpenGL, 1600 × 1000 | 195 environment checks passed; zero failures or runtime errors |
| Windows x64 | Cross-built for Direct3D 11 and Vulkan | Runtime unverified; no Windows test machine was available |
| Intel Mac | Included in the universal app | Runtime unverified |

## Story

The walkthrough checks that the story’s pages, the physical lettering and the puzzles agree: the slate’s engraved numerals are the manifold’s actual solution, the drowned score names the fountain’s actual five-bell song, the seal’s cut route appears on its readable page, both desks carry their names, and the journal holds only pages the visitor has read. Both physical letters print exactly the text the game reads; the scene builder refuses to build if the printed textures and the story file disagree. The early-visit fallback for macOS saves is checked with an isolated copy: the early visit loads when no newer visit exists, a newer visit takes precedence, and the early file is never modified.

## Sound and music

The walkthrough records the live mix at the listener, after every source and filter, at fourteen moments: the title, walking through the rainy hall, the manifold refusing and accepting the measures, a single bell, the five-bell song, a mirror, the light reaching the seal, the ending, the morning sea, muted, and full and half volume. Those recordings are kept with each run.

- Every capture stays below the −2 dBFS ceiling of the safety limiter. The loudest moment on the Mac was −5.9 dBFS (the five-bell song); on Linux the same moment reached the ceiling once and the limiter acted by 0.4 dB.
- Footsteps stand out from the rain at a walking cadence (11 steps heard on the Mac, 12 on Linux).
- Near the unsolved bells the score steps back to about a sixth of its level; it returns once the song is remembered.
- The four imported, compressed bells measure within half a cent of SUN C4, MOON D4, REED F4 and STAR G4 (a Goertzel scan in the walkthrough), so the sound puzzle keeps four distinct, true pitches.
- Mute silences the output (−120 dBFS at the listener on both systems), and the volume setting scales the listener; on Linux half volume measured 6.5 dB below full.
- The rain eases with each finished round and has stopped when the light reaches the seal; the ending plays Mara’s song; the morning has sea and birds and no rain.

## Interface

The new screens — title, settings, pause, journal, letters on paper, the slate, the drowned score, the seal, act titles, prompts and the ending — were inspected in native screenshots on both systems. The full walkthrough also exercises the developer guide through every step with deliberate wrong inputs, saved and resumed visits, collision and boundary recovery, moving passages, inscriptions, reflections and the morning.

At a 60 FPS cap, the scripted traversal averaged 48.44 ms per frame on the Mac and 19.76 ms on Linux, with P95 values of 72.61 ms and 31.52 ms; exterior views averaged 17.13 ms and 17.03 ms. These describe those machines and that route, not minimum requirements. The new audio did not change frame times measurably.

## Trailer

The trailer was recaptured from the release Mac player at 1920 × 1080: 1,260 frames at a fixed 30 FPS with no runtime errors. Its stereo soundtrack is mixed from the game’s own files — the evening rain and the title theme, a bell, a page turn, then the morning sea, wind, birds and Mara’s song — and the complete 42-second H.264/AAC film was decoded after composition.

## Package checks

Each platform archive contains the complete player, instructions, credits (including every sound’s origin and the Kenney CC0 licence texts) and checksums. Packaging reads every archived file back and compares its bytes. The Mac signature is checked before packaging and again after extracting the completed archive. Before publication, all GitHub release assets are downloaded again and checked against the local SHA-256 values.

The Mac app is ad-hoc signed and is not Apple-notarized. Windows is unsigned. Launch instructions explain the platform prompts.

The release’s `release-manifest.json` records archive hashes, executable hashes, platform status, the trailer hash, and the shared scene source fingerprint.
