# Haze 0.2.0 validation

| Platform | Tested configuration | Result |
| --- | --- | --- |
| macOS | Apple M1 Pro, Metal, 1600 × 1000 | 428 checks passed; zero failures or runtime errors |
| Linux | Omarchy, NVIDIA RTX 3080, Vulkan, 1600 × 1000 | 428 checks passed; zero failures or runtime errors |
| Linux fallback | NVIDIA RTX 3080, OpenGL, 1600 × 1000 | 34 environment checks passed; zero failures or runtime errors |
| Windows x64 | Cross-built for Direct3D 11 and Vulkan | Runtime unverified; no Windows test machine was available |
| Intel Mac | Included in the universal app | Runtime unverified |

The full walkthrough checks story progression, puzzle states, wrong inputs, developer-guide recovery, saved visits, collision, moving passages, inscriptions, reflections, menus, and the ending. It includes 20 camera-position checks of the wall lights' actual illumination and 14 checks of fixture attachments and foliage geometry. Each full native run captured 36 screenshots; representative lighting, window, landscape, and interface views were inspected.

At a 60 FPS cap, the scripted traversal averaged 26.01 ms per frame on the Mac and 16.92 ms on Linux, with P95 values of 37.50 ms and 30.68 ms. These measurements describe those machines and that route; they are not minimum hardware requirements.

## Package checks

Each platform archive contains the complete player, instructions, credits, and checksums. Packaging reads every archived file back and compares its bytes. Before publication, all GitHub release assets are downloaded again and checked against the local SHA-256 values.

The Mac app is ad-hoc signed and is not Apple-notarized. Windows is unsigned. Launch instructions explain the platform prompts.

The release's `release-manifest.json` records archive hashes, executable hashes, platform status, and the shared scene source fingerprint.
