# Haze 0.3.1 validation

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS | Apple M1 Pro, Metal, 1600 × 1000 | 519 checks passed; zero failures or runtime errors |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | 519 checks passed; zero failures or runtime errors |
| macOS environment | Apple M1 Pro, Metal, 1600 × 1000 | 125 checks passed; zero failures or runtime errors |
| Linux fallback | NVIDIA RTX 3080, OpenGL, 1600 × 1000 | 125 environment checks passed; zero failures or runtime errors |
| Windows x64 | Cross-built for Direct3D 11 and Vulkan | Runtime unverified; no Windows test machine was available |
| Intel Mac | Included in the universal app | Runtime unverified |

The new ironwork audit follows connected pieces of the rendered metal. It checks the stone contact at both ends of all 23 entrance uprights, the 15 fanlight uprights' contact with their fixed transom and arch, and the transom's bearings in the jambs. Invisible collision cannot satisfy the stone-contact checks. The saved 0.3.0 scene failed 42 of 44 baseline checks; the repaired saved scene passed all 80 checks, including an inspection of the imported metal for leftover floating bars.

The full walkthrough checks story progression, puzzle states, wrong inputs, developer-guide recovery, saved visits, collision, moving passages, inscriptions, reflections, menus, and the ending. It also checks the wall lights' actual illumination, fixture attachments, continuous masonry beneath all ten side windows, and native groundcover shaders and textures. Each full run captured 36 screenshots. The shorter environment runs each captured 46 views, including entrance-wide, threshold, arch, and fanlight views in morning and evening light. Representative native views of the ironwork, doors, planting, lighting, and interface were inspected.

At a 60 FPS cap, the scripted traversal averaged 45.84 ms per frame on the Mac and 19.20 ms on Linux, with P95 values of 66.54 ms and 31.45 ms. Exterior views averaged 16.85 ms and 16.67 ms respectively. These measurements describe those machines and that route; they are not minimum hardware requirements. The dense planting retains the rendering cost introduced in 0.3.0, so similar Macs should expect a lower frame rate inside the bathhouse.

## Trailer

The trailer was recaptured from the repaired native game at 1920 × 1080, with 1,260 frames at a fixed 30 FPS and no runtime errors. The complete 42-second H.264/AAC film was decoded after composition. Its stereo soundtrack uses the game's own ambience and bells. The capture frame rate is independent of normal gameplay performance.

## Package checks

Each platform archive contains the complete player, instructions, credits, and checksums. Packaging reads every archived file back and compares its bytes. The Mac signature is checked before packaging and again after extracting the completed archive. Before publication, all GitHub release assets are downloaded again and checked against the local SHA-256 values.

The Mac app is ad-hoc signed and is not Apple-notarized. Windows is unsigned. Launch instructions explain the platform prompts.

The release's `release-manifest.json` records archive hashes, executable hashes, platform status, the trailer hash, and the shared scene source fingerprint.
