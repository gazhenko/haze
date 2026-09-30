# Haze 0.3.0 validation

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS | Apple M1 Pro, Metal, 1600 × 1000 | 439 checks passed; zero failures or runtime errors |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | 439 checks passed; zero failures or runtime errors |
| Linux fallback | NVIDIA RTX 3080, OpenGL, 1600 × 1000 | 45 environment checks passed; zero failures or runtime errors |
| Windows x64 | Cross-built for Direct3D 11 and Vulkan | Runtime unverified; no Windows test machine was available |
| Intel Mac | Included in the universal app | Runtime unverified |

The full walkthrough checks story progression, puzzle states, wrong inputs, developer-guide recovery, saved visits, collision, moving passages, inscriptions, reflections, menus, and the ending. It includes 20 camera-position checks of the wall lights' actual illumination, fixture attachments, continuous masonry beneath all ten windows, and native groundcover shader and texture support. Each full native run captured 36 screenshots; representative lighting, window, landscape, and interface views were inspected.

At a 60 FPS cap, the scripted traversal averaged 44.02 ms per frame on the Mac and 19.23 ms on Linux, with P95 values of 68.20 ms and 31.60 ms. Exterior views averaged 16.85 ms and 16.67 ms respectively. These measurements describe those machines and that route; they are not minimum hardware requirements.

The denser planting increases rendering cost on the M1 Pro. The previous release averaged 26.01 ms; a repeat of the new walkthrough measured 45.31 ms. Players on similar Macs should expect a lower frame rate inside the bathhouse with this art update.

## Trailer

The trailer was captured from the native updated game at 1920 × 1080, with 1,260 frames at a fixed 30 FPS and no runtime errors. The complete 42-second H.264/AAC film was decoded after composition. Its soundtrack uses the game's own ambience and bells. The capture frame rate is independent of normal gameplay performance.

## Package checks

Each platform archive contains the complete player, instructions, credits, and checksums. Packaging reads every archived file back and compares its bytes. Before publication, all GitHub release assets are downloaded again and checked against the local SHA-256 values.

The Mac app is ad-hoc signed and is not Apple-notarized. Windows is unsigned. Launch instructions explain the platform prompts.

The release's `release-manifest.json` records archive hashes, executable hashes, platform status, the trailer hash, and the shared scene source fingerprint.
