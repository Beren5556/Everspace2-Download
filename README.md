# EVERSPACE 2 VR — Lite 0.9 Beta

## Downloads

Download **both** files from [Releases](https://github.com/Beren5556/Everspace2-Download/releases/tag/v0.9.0-beta):

1. **[UEVR-ES2-Lite-0.9-Beta.zip](https://github.com/Beren5556/Everspace2-Download/releases/download/v0.9.0-beta/UEVR-ES2-Lite-0.9-Beta.zip)** — UEVR injector and required libraries.
2. **[ES2-Win64-Shipping.zip](https://github.com/Beren5556/Everspace2-Download/releases/download/v0.9.0-beta/ES2-Win64-Shipping.zip)** — the EVERSPACE 2 VR profile.

## Requirements

- Windows 10 or Windows 11, 64-bit.
- The **Steam version of EVERSPACE 2**, running in **DirectX 11**.
- A VR headset connected through a working **OpenXR runtime**.
- The **UEVR build provided above**. Use it together with this profile.
- The Microsoft runtime requested by the UEVR injector, if it is not already installed. Follow the injector's download prompt.

This beta supports DX11 and OpenXR. DX12 and other game-store versions are not supported.

## Installation

1. Close the game and UEVR. If a profile already exists, enter `%APPDATA%\UnrealVRMod` in File Explorer's address bar and move the `ES2-Win64-Shipping` folder to a backup location outside that directory. Do not merge profiles.
2. Extract **UEVR-ES2-Lite-0.9-Beta.zip** into a new folder. Keep all its files together.
3. Open Steam, right-click **EVERSPACE 2 → Properties**, and add **`-dx11`** to **Launch Options**. Remove a conflicting `-dx12` option if present.
4. Connect your headset, start its OpenXR runtime as usual, and launch EVERSPACE 2 from Steam.
5. Run **UEVRInjector.exe** from the extracted UEVR folder and select **ES2-Win64-Shipping.exe** in the process list.
6. Use the injector's **Import Config** option and select **ES2-Win64-Shipping.zip**. Keep the profile ZIP compressed for this step.
7. In the injector, choose **OpenXR** and click **Inject**.
8. Load your game. The profile applies automatically.

Nothing needs to be copied into the game's installation folder. No commands or installation scripts are required. To play normally without VR, start the game without injecting UEVR.
