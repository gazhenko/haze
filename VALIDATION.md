# Haze 0.3.2 validation

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS | Apple M1 Pro, Metal, 1600 × 1000 | 589 checks passed; zero failures or runtime errors |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | 589 checks passed; zero failures or runtime errors |
| macOS environment | Apple M1 Pro, Metal, 1600 × 1000 | 195 checks passed; zero failures or runtime errors |
| Linux fallback | NVIDIA RTX 3080, OpenGL, 1600 × 1000 | 195 environment checks passed; zero failures or runtime errors |
| Windows x64 | Cross-built for Direct3D 11 and Vulkan | Runtime unverified; no Windows test machine was available |
| Intel Mac | Included in the universal app | Runtime unverified |

## Lamps, papers, seals and brass discs

The new checks cover shade thickness, support arms, fitted fasteners, internal light placement, thin paper and desk contact, wax stamps, raised brass crests, texture completeness and finite mesh vertices. Glass seat checks measure eight points around both rims of each shade against the actual rendered metal triangles. The first candidate failed all six lanterns with 8.548 mm lower gaps; the repaired lanterns measure 0.319 mm below and 0 mm above. Sconces measure 0.634 mm below and 0 mm above. All twelve fixtures pass the 1.1 mm gap limit.

Lighting checks compare the same visible stone pixels with each point source on and off, from four camera offsets. They also confirm the sample faces the lamp and is visible past the columns. All twenty illumination and twenty sample-validity checks passed on Metal, Vulkan and OpenGL, using the existing brightness thresholds.

The full handwritten text on both physical letters matches their readable story panels. All 23 small prop texture maps were hash-checked. Paper and base metal use ambientCG CC0 sources; Caveat handwriting uses the SIL Open Font License. Credits and font licenses ship with each player.

## Gameplay and environment

The full walkthrough checks story progression, puzzle states, wrong inputs, developer-guide recovery, saved visits, collision, moving passages, inscriptions, reflections, menus, and the ending. It also checks continuous masonry beneath all ten side windows and native groundcover shaders and textures. The 80 entrance and fanlight ironwork checks still pass, including actual stone contacts and inspection for leftover floating bars.

Each full run captured 60 screenshots; each short run captured 70 views. Representative native views of the new props, ironwork, doors, planting, lighting, and interface were inspected in both lighting states. Test visits use isolated save directories. Normal player saves remained unchanged.

At a 60 FPS cap, the scripted traversal averaged 46.53 ms per frame on the Mac and 19.60 ms on Linux, with P95 values of 68.47 ms and 32.09 ms. Exterior views averaged 16.85 ms and 16.67 ms respectively. These measurements describe those machines and that route; they are not minimum hardware requirements. Dense planting retains the rendering cost introduced in 0.3.0, so similar Macs should expect a lower frame rate inside the bathhouse.

## Trailer

The trailer was recaptured from the final native release player at 1920 × 1080, with 1,260 frames at a fixed 30 FPS and no runtime errors. It includes a closer view of the keeper's papers and lantern. The complete 42-second H.264/AAC film was decoded after composition. Its stereo soundtrack uses the game's own ambience and bells. The capture frame rate is independent of normal gameplay performance.

## Package checks

Each platform archive contains the complete player, instructions, credits, and checksums. Packaging reads every archived file back and compares its bytes. The Mac signature is checked before packaging and again after extracting the completed archive. Before publication, all GitHub release assets are downloaded again and checked against the local SHA-256 values.

The Mac app is ad-hoc signed and is not Apple-notarized. Windows is unsigned. Launch instructions explain the platform prompts.

The release's `release-manifest.json` records archive hashes, executable hashes, platform status, the trailer hash, and the shared scene source fingerprint.
