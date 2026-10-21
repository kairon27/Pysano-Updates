# Known issues and beta acceptance

Release scope: experimental Beta 26, build 40. A release is available only when it appears in Releases and the signed feed. Beta 24/25 were local candidates rather than separate public releases.

- Experimental public builds, including Beta 26, use the established local signing certificate and are not Developer ID notarized. Sparkle EdDSA verification remains enabled. Fresh installation can fail normal Gatekeeper assessment. Standard notarized distribution remains pending a Developer ID certificate, hardened-runtime testing and Apple notarization.
- Local meeting summaries are AI drafts. Exact source-quote checks do not establish semantic correctness, speaker identity, ownership or complete task extraction. Short Ukrainian probes and an accelerated one-hour journal/export test passed; actual sustained 30–60 minute capture still needs acceptance testing. Summary weights require a separate download and several GB of storage/memory.
- Repeated final-transcript insertion in Telegram, Codex and browser editors is not fully accepted. A failed paste keeps text recoverable but may require manual copying. An unconfirmed paste must not be repeated automatically, because it may already have reached the editor.
- Sustained Live Translation, actual output-device loopback and two-way meeting routing still need live testing. Use an appropriate headset and watch the source, translated signal and reconnection gap indicators. Interrupted phrases can require repetition.
- The supplied binary is arm64, not Intel. Compatibility is not physically verified on every supported macOS version or audio device.
- A changed signing identity can require renewed macOS permissions or Keychain access. Do not reset unrelated permissions or delete recovery data to resolve this.
- Google availability, supported regions, billing, preview model behavior and quotas can change. Own-key use does not waive platform terms.
- The Parakeet Core ML model card contains conflicting CC BY 4.0 / Apache 2.0 declarations; see MODEL_LICENSES.md.

Before a broad release, test fresh installation and upgrades on other Macs; permission denial/revocation; Keychain recovery without key loss; repeated dictation into several editors; switching field/window while transcription is pending; password fields; clipboard restoration and delayed paste; silent/noisy input; model download/resume and offline dictation; sleep/network/audio-device interruptions; both translation directions; and signed updater installation.

Automated checks and signature/hash verification do not replace this acceptance matrix or a legal review.
