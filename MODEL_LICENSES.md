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
- **Qwen3.5-4B Q4_K_M:** Qwen Team/Alibaba; GGUF conversion by Unsloth. Apache 2.0 as declared by providers. [Pinned weights](https://huggingface.co/unsloth/Qwen3.5-4B-GGUF/tree/e87f176479d0855a907a41277aca2f8ee7a09523).
- **Gemma 4 E4B QAT Q4_0:** Google DeepMind; official GGUF distribution. Apache 2.0 as declared by provider. [Pinned weights](https://huggingface.co/google/gemma-4-E4B-it-qat-q4_0-gguf/tree/4b4a2c1d584be7264f87aac328a1bc739ce81b6c).
- **Lapa v0.1.2 Instruct Q4_K_M:** Lapa LLM team, based on Google Gemma 3 12B; official Lapa GGUF. Governed by [Gemma terms](https://ai.google.dev/gemma/terms), not Apache 2.0. [Pinned weights](https://huggingface.co/lapa-llm/lapa-v0.1.2-instruct-GGUF/tree/1a30af6ad6341770e84e0eb51c27d86b6bf60b41). This is the published GGUF v0.1.2, not a claimed conversion of v0.1.3.

These weights remain separate downloads and are not included in the app ZIP. Downloads use immutable revisions and SHA-256 validation. Summary text and audio are never uploaded to a model provider by the local summary path.
