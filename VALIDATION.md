# Haze 0.15.0 validation

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS (universal build) | Apple M1 Pro, Metal, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors (mean frame 18.2 ms). Bathhouse suite: 738 checks, 0 failures. A first run while the Mac was heavily loaded by other work had 8 timing failures in one Light-region interaction; the rerun of the same app was clean |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors, 60 fps. Bathhouse suite, including simulated Steam virtual pads and Steam Deck controllers: 752 checks, 0 failures |
| Steam Deck (hardware) | Steam Deck OLED, SteamOS 3.8, Vulkan (RADV VANGOGH), 1280 × 800, Steam Deck preset | Controls and bathhouse suite: 0 failures; the Deck's Steam Input controller is detected and bridged. Crossing, Cure, Village, Light and Summit walkthroughs: 0 failures, holding the display's 60 Hz. Steam Deck preset: 11.9 ms mean, 19.7 ms P95. Every graphics preset applied and checked: 0 failures |
| Windows x64 build under Proton | Omarchy, NVIDIA RTX 3080, Proton Experimental (11.0), Direct3D 11 | Bathhouse suite: 738 checks, 0 failures, 0 runtime errors. Crossing walkthrough: 0 failures, 60 fps. This is the Windows game itself running through Steam's compatibility layer, not a Windows PC |
| Installers | DMG and Setup.exe built from the checksum-verified archives | Payloads compared file by file with their archives: 166 Mac and 173 Windows game files |
| Windows PC | Direct3D 11 with Vulkan fallback | Not run on a Windows PC |
| Intel Mac | Included in the universal app | Runtime unverified |

The Steam Deck checks ran on the hardware itself: the game's own verification modes, launched over SSH in Desktop Mode, with the Deck's controller attached. The Windows build ran its own checks under Proton on a Linux PC; no Windows PC or Intel Mac was available.

# Haze 0.14.0 validation (earlier release)

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS (universal build) | Apple M1 Pro, Metal, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors (mean frame 18.1 ms). Bathhouse suite: 738 checks, 0 failures |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors, 60 fps. Bathhouse suite, including simulated Steam virtual pads and Steam Deck controllers: 752 checks, 0 failures |
| Steam Deck (hardware) | Steam Deck OLED, SteamOS 3.8, Vulkan (RADV VANGOGH), 1280 × 800, Steam Deck preset | Controls and bathhouse suite: 0 failures; the Deck's Steam Input controller is detected and bridged. Crossing, Cure, Vessel, Village, Springs and Mainland walkthroughs: 0 failures, holding the display's 60 Hz. Steam Deck preset: 11.4 ms mean, 12.9 ms P95. Every graphics preset applied and checked: 0 failures |
| Windows x64 build under Proton | Omarchy, NVIDIA RTX 3080, Proton Experimental (11.0), Direct3D 11 | Bathhouse suite: 738 checks, 0 failures, 0 runtime errors. Crossing walkthrough: 0 failures, 60 fps. This is the Windows game itself running through Steam's compatibility layer, not a Windows PC |
| Installers | DMG and Setup.exe built from the checksum-verified archives | Payloads compared file by file with their archives: 166 Mac and 173 Windows game files |
| Windows PC | Direct3D 11 with Vulkan fallback | Not run on a Windows PC |
| Intel Mac | Included in the universal app | Runtime unverified |

The Steam Deck checks ran on the hardware itself: the game's own verification modes, launched over SSH in Desktop Mode, with the Deck's controller attached. The Windows build ran its own checks under Proton on a Linux PC; no Windows PC or Intel Mac was available.

# Haze 0.13.0 validation (earlier release)

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS (universal build) | Apple M1 Pro, Metal, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors (mean frame 17.6 ms). Bathhouse suite: 738 checks, 0 failures |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors, 60 fps. Bathhouse suite, including simulated Steam virtual pads and Steam Deck controllers: 752 checks, 0 failures |
| Steam Deck (hardware) | Steam Deck OLED, SteamOS 3.8, Vulkan (RADV VANGOGH), 1280 × 800, Steam Deck preset | Controls and bathhouse suite: 0 failures; the Deck's Steam Input controller is detected and bridged. Crossing, Cure, Vessel and Village walkthroughs: 0 failures, holding the display's 60 Hz, with up to two of the nearest lamps casting shadows. Steam Deck preset: 10.7 ms mean, 12.3 ms P95. Every graphics preset applied and checked: 0 failures |
| Windows x64 build under Proton | Omarchy, NVIDIA RTX 3080, Proton Experimental (11.0), Direct3D 11 | Bathhouse suite: 738 checks, 0 failures, 0 runtime errors. Crossing walkthrough: 0 failures, 60 fps. This is the Windows game itself running through Steam's compatibility layer, not a Windows PC |
| Installers | DMG and Setup.exe built from the checksum-verified archives | Payloads compared file by file with their archives: 166 Mac and 173 Windows game files |
| Windows PC | Direct3D 11 with Vulkan fallback | Not run on a Windows PC |
| Intel Mac | Included in the universal app | Runtime unverified |

The Steam Deck checks ran on the hardware itself: the game's own verification modes, launched over SSH in Desktop Mode, with the Deck's controller attached. The Windows build ran its own checks under Proton on a Linux PC; no Windows PC or Intel Mac was available.

