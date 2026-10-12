# Pysano Updates

Pysano is an independent macOS dictation and translation app. This public repository distributes application binaries and the Sparkle update feed. The source repository is private; the automatic GitHub **Source code.zip** contains only this update repository, not the application source.

## Download and requirements

Download **Pysano-<version>.zip** from [Releases](https://github.com/kairon27/Pysano-Updates/releases), extract it and move Pysano.app to Applications. The distributed application requires **Apple Silicon and macOS 14 or later**; process-audio translation additionally requires macOS 14.2 or later. Intel is not supported by the supplied binary.

Existing published builds through Beta 23 use a local signing certificate and are **not Developer ID notarized**. A valid local code signature and Sparkle signature do not mean Apple has approved the app. A fresh Mac may block installation through Gatekeeper. We do not recommend disabling Gatekeeper or changing system-wide trust settings.

Beta releases are experimental. The privacy/eligibility acknowledgement and bundled notices are implemented in the prepared Beta 24 candidate; existing publicly released versions through Beta 23 do not enforce that acknowledgement. Users of existing versions remain responsible for Google eligibility and data-use rules. In Pysano, enable **Updates → Receive beta releases** to receive betas. Stable users do not receive beta updates by default. Latest does not necessarily mean Stable; check the prerelease label. The last published Stable version is 0.7.1.

## Local and cloud operation

Local dictation uses separately downloaded models and processes speech on this Mac. Optional selected-text actions and preview speech can still use Google even with a local dictation model. Auto mode can switch between a local and a cloud recognizer based on power settings. Live Translation uses Gemini, except the explicitly selected local microphone pass-through route.

Cloud features are intended for **adult professional/business users** and require the user's own eligible Gemini API project. Google restricts supported regions and requires Paid Services for API clients made available to users in the EEA, Switzerland and the UK. Personal API keys do not waive Google's terms. API usage can incur charges billed by Google to the user's project; Pysano supplies no shared API key or quota.

Read [Privacy](PRIVACY.md), [Terms](TERMS.md), [Model licenses](MODEL_LICENSES.md), [Third-party notices](THIRD_PARTY_NOTICES.md) and [Known issues](KNOWN_ISSUES.md) before use. Pysano is not affiliated with or endorsed by Apple, Google, NVIDIA, Argmax or Fluid Inference.

## Permissions and support

Microphone records speech on command; Accessibility reads the focused editor and sends Paste; Input Monitoring receives configured global hotkeys. Grant permissions only to the installed Applications copy. A signing change may require macOS consent again; Pysano cannot silently grant permissions.

Review recognized text before using it. Record/capture other people or protected content only when you have the necessary rights and any required consent. See [Known issues](KNOWN_ISSUES.md) for acceptance-test limits.

Use [Issues](https://github.com/kairon27/Pysano-Updates/issues) for general support. Do not publish API keys, passwords, recordings, private transcripts or personal information. For a sensitive security issue, follow [SECURITY.md](SECURITY.md).

## Verification and history

Release notes include an archive SHA-256. Sparkle verifies signed update archives before installation. Recent release notes also identify the private source commit, which is a provenance identifier, not a public source-code link. Update-repository tags identify publication metadata, not private source commits.

The feed is [appcast.xml](https://github.com/kairon27/Pysano-Updates/blob/main/appcast.xml). Previously downloaded archives remain immutable; corrected binaries are shipped under a new version. SHA-256 and signature verification are integrity checks, not a legal audit or proof of compatibility with every Mac/editor.
