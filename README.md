# EVERSPACE 2 VR — Lite 0.9.1

## Downloads

This candidate is awaiting an in-game test. While signed in with repository owner access, open [Releases](https://github.com/Beren5556/Everspace2-Download/releases), select **EVERSPACE 2 VR Lite 0.9.1** marked **Draft**, and download **both** attached ZIP files:

1. **UEVR-ES2-Lite-0.9.1.zip** — UEVR injector and required libraries.
2. **ES2-Win64-Shipping.zip** — the EVERSPACE 2 VR profile. Keep it compressed for import.

## Requirements

- Windows 10 or Windows 11, 64-bit.
- The **Steam version of EVERSPACE 2**, running in **DirectX 11**.
- A connected VR headset with a working **OpenXR runtime**.
- The UEVR build supplied with this profile.
- The Microsoft runtime requested by the injector, if needed; follow its download prompt.

This build supports DX11 and OpenXR. The plugin checks the supported Steam executable and refuses incompatible builds. DX12 and other game-store versions are unsupported.

## Installation

1. Close the game and UEVR. If a profile exists, enter `%APPDATA%\UnrealVRMod` in File Explorer and move `ES2-Win64-Shipping` to a backup location outside that directory. Start with a clean profile; do not merge profiles.
2. Extract **UEVR-ES2-Lite-0.9.1.zip** into a new folder. Keep all its files together.
3. In Steam, right-click **EVERSPACE 2 → Properties** and add **`-dx11`** to **Launch Options**. Remove a conflicting `-dx12` option.
4. Connect the headset, start its OpenXR runtime and launch EVERSPACE 2 from Steam.
5. Run **UEVRInjector.exe** from the new UEVR folder and select **ES2-Win64-Shipping.exe**.
6. Choose **Import Config** and select **ES2-Win64-Shipping.zip**.
7. Select **OpenXR**, click **Inject** and load your game. The profile applies automatically.

Nothing needs to be copied into the game's installation folder. To play without VR, start the game without injecting UEVR. To restore an earlier profile, close the game and UEVR, move the Lite profile out of `UnrealVRMod`, and restore your backup folder.

## Credits and UEVR version

- **[Pande4360](https://github.com/Pande4360)** — creator of the original EVERSPACE 2 VR profile on which this profile is based.
- **[Joey](https://github.com/joeyhodge/UEVR)** — author of the UEVR version used and forked for this adaptation.
- **[praydog and the UEVR contributors](https://github.com/praydog/UEVR)** — creators of the original UEVR framework.

The bundled UEVR is a modified build based on **joeyhodge/UEVR**, branch **ue57performance**, commit **[738976660f1297f752be27a4f08d28ec5a60c2c2](https://github.com/joeyhodge/UEVR/commit/738976660f1297f752be27a4f08d28ec5a60c2c2)** (4 October 2026).

UEVR's [main license](https://github.com/joeyhodge/UEVR/blob/738976660f1297f752be27a4f08d28ec5a60c2c2/LICENSE) states **All rights reserved**. Its [plugin SDK has a separate MIT license](https://github.com/joeyhodge/UEVR/blob/738976660f1297f752be27a4f08d28ec5a60c2c2/include/LICENSE). Exact third-party license notices are included in the UEVR ZIP.
