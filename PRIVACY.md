# Pysano privacy notice

Policy version: 2026-10-12. Version scope: existing public versions through Beta 23 plus the locally prepared Beta 24 candidate. A new user-declaration gate is implemented only in the candidate. Maintainer/publisher account: [kairon27](https://github.com/kairon27). This notice describes the app's current technical behavior; it does not claim Google, GitHub or Hugging Face follow the same retention policy as Pysano.

## Processing on your Mac

Pysano processes microphone audio, recognized text, selected editor text and configured vocabulary to provide features you request. Accessibility captures the target app/editor, available value and selection to prevent pasting into a changed field. Input Monitoring detects configured shortcuts. These permissions do not authorize continuous audio capture or publishing messages.

Local dictation and local previews process audio on the Mac once models are downloaded. Phrase substitutions and settings are stored locally. Optional cloud actions, cloud preview speech and Auto-mode cloud routes remain cloud operations even when a local model is installed.

The Gemini key is stored in the login Keychain and held in app memory while needed. It is sent directly to Google to authenticate requests, not to a Pysano server. Session lock/sleep handling clears the in-memory credential session. Repair key access can update the Keychain item's access control only after the user invokes the repair flow and approves any macOS prompt.

## Recovery and deletion

Pysano preserves the latest completed dictation transcript in `~/Library/Application Support/Pysano/Recovery/latest-transcript.json`. A failed/interrupted recording can be preserved as `pending-dictation.wav` for Retry. These files are restricted to the macOS user (files 0600, directory 0700), but are not separately encrypted by Pysano. They may be included in your backups. The latest text persists until replaced or cleared; a pending recording persists until successful recognition or explicit discard.

Use **Latest text → Clear** to remove the saved transcript, **Discard failed recording** to remove a pending recording, **Connection → Delete key** to remove the local Keychain key, and **Delete** on a local model card to remove downloaded weights. Removing the local key does not revoke it at Google. Uninstalling only the app bundle does not remove settings, models, Keychain entries or recovery files.

Normal Live Translation keeps audio buffers and displayed translations in memory, without a Pysano audio/transcript archive. macOS logs can contain operational errors and app/device identity; Pysano's focus diagnostics omit field values, selected text, key values, keystrokes and clipboard contents. Do not assume arbitrary support screenshots or exported logs contain no private information.

## Google Gemini

Standard cloud dictation sends audio after recording. Live dictation/translation streams audio while active. Selected-text actions send the selected text and instruction. Cloud text-to-speech sends the preview text. Configured vocabulary and instructions can accompany applicable requests. Cloud usage requires an internet connection and may incur Google API charges.

Long or recovered dictation can upload audio to Google's Files API. Pysano requests deletion after recognition; deletion may fail during an interruption. Google documents automatic Files API deletion after 48 hours. `store=false` on Interactions does not override Google's terms, safety logging, temporary file retention or data-processing rules. Cancelling cannot recall data already transmitted.

Under [Google's current Gemini terms](https://ai.google.dev/gemini-api/terms), Unpaid Services may use submitted content and responses to improve products, with human review. Do not submit sensitive, confidential or personal information to Unpaid Services. Paid Services have different data-use terms, including limited safety/abuse logging. Pysano does not independently verify your Google billing tier, region or contractual eligibility.

## Other network recipients

Google receives authenticated requests and normal connection metadata. Model downloads connect to Hugging Face and its delivery infrastructure; GitHub hosts update archives and the feed. These providers can receive IP addresses and connection/request metadata under their own policies. Automatic update checks can be disabled under Updates. The Beta 24 candidate explicitly disables Sparkle system-profile submission and does not include an advertising or analytics SDK of its own.

## Rights, questions and changes

Submit a general question or a request for a private contact channel through [GitHub Issues](https://github.com/kairon27/Pysano-Updates/issues). Do not put private data into a public issue. There is currently no dedicated private support inbox advertised by this project. Do not submit sensitive material until a suitable private channel is agreed.

Applicable privacy rights and publisher-identification obligations depend on where the product is offered and on the actual processing relationship. This technical notice does not certify compliance in every jurisdiction. Before an unrestricted commercial/international rollout, the maintainer must review the required legal identification/contact details and applicable obligations. Material changes to cloud disclosures require a new in-app acknowledgement.
