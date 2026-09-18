# Awesome Voice Typing

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](CONTRIBUTING.md)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

A curated list of open-source speech-to-text tools for voice typing and dictation across desktop, mobile, and CLI.

These tools let you speak and have text appear wherever you're typing. Some run speech-to-text entirely offline on your own hardware, others use cloud APIs, and many support both. All are open source.

---

## Contents

- [Just Tell Me What to Use](#just-tell-me-what-to-use)
- [Trending Voice Typing Tools](#trending-voice-typing-tools)
- [Hacker News Discussions](#hacker-news-discussions)
- [Directory](#directory)
- [Related Projects](#related-projects)
- [Scope](#scope)

## Just Tell Me What to Use

All these tools do the same core thing: transcribe your speech and paste it wherever your cursor is. The differences come down to platform, engine preference, and how much you want beyond basic dictation.

A few starting points:

- **Cross-platform default:** [Handy](https://github.com/cjpais/Handy). Biggest open-source project in this list, runs on Linux, macOS, and Windows.
- **On macOS, want a native feel:** [VoiceInk](https://github.com/Beingpax/VoiceInk) or [FluidVoice](https://github.com/altic-dev/FluidVoice).

## Trending Voice Typing Tools

<!-- trending:start -->

Based on stars gained in the last 30 days | Last updated: 2026-09-18

| Tool | Stars gained (30 days) | Total stars | Growth |
| --- | ---: | ---: | ---: |
| [OpenWhispr](https://github.com/OpenWhispr/openwhispr) | 2,800 | 8,321 | 50.7% |
| [Handy](https://github.com/cjpais/Handy) | 1,973 | 31,807 | 6.6% |
| [FluidVoice](https://github.com/altic-dev/FluidVoice) | 1,005 | 11,613 | 9.5% |
| [VoiceInk](https://github.com/Beingpax/VoiceInk) | 477 | 6,443 | 8.0% |
| [OpenLess](https://github.com/Open-Less/openless) | 416 | 3,567 | 13.2% |

<!-- trending:end -->

## Hacker News Discussions

| HN title | Points | Comments | Date posted |
| --- | ---: | ---: | --- |
| [Show HN: Whispering – Open-source, local-first dictation you can trust](https://news.ycombinator.com/item?id=44942731) | 591 | 152 | 2025-08-18 |
| [Show HN: Ghost Pepper – Local hold-to-talk speech-to-text for macOS](https://news.ycombinator.com/item?id=47666024) | 467 | 200 | 2026-04-06 |
| [Handy – Free open source speech-to-text app](https://news.ycombinator.com/item?id=46628397) | 247 | 110 | 2026-01-15 |
| [Transcribro: On-device Accurate Speech-to-text](https://news.ycombinator.com/item?id=40997850) | 165 | 60 | 2024-07-18 |
| [Show HN: Yap – OSS on-device voice dictation for macOS with no model to download](https://news.ycombinator.com/item?id=49073834) | 104 | 44 | 2026-07-27 |

## Directory

`Mode`: `Local` means on-device speech recognition. `Hybrid` means the tool supports both local and cloud or BYO-cloud setups. `Cloud` means speech recognition requires a remote service.

| Name | Platforms | Mode | Engine | Summary |
| --- | --- | --- | --- | --- |
| [Amical](https://github.com/amicalhq/amical)<br/><br/>![stars](https://img.shields.io/github/stars/amicalhq/amical?style=plastic&label=%E2%98%85) | macOS, Windows | Local | Whisper | Context-aware dictation that adapts formatting to the app you are using. |
| [BiBi Keyboard](https://github.com/BryceWG/BiBi-Keyboard)<br/><br/>![stars](https://img.shields.io/github/stars/BryceWG/BiBi-Keyboard?style=plastic&label=%E2%98%85) | Android | Hybrid | SenseVoice, FunASR Nano, Qwen3-ASR, Parakeet, BYOK cloud | Voice input keyboard with optional text cleanup and a floating recorder that inserts text into other apps. |
| [CapsWriter-Offline](https://github.com/HaujetZhao/CapsWriter-Offline)<br/><br/>![stars](https://img.shields.io/github/stars/HaujetZhao/CapsWriter-Offline?style=plastic&label=%E2%98%85) | Windows | Local | Paraformer, SenseVoice, Fun-ASR-Nano, Qwen3-ASR | Hold-to-dictate tool with fully offline Chinese and English recognition, phoneme-based hotword correction, LLM post-processing roles, and date-archived transcripts with audio. |
| [Chirp](https://github.com/Whamp/chirp)<br/><br/>![stars](https://img.shields.io/github/stars/Whamp/chirp?style=plastic&label=%E2%98%85) | Windows | Local | Parakeet TDT | Dictates into Windows apps, runs on CPU only, and is aimed at locked-down corporate environments. |
| [Clovy](https://github.com/open-software-network/os-clovy)<br/><br/>![stars](https://img.shields.io/github/stars/open-software-network/os-clovy?style=plastic&label=%E2%98%85) | macOS | Cloud | Parakeet TDT, GPT-4o Transcribe | Push-to-talk or hands-free dictation with text cleanup, writing styles, and automatic paste into the previous app. |
| [Dictate Keyboard](https://github.com/DevEmperor/DictateKeyboard)<br/><br/>![stars](https://img.shields.io/github/stars/DevEmperor/DictateKeyboard?style=plastic&label=%E2%98%85) | Android, Wear OS | Hybrid | Whisper, Parakeet, Canary, BYOK cloud | Android keyboard with offline and streaming dictation, a floating input button, and configurable text rewriting. |
| [Elograf](https://github.com/papoteur-mga/elograf)<br/><br/>![stars](https://img.shields.io/github/stars/papoteur-mga/elograf?style=plastic&label=%E2%98%85) | Linux | Local | Vosk (via nerd-dictation) | GUI tray frontend for nerd-dictation with model switching and timeout controls. |
| [Epicenter Whispering](https://github.com/EpicenterHQ/epicenter/tree/main/apps/whispering)<br/><br/>![stars](https://img.shields.io/github/stars/EpicenterHQ/epicenter?style=plastic&label=%E2%98%85) | Linux, macOS, Windows, Web | Hybrid | Whisper | Local-first dictation with a global shortcut and multiple Whisper providers; also available as a Chrome extension and web app. |
| [fcitx5-vinput](https://github.com/xifan2333/fcitx5-vinput)<br/><br/>![stars](https://img.shields.io/github/stars/xifan2333/fcitx5-vinput?style=plastic&label=%E2%98%85) | Linux | Hybrid | sherpa-onnx, BYOK cloud | Fcitx5 voice input with push-to-talk and toggle modes, hotwords, and optional text rewriting. |
| [FluidVoice](https://github.com/altic-dev/FluidVoice)<br/><br/>![stars](https://img.shields.io/github/stars/altic-dev/FluidVoice?style=plastic&label=%E2%98%85) | macOS | Hybrid | Parakeet, Apple Speech, Whisper | macOS dictation app that can type into any app and switch between local speech engines. |
| [FnKey](https://github.com/evoleinik/fnkey)<br/><br/>![stars](https://img.shields.io/github/stars/evoleinik/fnkey?style=plastic&label=%E2%98%85) | macOS | Hybrid | Deepgram Nova-3, Groq Whisper | Rust menu bar app that activates the microphone only while holding Fn, with real-time streaming and batch cloud backends. |
| [Freestyle](https://github.com/freestyle-voice/freestyle)<br/><br/>![stars](https://img.shields.io/github/stars/freestyle-voice/freestyle?style=plastic&label=%E2%98%85) | Linux, macOS, Windows | Hybrid | Whisper.cpp, Qwen3-ASR, SenseVoice, Parakeet, BYOK cloud | Hotkey dictation with automatic paste, custom vocabulary, and app-specific formatting. |
| [Ghost Pepper](https://github.com/matthartman/ghost-pepper)<br/><br/>![stars](https://img.shields.io/github/stars/matthartman/ghost-pepper?style=plastic&label=%E2%98%85) | macOS | Local | WhisperKit | Hold-to-talk menu bar dictation with local LLM cleanup of filler words; runs entirely on Apple Silicon. |
| [Glimpse](https://github.com/glimpse-hq/Glimpse)<br/><br/>![stars](https://img.shields.io/github/stars/glimpse-hq/Glimpse?style=plastic&label=%E2%98%85) | macOS, Windows | Hybrid | Whisper.cpp, Parakeet TDT | Dictation with a custom dictionary, text replacements, and a library for transcribing imported audio and video files. |
| [Handy](https://github.com/cjpais/Handy)<br/><br/>![stars](https://img.shields.io/github/stars/cjpais/Handy?style=plastic&label=%E2%98%85) | Linux, macOS, Windows | Local | Whisper.cpp, Parakeet TDT | Shortcut-driven offline dictation built with Tauri and supporting several ASR model families. |
| [HNS](https://github.com/primaprashant/hns)<br/><br/>![stars](https://img.shields.io/github/stars/primaprashant/hns?style=plastic&label=%E2%98%85) | Linux, macOS, Windows | Local | Faster Whisper | CLI tool that records from your mic, transcribes locally, and copies the result to the clipboard. |
| [hyprwhspr](https://github.com/goodroot/hyprwhspr)<br/><br/>![stars](https://img.shields.io/github/stars/goodroot/hyprwhspr?style=plastic&label=%E2%98%85) | Linux | Hybrid | Whisper.cpp, Parakeet, BYOK cloud | Push-to-talk Linux dictation with a visualizer plus Waybar and systemd integration. |
| [Koe](https://github.com/missuo/koe)<br/><br/>![stars](https://img.shields.io/github/stars/missuo/koe?style=plastic&label=%E2%98%85) | macOS | Hybrid | Apple Speech, Qwen3-ASR, Zipformer, BYOK cloud | Apple Silicon dictation with automatic paste, configurable text correction, and a plain-text dictionary. |
| [LiltKey](https://github.com/tangzk/liltkey)<br/><br/>![stars](https://img.shields.io/github/stars/tangzk/liltkey?style=plastic&label=%E2%98%85) | Linux | Local | sherpa-onnx (Streaming Zipformer, SenseVoice) | Fcitx5 hold-to-talk dictation with streaming preedit, local punctuation, and Chinese–English mixed input; Ubuntu 26.04 deb only. |
| [MacParakeet](https://github.com/moona3k/macparakeet)<br/><br/>![stars](https://img.shields.io/github/stars/moona3k/macparakeet?style=plastic&label=%E2%98%85) | macOS | Local | Parakeet, WhisperKit, Nemotron, Cohere Transcribe | Apple Silicon dictation with push-to-talk and hands-free modes, custom word replacements, and automatic paste. |
| [Muesli](https://github.com/Muesli-HQ/muesli)<br/><br/>![stars](https://img.shields.io/github/stars/Muesli-HQ/muesli?style=plastic&label=%E2%98%85) | macOS | Hybrid | Parakeet, WhisperKit, Qwen3-ASR, BYOK cloud | Hold-to-talk or hands-free dictation with a personal dictionary and optional transcript cleanup. |
| [Murmure](https://github.com/Kieirra/murmure)<br/><br/>![stars](https://img.shields.io/github/stars/Kieirra/murmure?style=plastic&label=%E2%98%85) | Linux, macOS, Windows | Local | Parakeet TDT | Offline dictation with a custom dictionary and optional local LLM processing. |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation)<br/><br/>![stars](https://img.shields.io/github/stars/ideasman42/nerd-dictation?style=plastic&label=%E2%98%85) | Linux | Local | Vosk | Hackable offline dictation that types into any window via simulated keystrokes. |
| [Offline Voice Input (Android)](https://github.com/notune/android_transcribe_app)<br/><br/>![stars](https://img.shields.io/github/stars/notune/android_transcribe_app?style=plastic&label=%E2%98%85) | Android | Local | Parakeet TDT | Offline Android voice input keyboard with live subtitles and a privacy-first focus. |
| [OpenLess](https://github.com/Open-Less/openless)<br/><br/>![stars](https://img.shields.io/github/stars/Open-Less/openless?style=plastic&label=%E2%98%85) | macOS, Windows | Hybrid | Qwen3-ASR, Whisper, BYOK cloud | Hotkey dictation with a custom dictionary and configurable transcript cleanup. |
| [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper)<br/><br/>![stars](https://img.shields.io/github/stars/Starmel/OpenSuperWhisper?style=plastic&label=%E2%98%85) | macOS | Local | Whisper, Parakeet | Native Swift menu bar dictation app optimized for Apple Silicon and global shortcuts. |
| [OpenTypeless](https://github.com/tover0314-w/opentypeless)<br/><br/>![stars](https://img.shields.io/github/stars/tover0314-w/opentypeless?style=plastic&label=%E2%98%85) | Linux, macOS, Windows | Hybrid | Whisper-compatible, Deepgram, AssemblyAI, Groq | Cross-platform voice input with AI polishing, selected-text rewriting, translation, and provider choice. |
| [OpenWhispr](https://github.com/OpenWhispr/openwhispr)<br/><br/>![stars](https://img.shields.io/github/stars/OpenWhispr/openwhispr?style=plastic&label=%E2%98%85) | Linux, macOS, Windows | Hybrid | Whisper.cpp, Parakeet, BYOK cloud | Cross-platform dictation with local models, optional cloud providers, and a custom dictionary. |
| [OSTT](https://github.com/kristoferlund/ostt)<br/><br/>![stars](https://img.shields.io/github/stars/kristoferlund/ostt?style=plastic&label=%E2%98%85) | Linux, macOS | Hybrid | Whisper.cpp, BYOK cloud | CLI dictation with a hotkey popup, automatic paste, and transcript processing through shell commands. |
| [Pindrop](https://github.com/watzon/pindrop)<br/><br/>![stars](https://img.shields.io/github/stars/watzon/pindrop?style=plastic&label=%E2%98%85) | macOS | Local | WhisperKit | Offline menu bar dictation app with optional AI-based transcript cleanup. |
| [Speak to AI](https://github.com/AshBuk/speak-to-ai)<br/><br/>![stars](https://img.shields.io/github/stars/AshBuk/speak-to-ai?style=plastic&label=%E2%98%85) | Linux | Local | Whisper.cpp | Minimal Linux dictation tool that inserts text into the active window and can also run from the CLI. |
| [SpeakoFlow](https://github.com/AbhishekBarali/SpeakoFlow)<br/><br/>![stars](https://img.shields.io/github/stars/AbhishekBarali/SpeakoFlow?style=plastic&label=%E2%98%85) | Linux, macOS, Windows | Local | Whisper.cpp, Parakeet | Offline dictation that can also turn a spoken request into finished text, with tone-based cleanup and an optional screen-aware assistant panel. |
| [SpeakType](https://github.com/karansinghgit/speaktype)<br/><br/>![stars](https://img.shields.io/github/stars/karansinghgit/speaktype?style=plastic&label=%E2%98%85) | macOS | Local | WhisperKit | Hold-to-talk offline dictation with a global shortcut and automatic paste into the active app. |
| [Talk-type](https://github.com/cyx2333hhh/talk-type)<br/><br/>![stars](https://img.shields.io/github/stars/cyx2333hhh/talk-type?style=plastic&label=%E2%98%85) | macOS | Hybrid | Apple Speech, Whisper.cpp | Chinese, English, and mixed-language dictation with live previews, optional text cleanup, and local Whisper fallback. |
| [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice)<br/><br/>![stars](https://img.shields.io/github/stars/kstonekuan/tambourine-voice?style=plastic&label=%E2%98%85) | macOS, Windows | Hybrid | Faster Whisper, BYOK cloud | Voice interface for any app with configurable STT and LLM providers. |
| [Transcribro](https://github.com/soupslurpr/Transcribro)<br/><br/>![stars](https://img.shields.io/github/stars/soupslurpr/Transcribro?style=plastic&label=%E2%98%85) | Android | Local | Whisper.cpp | Private and on-device speech recognition keyboard and service for Android. |
| [TranscriptionSuite](https://github.com/homelab-00/TranscriptionSuite)<br/><br/>![stars](https://img.shields.io/github/stars/homelab-00/TranscriptionSuite?style=plastic&label=%E2%98%85) | Linux, macOS, Windows | Local | Faster Whisper, Whisper.cpp, Parakeet | Dictation with global shortcuts and automatic paste, using a local or self-hosted transcription server. |
| [Typeflux](https://github.com/mylxsw/typeflux)<br/><br/>![stars](https://img.shields.io/github/stars/mylxsw/typeflux?style=plastic&label=%E2%98%85) | macOS | Hybrid | SenseVoice, Paraformer, WhisperKit, Qwen3-ASR, BYOK cloud | Hold Fn to dictate into the active app, with streaming previews, local history, and voice-driven text rewriting. |
| [TypeWhisper](https://github.com/TypeWhisper/typewhisper-mac)<br/><br/>![stars](https://img.shields.io/github/stars/TypeWhisper/typewhisper-mac?style=plastic&label=%E2%98%85) | macOS | Hybrid | Whisper (local and/or cloud) | Voice typing app with both local and cloud engine options. |
| [Vocalinux](https://github.com/jatinkrmalik/vocalinux)<br/><br/>![stars](https://img.shields.io/github/stars/jatinkrmalik/vocalinux?style=plastic&label=%E2%98%85) | Linux | Local | Whisper.cpp, Whisper, Vosk | Linux dictation with distro-specific setup guides and Vulkan acceleration notes. |
| [VoiceFlow](https://github.com/infiniV/VoiceFlow)<br/><br/>![stars](https://img.shields.io/github/stars/infiniV/VoiceFlow?style=plastic&label=%E2%98%85) | Linux, Windows | Local | Faster Whisper | Tray dictation with hold or toggle shortcuts, automatic paste, and searchable transcript history. |
| [VoiceInk](https://github.com/Beingpax/VoiceInk)<br/><br/>![stars](https://img.shields.io/github/stars/Beingpax/VoiceInk?style=plastic&label=%E2%98%85) | macOS | Hybrid | WhisperKit, BYOK | Native macOS dictation with per-app tuning, a custom dictionary, and optional commercial distribution. |
| [VoiceTypr](https://github.com/moinulmoin/voicetypr)<br/><br/>![stars](https://img.shields.io/github/stars/moinulmoin/voicetypr?style=plastic&label=%E2%98%85) | macOS, Windows | Local | Whisper-based | Voice-to-text dictation built with Tauri; the repository is open source, but binaries require a one-time license purchase. |
| [Voquill](https://github.com/josiahsrc/voquill)<br/><br/>![stars](https://img.shields.io/github/stars/josiahsrc/voquill?style=plastic&label=%E2%98%85) | Linux, macOS, Windows | Hybrid | Whisper.cpp, BYOK cloud | Cross-platform voice typing with a personal glossary and AI-assisted cleanup. |
| [VOXD](https://github.com/jakovius/voxd)<br/><br/>![stars](https://img.shields.io/github/stars/jakovius/voxd?style=plastic&label=%E2%98%85) | Linux | Local | Whisper.cpp | Linux dictation with GUI, tray, and CLI modes plus optional LLM post-processing. |
| [VoxType](https://github.com/peteonrails/voxtype)<br/><br/>![stars](https://img.shields.io/github/stars/peteonrails/voxtype?style=plastic&label=%E2%98%85) | Linux | Hybrid | Whisper.cpp, Parakeet, Moonshine, SenseVoice | Push-to-talk Linux dictation with seven engine choices, CJK support, and Wayland-optimized text insertion. |
| [Whisper IME](https://github.com/woheller69/whisperIME)<br/><br/>![stars](https://img.shields.io/github/stars/woheller69/whisperIME?style=plastic&label=%E2%98%85) | Android | Local | Whisper.cpp | Android keyboard and standalone app powered by Whisper, fully offline, and available on F-Droid. |
| [whisper_dictation](https://github.com/themanyone/whisper_dictation)<br/><br/>![stars](https://img.shields.io/github/stars/themanyone/whisper_dictation?style=plastic&label=%E2%98%85) | Linux | Local | Whisper.cpp | Feature-rich Linux voice keyboard with dictation, voice commands, and webcam integration. |
| [Yap](https://github.com/FrigadeHQ/yap)<br/><br/>![stars](https://img.shields.io/github/stars/FrigadeHQ/yap?style=plastic&label=%E2%98%85) | macOS | Local | Apple Speech | Native macOS 26 menu bar dictation using Apple's SpeechAnalyzer for streaming on-device transcription. |

## Related Projects

Speech recognition engines, models, and APIs that power the tools listed above.

- [Whisper](https://huggingface.co/collections/openai/whisper-release-6501bba2cf999715571c6b98) - OpenAI's ASR model weights; tiny through large, English-only and multilingual.
- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) - Pure C/C++ Whisper inference with zero dependencies; runs on Apple Silicon, CUDA, Vulkan, and WASM.
- [Faster Whisper](https://github.com/SYSTRAN/faster-whisper) - CTranslate2-based Whisper reimplementation; up to 4x faster with lower memory.
- [WhisperKit](https://github.com/argmaxinc/WhisperKit) - Swift package for on-device Whisper on Apple Silicon with streaming support.
- [Parakeet](https://huggingface.co/collections/nvidia/parakeet-702d39a47302ef820e49839d) - NVIDIA's high-accuracy English ASR models in CTC, RNN-T, and TDT architectures.
- [Vosk](https://github.com/alphacep/vosk-api) - Lightweight offline ASR with compact models, 20+ languages, and multi-language bindings.
- [Apple Speech](https://developer.apple.com/documentation/speech) - Apple's on-device speech recognition framework for iOS, macOS, and watchOS.
- [Awesome Whisper](https://github.com/sindresorhus/awesome-whisper) - Curated list of Whisper tools and resources.

## Scope

This list focuses on open-source apps, keyboards, and CLI tools for voice typing and dictation across desktop, mobile, and terminal workflows, with local or cloud speech recognition. Closed-source products, general transcription tools without dictation workflows, meeting bots, note takers, and standalone speech APIs are outside its scope.
