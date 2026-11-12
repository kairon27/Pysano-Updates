# Model provenance and licenses

Weights are downloaded separately from Hugging Face and are not included in the application ZIP. Library licensing is separate from model licensing. No affiliation or endorsement is implied.

| Model | Provider / original author | Pinned source | License information |
|---|---|---|---|
| Whisper Large v3 Turbo, compressed and full Core ML variants | OpenAI; Core ML conversion/distribution by Argmax | [Argmax revision 0f63a780](https://huggingface.co/argmaxinc/whisperkit-coreml/tree/0f63a7800b00dd0226abd051b906c246e1907482); [OpenAI tokenizer revision 41f01f3f](https://huggingface.co/openai/whisper-large-v3-turbo/tree/41f01f3fe87f28c78e2fbf8b568835947dd65ed9) | MIT as declared by the providers; [OpenAI notice](licenses/Whisper-OpenAI-MIT.txt) and [Argmax notice](licenses/Argmax-MIT.txt). |
| Parakeet TDT 0.6B v3 Core ML | NVIDIA; conversion/distribution by Fluid Inference | [Fluid Inference revision 7dd20fe6](https://huggingface.co/FluidInference/parakeet-tdt-0.6b-v3-coreml/tree/7dd20fe6b1797d35f5e3307e8b1732d9a178edfe) | The card metadata and [original NVIDIA model](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3) declare CC BY 4.0. The Core ML card body also says Apache 2.0. This discrepancy remains unresolved; Pysano preserves both notices and does not claim the conversion relicenses the original model. |

Parakeet attribution: NVIDIA, parakeet-tdt-0.6b-v3; adapted to Core ML by Fluid Inference. [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) ([full text](licenses/CC-BY-4.0.txt)). Pysano consumes the supplied converted models without claiming authorship of the weights. Attribution does not imply endorsement. The weight files remain usable under their own license, independently of the Pysano binary-use terms.

The application verifies downloaded file sizes and SHA-256 values against its pinned catalog. Those checks verify file integrity, not the legal validity of a provider's license declaration. The provider discrepancy requires clarification before claiming a complete model-license clearance.

## Beta 26 local additions

- **Parakeet Ultra:** NVIDIA original Parakeet, post-training by Moondream, Core ML distribution by Fluid Inference. CC BY 4.0 attribution is retained. [Pinned conversion](https://huggingface.co/FluidInference/parakeet-ultra-coreml/tree/95eaa59a39d4394f047a4dc5cce480388a60d1b6), [Moondream model](https://huggingface.co/moondream/parakeet-ultra).
- **Qwen3.5-4B Q4_K_M and optional F16 vision projector:** Qwen Team/Alibaba; GGUF conversion by Unsloth. Apache 2.0 as declared by providers. [Pinned weights and projector](https://huggingface.co/unsloth/Qwen3.5-4B-GGUF/tree/e87f176479d0855a907a41277aca2f8ee7a09523).
- **Gemma 4 E4B QAT Q4_0 and optional vision projector:** Google DeepMind; official GGUF distribution. Apache 2.0 as declared by provider. [Pinned weights and projector](https://huggingface.co/google/gemma-4-E4B-it-qat-q4_0-gguf/tree/4b4a2c1d584be7264f87aac328a1bc739ce81b6c).
- **Lapa v0.1.2 Instruct Q4_K_M:** Lapa LLM team, based on Google Gemma 3 12B; official Lapa GGUF. Governed by [Gemma terms](https://ai.google.dev/gemma/terms), not Apache 2.0. [Pinned weights](https://huggingface.co/lapa-llm/lapa-v0.1.2-instruct-GGUF/tree/1a30af6ad6341770e84e0eb51c27d86b6bf60b41). This is the published GGUF v0.1.2, not a claimed conversion of v0.1.3.

These weights remain separate downloads and are not included in the app ZIP. Downloads use immutable revisions and SHA-256 validation. Summary text and audio are never uploaded to a model provider by the local summary path.

## Beta 29 local additions

- **Parakeet UK v3:** NVIDIA Parakeet TDT 0.6B v3, Ukrainian fine-tuning by Yuri Ihnatov. CC BY 4.0. The supplied Core ML int8 conversion is consumed unchanged. [Pinned model, attribution, limitations and training-data disclosure](https://huggingface.co/ihnatov-yuri/parakeet-tdt-0.6b-v3-uk/tree/5c4bcfaca501587beaedfd23b72a678bf7194de1). The pinned revision is the provider’s version 3 (30 October 2026); its internal config version is `uk_v5`. The legacy storage ID is retained for existing installations.
- **Nemotron Unified ASR 0.6B:** NVIDIA; unofficial Core ML conversion by Fluid Inference. [OpenMDW License 1.1 and NVIDIA notice](licenses/Nemotron-OpenMDW-1.1.md). [Pinned conversion](https://huggingface.co/FluidInference/nemotron-labs-unified-asr-0.6b-coreml/tree/bd13ddde81d3134719c520845346b3252daf3175), [original model](https://huggingface.co/nvidia/nemotron-labs-unified-asr-0.6b). Pysano uses the offline int8 encoder with the decoder, joint and vocabulary from the same revision. Streaming exports are not downloaded by this package. No NVIDIA or Apple affiliation or endorsement is implied.

## Beta 37 local additions

- **Qwen3.5-9B Q4_K_M and optional F16 vision projector:** Qwen Team/Alibaba; GGUF conversion by Unsloth. Apache 2.0. [Pinned weights and projector](https://huggingface.co/unsloth/Qwen3.5-9B-GGUF/tree/3885219b6810b007914f3a7950a8d1b469d598a5).
- **Qwen3.5-27B Q4_K_M and optional F16 vision projector:** Qwen Team/Alibaba; GGUF conversion by Unsloth. Apache 2.0. [Pinned weights and projector](https://huggingface.co/unsloth/Qwen3.5-27B-GGUF/tree/3221f178a6b842d04f1fb42f1c413534adcc0a6a).

## Beta 38 local ASR additions

- **Parakeet ReDux:** NVIDIA Parakeet TDT v3, ternary retraining by Moondream, Core ML conversion by Fluid Inference. CC BY 4.0 as declared by the provider. [Pinned conversion and attribution](https://huggingface.co/FluidInference/parakeet-redux-coreml/tree/8c5ef97a29cd120dc76b354b3f22b7fec3b486f9), [Moondream original](https://huggingface.co/moondream/parakeet-redux). Pysano consumes the converted components unchanged and uses a GPU encoder configuration.
- **Phonon 2.5 multilingual:** based on NVIDIA Parakeet TDT v3, retraining/compression by Fermion Research, Core ML conversion by Muesli-HQ. CC BY 4.0 weights. [Pinned conversion, full notices and licenses](https://huggingface.co/Muesli-HQ/phonon-2.5-coreml/tree/a042ef89966d289df295709b58ffdabb50bd2510), [Fermion model](https://huggingface.co/FermionResearch/Phonon-2.5), [retained original NOTICE](licenses/Phonon-2.5-NOTICE.txt). Each download includes the original NOTICE and weight/code license files. The provider's NOTICE is retained verbatim; its runtime list describes the provider implementation. Pysano runs the compiled Core ML exports through FluidAudio.

- **Canary 1B v2:** [NVIDIA original model](https://huggingface.co/nvidia/canary-1b-v2) and [Fluid Inference int4 Core ML conversion](https://huggingface.co/FluidInference/canary-1b-v2-coreml/tree/224631d3724c8f34c2d4d99b92e7e26cd6d2f93b), CC BY 4.0. Pysano uses the supplied components with GPU execution and transcription prompts.

These models are separate weight downloads for macOS 15 or later. Each package uses an immutable revision with SHA256 validation. ReDux is labelled compact. Phonon and Canary are labelled experimental.
