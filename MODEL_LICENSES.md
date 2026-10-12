# Model provenance and licenses

Weights are downloaded separately from Hugging Face and are not included in the application ZIP. Library licensing is separate from model licensing. No affiliation or endorsement is implied.

| Model | Provider / original author | Pinned source | License information |
|---|---|---|---|
| Whisper Large v3 Turbo, compressed and full Core ML variants | OpenAI; Core ML conversion/distribution by Argmax | [Argmax revision 0f63a780](https://huggingface.co/argmaxinc/whisperkit-coreml/tree/0f63a7800b00dd0226abd051b906c246e1907482); [OpenAI tokenizer revision 41f01f3f](https://huggingface.co/openai/whisper-large-v3-turbo/tree/41f01f3fe87f28c78e2fbf8b568835947dd65ed9) | MIT as declared by the providers; [OpenAI notice](licenses/Whisper-OpenAI-MIT.txt) and [Argmax notice](licenses/Argmax-MIT.txt). |
| Parakeet TDT 0.6B v3 Core ML | NVIDIA; conversion/distribution by Fluid Inference | [Fluid Inference revision 7dd20fe6](https://huggingface.co/FluidInference/parakeet-tdt-0.6b-v3-coreml/tree/7dd20fe6b1797d35f5e3307e8b1732d9a178edfe) | The card metadata and [original NVIDIA model](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3) declare CC BY 4.0. The Core ML card body also says Apache 2.0. This discrepancy remains unresolved; Pysano preserves both notices and does not claim the conversion relicenses the original model. |

Parakeet attribution: NVIDIA, parakeet-tdt-0.6b-v3; adapted to Core ML by Fluid Inference. [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) ([full text](licenses/CC-BY-4.0.txt)). Pysano consumes the supplied converted models without claiming authorship of the weights. Attribution does not imply endorsement. The weight files remain usable under their own license, independently of the Pysano binary-use terms.

The application verifies downloaded file sizes and SHA-256 values against its pinned catalog. Those checks verify file integrity, not the legal validity of a provider's license declaration. The provider discrepancy requires clarification before claiming a complete model-license clearance.
