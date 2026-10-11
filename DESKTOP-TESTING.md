# i+°i Windows desktop alpha testing

1. Read LICENSE-EVAL.md. Evaluation lasts 30 calendar days from first installation unless extended in writing.
2. Download the Windows x64 installer and SHA256SUMS.txt from the desktop release. Check it with `Get-FileHash -Algorithm SHA256 -LiteralPath "i2i-desktop-alpha-20261011-r6-windows-x64.exe"` and compare the complete hash.
3. Close any running older copy, install and launch i+°i — eye to eye. Setup offers folder selection, defaults to Program Files (x86)\i+°i and requires administrator approval. The installation folder contains its uninstaller; profiles are retained. R6 includes a targeted migration correction for original CCU Overlay 0.1.0. If installation fails, keep the complete error/details rather than repeatedly retrying. The runtime is included; Node.js and development tools are unnecessary.
4. Record Windows version, GPU/driver, release tag and installer hash. Check first launch, default character rendering, transparency/overlay behavior, menu interaction and window placement.
5. Try a VRM you are entitled to use; check loading, animations, expressions and presentation controls. Test backgrounds and profile save/reload. Record expected and actual results, including any unsupported or missing packaged assets.
6. Check closing/relaunching, multiple displays if available, and resource use during a representative session. Avoid enabling microphone or audio capture unless you intend to test those features and consent to that input. Current desktop code grants media permission internally when those features request it; the absence of a browser permission prompt does not mean capture is inactive.
7. File reproducible bugs in the public Issues tracker using nonconfidential material. Contact the author separately for confidential company evaluation or customization.

Alpha limitations: unsigned installer; remaining known and unknown bugs; animation/model behavior varies with assets. A successful build is not a complete Windows functionality, performance or compatibility test. The native audio helper was reused from the existing local build. Packaging checks do not establish an end-to-end audio test.

Also test dual VRM, auto camera + parallax, click/wink reactions, profile thumbnails, and an MP4 file representative of your target resolution. VR/AR and audio-input tests are optional and require intended device/input permission.

Android remains an optional preview with its own TESTING.md and release. Desktop and mobile results should be reported separately.

Release gate: verify the actual installer and installed application startup before a new desktop release. Build/archive checks alone are insufficient. Record installer hash, default model and menu graphics, animations, shortcut/uninstaller icons, selected path and profile continuity. Test migration from the prior release when applicable; distinguish developer checks, author manual acceptance and remaining feature tests.
