# Third-party notices

Pysano's own binary-use terms do not replace or restrict the rights granted by these licenses. Full copyright, permission and disclaimer texts are provided in the linked files, also included inside each newly prepared app bundle. The table describes Beta 38, with previous versions recorded where applicable. Upstream versions are pinned in Package.resolved.

| Incorporated component | Version / license | Full notices |
|---|---|---|
| Argmax OSS / WhisperKit / ArgmaxCore | 1.1.0, MIT; incorporated swift-transformers portions under Apache 2.0 | [MIT](licenses/Argmax-MIT.txt), [Argmax third-party notices](licenses/Argmax-NOTICES.txt) |
| FluidAudio | 0.18.3 in Beta 38; 0.18.0 in published Beta 29–37; 0.17.7 in Beta 26/28; 0.15.6 in Beta 24/25, Apache 2.0 | [Full license](licenses/FluidAudio-Apache-2.0.txt) |
| FluidAudio FastClusterWrapper | BSD, upstream fastcluster | [Copyright, conditions and disclaimer](licenses/FluidAudio-Fastcluster-BSD.txt) |
| FluidAudio NemoTextProcessing / text-processing-rs | v0.3.1 binary in Beta 26; v0.3.0 in Beta 24/25, Apache 2.0 and MIT incorporated works | [Third-party notices](licenses/FluidAudio-NemoTextProcessing-NOTICES.md), [Apache 2.0](licenses/FluidAudio-Apache-2.0.txt), [Rust port license](licenses/NemoTextProcessing-Rust-LICENSES.txt), [Rust NOTICE](licenses/NemoTextProcessing-Rust-NOTICE.txt), [dependency license texts](licenses/NemoTextProcessing-Rust-Dependencies.txt) |
| FluidAudio incorporated VBX work | Apache 2.0 | [Full license](licenses/FluidAudio-VBX-Apache-2.0.txt) |
| Sparkle and incorporated components | 2.10.0 in Beta 26; 2.9.2 in public Beta 23, MIT and included BSD/MIT notices | [2.10.0 full notices](licenses/Sparkle-LICENSE.txt), [2.9.2 full notices](licenses/Sparkle-2.9.2-LICENSE.txt) |

Full model attribution and licensing information is in [MODEL_LICENSES.md](MODEL_LICENSES.md). We include a tooling notice for [swift-argument-parser](licenses/SwiftArgumentParser-Apache-2.0.txt) (1.8.2, Apache 2.0); presence here does not claim its command-line tooling is part of the shipped Pysano executable.

The Typewriter feedback sounds use edited excerpts of [Typewriter snippet 02](https://freesound.org/people/cabled_mess/sounds/360602/) and [Typewriter snippet 03](https://freesound.org/people/cabled_mess/sounds/360601/) by cabled_mess, released under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).

The Gaming Keyboard feedback sounds use edited excerpts of [Keyboard - Press down](https://freesound.org/people/Foxfire-/sounds/570754/) and [Keyboard - Key release](https://freesound.org/people/Foxfire-/sounds/570755/) by Foxfire-, also released under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).

The Toggle Switch and Wood Tap feedback sounds use edited excerpts of [Small Toggle Switch](https://freesound.org/people/loganzsound/sounds/877305/) by loganzsound and [Random Wooden Stick Foley](https://freesound.org/people/deadrobotmusic/sounds/609943/) by deadrobotmusic, respectively. Both recordings are released under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).

The Mellow Tap feedback sounds are adapted from [Woodblock-soft.wav](https://freesound.org/people/hollandm/sounds/692828/) by hollandm, released under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).

The Water Drop feedback sounds are adapted from [Water drops 1.wav](https://freesound.org/people/Zaziesound/sounds/496306/) by Zaziesound, released under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).

Existing archives through Beta 23 predate this bundled notices directory. Their byte contents and published hashes are not silently changed. The accompanying notices cover Beta 23 libraries and Beta 26; earlier releases can contain different versions or fewer components. Newly prepared binaries include their notices directly.

The optional local AI workers for summaries, text actions, dictation proofreading and screenshot questions bundle llama.cpp b11669 under MIT: [full copyright and license](licenses/llama.cpp-MIT.txt). They are launched only with installed local GGUF weights, without a server. Voicetypr was reviewed as a reference; its AGPL source code is not incorporated.