# Haze 0.12.0 validation (earlier release)

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS (universal build) | Apple M1 Pro, Metal, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors (mean frame 17.4 ms). Bathhouse suite: 738 checks, 0 failures |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors, 60 fps. Bathhouse suite, including simulated Steam virtual pads and Steam Deck controllers: 752 checks, 0 failures |
| Steam Deck (hardware) | Steam Deck OLED, SteamOS 3.8, Vulkan (RADV VANGOGH), 1280 × 800, Steam Deck preset | Controls and bathhouse suite: 0 failures; the Deck's Steam Input controller is detected and bridged. Crossing, Cure, Vessel and Village walkthroughs: 0 failures, holding the display's 60 Hz. Steam Deck preset with rain reflections: 9.7 ms mean, 11.3 ms P95 |
| Graphics presets | Apple M1 Pro, Metal, 1600 × 1000 | Every preset applied and checked, 0 failures |
| Installers | DMG and Setup.exe built from the checksum-verified archives | Payloads compared file by file with their archives: 166 Mac and 173 Windows game files |
| Windows x64 | Cross-built, Direct3D 11 with Vulkan fallback | Runtime unverified |
| Intel Mac | Included in the universal app | Runtime unverified |

The Steam Deck checks ran on the hardware itself: the game's own verification modes, launched over SSH in Desktop Mode, with the Deck's controller attached. No Windows PC or Intel Mac was available.

# Haze 0.11.0 validation (earlier release)

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS (universal build) | Apple M1 Pro, Metal, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors (mean frame 17.5 ms). Bathhouse suite: 738 checks, 0 failures |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors, 60 fps. Bathhouse suite, including simulated Steam virtual pads and Steam Deck controllers: 752 checks, 0 failures |
| Steam Deck (hardware) | Steam Deck OLED, SteamOS 3.8, Vulkan (RADV VANGOGH), 1280 × 800, Steam Deck preset | Controls and bathhouse suite: 0 failures; the Deck's Steam Input controller is detected and bridged. Crossing, Cure, Vessel (26 people) and Village walkthroughs: 0 failures, holding the display's 60 Hz. Steam Deck preset: 9.5 ms mean, 12.7 ms P95 |
| Graphics presets | Apple M1 Pro, Metal, 1600 × 1000 | Every preset applied and checked, 0 failures |
| Installers | DMG and Setup.exe built from the checksum-verified archives | Payloads compared file by file with their archives: 166 Mac and 173 Windows game files |
| Windows x64 | Cross-built, Direct3D 11 with Vulkan fallback | Runtime unverified |
| Intel Mac | Included in the universal app | Runtime unverified |

The Steam Deck checks ran on the hardware itself: the game's own verification modes, launched over SSH in Desktop Mode, with the Deck's controller attached. No Windows PC or Intel Mac was available.

# Haze 0.10.0 validation (earlier release)

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS (universal build) | Apple M1 Pro, Metal, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors (mean frame 17.4 ms). Bathhouse suite: 738 checks, 0 failures |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | Whole-island walkthrough: 920 checks, 0 failures, 0 runtime errors, 60 fps. Bathhouse suite, including simulated Steam virtual pads and Steam Deck controllers: 752 checks, 0 failures |
| Graphics presets | Apple M1 Pro, Metal, 1600 × 1000 | Every preset applied and checked, 0 failures. Frame time: Steam Deck 3.7 ms, Low 2.2 ms, Medium 4.4 ms, High 8.7 ms, Ultra 10.4 ms, Cinematic 17.9 ms |
| Installers | DMG and Setup.exe built from the checksum-verified archives | Payloads compared file by file with their archives: 166 Mac and 175 Windows game files |
| Steam Deck | Linux build, Steam Deck preset | Controls verified with simulated Deck controllers on Linux; not yet run on Deck hardware |
| Windows x64 | Cross-built, Direct3D 11 with Vulkan fallback | Runtime unverified |
| Intel Mac | Included in the universal app | Runtime unverified |

The graphics verifier applies every preset, checks that the renderer really changed (render scale, anti-aliasing, shadows, AO, reflections, water, terrain, atmosphere, vegetation), photographs the same view and times it. The Linux bathhouse suite includes simulated Steam virtual pads and the Steam Deck's own controller. No physical Steam Deck or Windows PC was available.

# Haze 0.9.0 validation (earlier release)

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS, universal build | Apple M1 Pro, Metal, 1600 × 1000 | Whole-island walkthrough: 920 checks passed; zero failures or runtime errors (mean frame 16.9 ms) |
| macOS bathhouse suite | Apple M1 Pro, Metal, 1600 × 1000 | 738 checks passed; zero failures or runtime errors |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | Whole-island walkthrough: 920 checks passed; zero failures or runtime errors (mean frame 16.7 ms) |
| Linux bathhouse suite | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | 746 checks passed; zero failures or runtime errors |
| Installers | DMG and Setup.exe payloads compared with every file in their archives | 177 Mac and 175 Windows game files verified |
| Windows x64 | Cross-built for Direct3D 11 and Vulkan | Runtime unverified; no Windows test machine was available |
| Intel Mac | Included in the universal app | Runtime unverified |

## The island walkthrough

A native walkthrough drives a real first-person character controller through the whole game in story order, starting in the rowing boat: every road between the ten regions; every puzzle, including at least one deliberate wrong answer for each; every page and echo; the finale; the hidden ending, after which the bell remains; the ending; the epilogue; and the return to Morrow in the morning. Each region must load, place the visitor on solid ground, be finished by its own round, and hand over to the next region through its road. A screenshot and position are recorded for any failure.

## The bathhouse suite

The 0.4 suite still runs in full against the bathhouse, which is now Act I: puzzles, letters, sound, the developer guide, collision and recovery, inscriptions and reflections. It now also checks the new journal (rounds, island, pages, hints) and counts only the house's own 28 inscriptions, separately from the island's lettering at the north gate.

# Haze 0.4.0 validation (earlier release)

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
