# Third-party notices

Hot Mic is built on these free and open-source projects. Thank you to their authors.

## AI models (downloaded on first run)

| Model | Used for | Licence | Credit |
|---|---|---|---|
| **NVIDIA Parakeet TDT 0.6B v3** (int8 ONNX export) | Speech recognition | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) | © NVIDIA Corporation. Model: <https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3>. ONNX conversion by the k2-fsa / sherpa-onnx project: <https://huggingface.co/csukuangfj/sherpa-onnx-nemo-parakeet-tdt-0.6b-v3-int8>. Converted (quantised) from the original. |
| **OpenAI Whisper large-v3-turbo** (Q5_0 GGML, optional) | Speech recognition for muffled mics | [MIT](https://github.com/openai/whisper/blob/main/LICENSE) | © OpenAI. <https://huggingface.co/openai/whisper-large-v3-turbo>. GGML conversion by the whisper.cpp project: <https://huggingface.co/ggerganov/whisper.cpp>. Converted (quantised) from the original. |
| **SpeakoFlow Mini 0.8B** (Q5_K_M GGUF) | Smart cleanup | [Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0) | © Abhishek Barali. <https://huggingface.co/SpeakoFlow/speakoflow-mini>. Fine-tuned from Qwen3.5-0.8B (Apache-2.0, © Alibaba Cloud / Qwen team). The system prompt in `SpeakoFlowPrompt.cs` is reproduced from the model card, as the model requires it verbatim. |

## Software libraries

| Library | Licence | Link |
|---|---|---|
| sherpa-onnx | Apache-2.0 | <https://github.com/k2-fsa/sherpa-onnx> |
| ONNX Runtime (bundled with sherpa-onnx) | MIT | <https://github.com/microsoft/onnxruntime> |
| LLamaSharp | MIT | <https://github.com/SciSharp/LLamaSharp> |
| llama.cpp / ggml (bundled with LLamaSharp) | MIT | <https://github.com/ggml-org/llama.cpp> |
| Velopack (the installer and self-updates) | MIT | <https://github.com/velopack/velopack> |
| Whisper.net (runs Whisper) | MIT | <https://github.com/sandrohanea/whisper.net> |
| whisper.cpp / ggml (bundled with Whisper.net) | MIT | <https://github.com/ggml-org/whisper.cpp> |
| .NET runtime and Windows Forms | MIT | <https://github.com/dotnet/runtime> |
| Microsoft Edge WebView2 SDK (draws the Settings and Welcome windows) | BSD-3-Clause | <https://www.nuget.org/packages/Microsoft.Web.WebView2> |

## Ideas and techniques

- The careful clipboard handling (private clipboard formats, delayed rendering, admin-window detection) follows the approach documented by the `win-text-inject` project.
- The two-stage cleanup design (instant rules first, then a small model) follows the SpeakoFlow Mini model card.
