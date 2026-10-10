# Android mobile alpha/demo testing

This is an existing debug-signed Android build dated 2026-08-30. The owner describes it as functional with remaining bugs. It is offered for testing platform fit, usability and behavior; no production-readiness claim is made.

## Installation

Download the APK from the release assets and compare it with SHA256SUMS.txt. Install it on a test device compatible with minimum API 24. Android may require permission for the browser or file manager to install this APK. Grant that permission deliberately for this installation.

If Android reports an incompatible existing installation, record the message first. A different signing certificate may prevent an in-place update. Preserve existing profiles before choosing to uninstall; uninstalling can remove app data.

## Test sequence

1. Record phone model, Android version, APK hash and whether this is a fresh installation or update.
2. Confirm first launch, character rendering, navigation and the functions available in this build.
3. Test portrait/landscape changes, switching away and back, and profile restoration after closing/reopening.
4. Try the available presentation modes and characterize their actual behavior on this device. Report split-screen, overlay or capture behavior separately.
5. Test optional audio/camera/capture features only when needed. Check their permission prompts, and confirm basic navigation remains usable when permissions are declined.
6. Record crashes, rendering faults, animation issues, heat/battery behavior, and interface difficulties with reproduction steps.

The APK declares camera, audio recording, network, foreground media projection and overlay permissions. Declaration does not mean each feature is active or proven functional. Device permission and capture consent remain under the tester's control.

## Feedback

Report the build/hash, device and Android version, steps, expected behavior and actual behavior. Screenshots or short recordings are useful when they contain no private messages, faces or other personal information. Use the evaluation repository's issue tracker after it is created.

Company feedback can also identify desired colors, functions, removals or integrations. Those requests can become a separately agreed customization or integration scope. Evaluation feedback does not itself authorize production use or redistribution.
