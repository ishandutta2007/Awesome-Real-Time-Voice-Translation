# Awesome-Real-Time-Voice-Translation

## Real-Time Voice Translation Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on AI-Powered Real-Time Speech-to-Speech & Voice Translation*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** building **real-time voice translation** solutions. These tools enable live interpretation during conversations, meetings, conferences, calls, and events by performing speech recognition, translation, and speech synthesis with low latency.

**Examples** include Palabra.ai, Maestra AI, Wordly.ai, Talo, DeepL Voice, Interprefy, Timekettle X1, and KUDO AI (the category leaders). Tools listed here emphasize **agentic and low-latency capabilities** (streaming translation, multi-speaker support, natural prosody, offline modes, and high-accuracy interpretation for 50+ languages).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, local LLMs, offline voice translation, custom pipelines, and full privacy control — ideal for developers, enterprises, and privacy-conscious users building their own real-time translation systems.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS Products](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS Products

### Core Platforms (Real-Time Voice Translation)

| SaaS Product | Description | Pricing | Free Tier / Trial Limits |
| :--- | :--- | :--- | :--- |
| **[Palabra.ai](https://palabra.ai/)** | AI-powered real-time voice translation optimized for conversations, meetings, and events. | **Starter:** $60/mo for 3h<br>**Pro:** $200/mo for 10h<br>**Team:** $1000/mo for 50h | **Free Trial:** Limited daily minutes to test latency/cloning. |
| **[Maestra AI](https://maestra.ai/)** | Comprehensive platform for real-time speech-to-speech, transcription, and subtitles. | **Pay-As-You-Go:** $0.20/min<br>**Lite:** $23/mo (180 mins)<br>**Premium:** $79/mo (900 mins) | **Free Trial:** 30 minutes of free transcription/translation. |
| **[Wordly.ai](https://wordly.ai/)** | Enterprise-grade interpretation for conferences and large events. | **Starter:** ~$75/hour<br>Custom quotes for large packages. | **Free Trial:** Available upon request. |
| **[Talo](https://talo.ai/)** | Low-latency solution focused on natural conversation flow. | **Starter:** $33/mo (95 mins)<br>**Pro:** $80/mo (400 mins)<br>**Team:** $400/mo | **Free Trial:** 7-day trial with 200 minutes. |
| **[DeepL Voice](https://www.deepl.com/)** | High-accuracy voice translation using the DeepL engine. | **Custom:** Contact sales for Voice API pricing. | **Free Tier:** 50k chars/mo for Translator (not Voice). |
| **[Interprefy](https://interprefy.com/)** | Professional remote interpretation for high-stakes multilingual events. | **Custom:** Based on duration and complexity. | **Free Tier:** Demos available on request. |
| **[Timekettle X1](https://www.timekettle.co/)** | Hardware + AI hybrid for two-way translation (earbuds/device). | **Hardware:** $699.99 (Standalone device) | **N/A:** Hardware purchase; no recurring sub for core features. |
| **[KUDO AI](https://www.kudo.ai/)** | AI simultaneous interpretation for business communication. | **Subscription:** Tiered packages (75h to 1,000h per year). | **Free Tier:** 10 minutes of live transcription for testing. |

### Advanced & Specialized Platforms

| Service | Description | Pricing (per 1M characters) | Free Tier Limits |
| :--- | :--- | :--- | :--- |
| **[Google Translate Live](https://cloud.google.com/translate)** | Standard NMT for apps and streaming. | $20.00 | 500,000 characters per month |
| **[Microsoft Translator](https://azure.microsoft.com/en-us/products/ai-services/ai-translator)** | Azure-based translation with broad language support. | $10.00 | 2,000,000 characters per month |
| **[iTranslate](https://www.itranslate.com/)** | Consumer app and enterprise-level translation. | **Consumer:** $5.99/mo (Pro)<br>**API:** Custom Enterprise | Limited free version for app users. |

## Open-Source GitHub Projects

### Dedicated Real-Time Voice Translation Projects

- **[Seamless Communication (Meta)](https://github.com/facebookresearch/seamless_communication)**  
  State-of-the-art open-source SeamlessM4T model family for speech-to-speech, speech-to-text, text-to-speech, and text-to-text translation supporting 100+ languages. Excellent for building real-time systems.

- **[faster-whisper + NLLB / Seamless pipelines](https://github.com/SYSTRAN/faster-whisper)**  
  High-performance Whisper implementation optimized for speed. Widely used as the foundation for real-time speech-to-text + translation pipelines.

- **[Live-Translate](https://github.com/ahmetoner/whisper-asr-websocket)** + translation extensions  
  Real-time speech recognition server with WebSocket support, easily combined with translation models for live voice translation.

- **[Coqui TTS / Tortoise TTS](https://github.com/coqui-ai/TTS)**  
  High-quality open-source text-to-speech models that can be paired with translation models for natural voice output in target languages.

- **[Piper TTS](https://github.com/rhasspy/piper)**  
  Fast, local neural text-to-speech system optimized for real-time performance on edge devices.

- **[OpenVoice](https://github.com/myshell-ai/OpenVoice)**  
  Instant voice cloning and real-time voice conversion toolkit that can be integrated into translation pipelines for natural prosody.

- **[Vosk API](https://github.com/alphacep/vosk-api)**  
  Lightweight offline speech recognition toolkit supporting 20+ languages. Excellent for on-device real-time translation.

- **[whisper-live](https://github.com/collabora/WhisperLive)**  
  Real-time whisper-based transcription server designed for low-latency streaming applications.

### Additional Strong Open-Source Options

- **[Meta MMS (Massively Multilingual Speech)](https://github.com/facebookresearch/fairseq/tree/main/examples/mms)** — Large collection of speech models for 1,000+ languages.
- **[NVIDIA NeMo](https://github.com/NVIDIA/NeMo)** — Toolkit for building ASR, TTS, and translation models with excellent real-time support.
- **[SpeechBrain](https://github.com/speechbrain/speechbrain)** — PyTorch-based toolkit for speech processing including translation pipelines.
- **[Rhasspy / Mycroft](https://github.com/rhasspy)** — Offline voice assistant frameworks that can be extended for translation.
- **Custom Pipelines**: Many community repos combining `faster-whisper` + `transformers` (NLLB/Seamless) + `Piper TTS` for full speech-to-speech translation.
- Edge-optimized projects using ONNX Runtime, TensorRT-LLM, or llama.cpp for running translation models locally.

**Frameworks for building custom agents**: Use **Faster-Whisper + SeamlessM4T + Piper TTS** with **LangGraph** or **Streaming pipelines** (WebSockets, WebRTC) for low-latency, self-hosted real-time voice translation systems. Combine with **Silero VAD** for voice activity detection and **DeepFilterNet** for noise suppression.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Real-time translation accuracy varies by language pair, accent, and audio quality. Always verify critical communications manually, especially in medical, legal, or high-stakes scenarios.
- When self-hosting open-source solutions, ensure sufficient hardware (GPU recommended for best performance) and respect privacy regulations (GDPR, etc.).

---

**Made for interpreters, event organizers, global teams, developers, and accessibility advocates.**  
Let's make real-time voice translation more accurate, private, and accessible to everyone.


## 📈 Star History

<div align="center">
  <a href="https://www.star-history.com/?repos=ishandutta2007%2FAwesome-Real-Time-Voice-Translation&type=date&legend=bottom-right">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/Awesome-Real-Time-Voice-Translation&type=date&theme=dark&legend=bottom-right" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/Awesome-Real-Time-Voice-Translation&type=date&legend=bottom-right" />
      <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/Awesome-Real-Time-Voice-Translation&type=date&legend=bottom-right" />
    </picture>
  </a>
</div>

