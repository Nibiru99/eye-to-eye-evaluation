# i+°i Windows desktop alpha testing

1. Read LICENSE-EVAL.md. Evaluation lasts 30 calendar days from first installation unless extended in writing.
2. Download the Windows x64 installer and SHA256SUMS.txt from the desktop release. Check it with `Get-FileHash -Algorithm SHA256 -LiteralPath "i2i-desktop-alpha-20261011-r2-windows-x64.exe"` and compare the complete hash.
3. Install and launch CCU Overlay. This is the current internal application label. The runtime is included; Node.js and development tools are unnecessary.
4. Record Windows version, GPU/driver, release tag and installer hash. Check first launch, default character rendering, transparency/overlay behavior, menu interaction and window placement.
5. Try a VRM you are entitled to use; check loading, animations, expressions and presentation controls. Test backgrounds and profile save/reload. Record expected and actual results, including any unsupported or missing packaged assets.
6. Check closing/relaunching, multiple displays if available, and resource use during a representative session. Avoid enabling microphone or audio capture unless you intend to test those features and consent to that input. Current desktop code grants media permission internally when those features request it; the absence of a browser permission prompt does not mean capture is inactive.
7. File reproducible bugs in the public Issues tracker using nonconfidential material. Contact the author separately for confidential company evaluation or customization.

Alpha limitations: unsigned installer; internal development app label; remaining known and unknown bugs; animation/model behavior varies with assets. A successful build is not a complete Windows functionality, performance or compatibility test. The native audio helper was reused from the existing local build. Packaging checks do not establish an end-to-end audio test.

Also test dual VRM, auto camera + parallax, click/wink reactions, profile thumbnails, and an MP4 file representative of your target resolution. VR/AR and audio-input tests are optional and require intended device/input permission.

Android remains an optional preview with its own TESTING.md and release. Desktop and mobile results should be reported separately.
