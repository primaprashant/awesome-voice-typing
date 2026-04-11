# Awesome Voice Typing

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](CONTRIBUTING.md)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

A curated list of open-source speech-to-text tools for voice typing and dictation across desktop, mobile, and CLI.

These tools let you speak and have text appear wherever you're typing. Some run speech-to-text entirely offline on your own hardware, others use cloud APIs, and many support both. All are open source.

---

## Contents

- [Scope](#scope)
- [Platform Snapshot](#platform-snapshot)
- [Directory](#directory)
- [Related Projects](#related-projects)
- [Inclusion Notes](#inclusion-notes)
- [Contributing](#contributing)
- [License](#license)

## Scope

This list focuses on tools that let you speak and get text into the place where you are actively working.

- Open-source apps, keyboards, menu bar utilities, and CLI tools for dictation or voice typing
- Desktop, mobile, and terminal-first workflows
- Local-only and hybrid tools, as long as the project itself is open source

This list does not try to cover:

- Closed-source products
- General transcription tools that do not support typing or dictation workflows
- Meeting bots, note takers, or speech APIs without a usable typing interface

<details>
<summary>Browse by platform</summary>

- Linux: Buzz, Elograf, Epicenter Whispering, Handy, HNS, hyprwhspr, nerd-dictation, OpenWhispr, Speak to AI, Vibe, Vocalinux, Voquill, VOXD, VoxType, whisper_dictation, whisper-writer
- macOS: Amical, Buzz, Epicenter Whispering, FluidVoice, FnKey, Handy, HNS, OpenSuperWhisper, OpenWhispr, Pindrop, Tambourine Voice, TypeWhisper, Vibe, VoiceInk, VoiceTypr, Voquill, whisper-writer
- Windows: Amical, Buzz, Chirp, Epicenter Whispering, Handy, HNS, OmniDictate, OpenWhispr, Tambourine Voice, Vibe, VoiceTypr, Voquill, whisper-writer
- Android: Offline Voice Input, Transcribro, Whisper IME
- iOS: WhisperBoard

</details>

Most tools on this list support offline speech recognition. See `Mode` and `Engine` in the directory below for the details.

## Directory

`Mode`: `Local` means on-device speech recognition. `Hybrid` means the tool supports both local and cloud or BYO-cloud setups.

| Name | Platforms | Mode | Engine | Summary |
| --- | --- | --- | --- | --- |
| [Amical](https://github.com/amicalhq/amical) ![](https://img.shields.io/github/stars/amicalhq/amical?style=flat-square&label=%E2%98%85&color=777) | macOS, Windows | Local | Whisper | Context-aware dictation that adapts formatting to the app you are using. |
| [Buzz](https://github.com/chidiwilliams/buzz) ![](https://img.shields.io/github/stars/chidiwilliams/buzz?style=flat-square&label=%E2%98%85&color=777) | Linux, macOS, Windows | Local | Whisper, Whisper.cpp, Faster Whisper | Desktop app for microphone or file transcription; text stays in its own UI rather than typing into other apps. |
| [Chirp](https://github.com/Whamp/chirp) ![](https://img.shields.io/github/stars/Whamp/chirp?style=flat-square&label=%E2%98%85&color=777) | Windows | Local | Parakeet TDT | Dictates into Windows apps, runs on CPU only, and is aimed at locked-down corporate environments. |
| [Elograf](https://github.com/papoteur-mga/elograf) ![](https://img.shields.io/github/stars/papoteur-mga/elograf?style=flat-square&label=%E2%98%85&color=777) | Linux | Local | Vosk (via nerd-dictation) | GUI tray frontend for nerd-dictation with model switching and timeout controls. |
| [Epicenter Whispering](https://github.com/EpicenterHQ/epicenter/tree/main/apps/whispering) ![](https://img.shields.io/github/stars/EpicenterHQ/epicenter?style=flat-square&label=%E2%98%85&color=777) | Linux, macOS, Windows, Web | Hybrid | Whisper | Local-first dictation with a global shortcut and multiple Whisper providers; also available as a Chrome extension and web app. |
| [FluidVoice](https://github.com/altic-dev/FluidVoice) ![](https://img.shields.io/github/stars/altic-dev/FluidVoice?style=flat-square&label=%E2%98%85&color=777) | macOS | Hybrid | Parakeet, Apple Speech, Whisper | macOS dictation app that can type into any app and switch between local speech engines. |
| [FnKey](https://github.com/evoleinik/fnkey) ![](https://img.shields.io/github/stars/evoleinik/fnkey?style=flat-square&label=%E2%98%85&color=777) | macOS | Hybrid | Deepgram Nova-3, Groq Whisper | Rust menu bar app that activates the microphone only while holding Fn, with real-time streaming and batch cloud backends. |
| [Handy](https://github.com/cjpais/Handy) ![](https://img.shields.io/github/stars/cjpais/Handy?style=flat-square&label=%E2%98%85&color=777) | Linux, macOS, Windows | Local | Whisper.cpp, Parakeet TDT | Shortcut-driven offline dictation built with Tauri and supporting several ASR model families. |
| [HNS](https://github.com/primaprashant/hns) ![](https://img.shields.io/github/stars/primaprashant/hns?style=flat-square&label=%E2%98%85&color=777) | Linux, macOS, Windows | Local | Faster Whisper | CLI tool that records from your mic, transcribes locally, and copies the result to the clipboard. |
| [hyprwhspr](https://github.com/goodroot/hyprwhspr) ![](https://img.shields.io/github/stars/goodroot/hyprwhspr?style=flat-square&label=%E2%98%85&color=777) | Linux | Hybrid | Whisper.cpp, Parakeet, BYOK cloud | Push-to-talk Linux dictation with a visualizer plus Waybar and systemd integration. |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) ![](https://img.shields.io/github/stars/ideasman42/nerd-dictation?style=flat-square&label=%E2%98%85&color=777) | Linux | Local | Vosk | Hackable offline dictation that types into any window via simulated keystrokes. |
| [Offline Voice Input (Android)](https://github.com/notune/android_transcribe_app) ![](https://img.shields.io/github/stars/notune/android_transcribe_app?style=flat-square&label=%E2%98%85&color=777) | Android | Local | Parakeet TDT | Offline Android voice input keyboard with live subtitles and a privacy-first focus. |
| [OmniDictate](https://github.com/gurjar1/OmniDictate) ![](https://img.shields.io/github/stars/gurjar1/OmniDictate?style=flat-square&label=%E2%98%85&color=777) | Windows | Local | Whisper | Desktop dictation tool aimed at type-anywhere workflows. |
| [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) ![](https://img.shields.io/github/stars/Starmel/OpenSuperWhisper?style=flat-square&label=%E2%98%85&color=777) | macOS | Local | Whisper, Parakeet | Native Swift menu bar dictation app optimized for Apple Silicon and global shortcuts. |
| [OpenWhispr](https://github.com/OpenWhispr/openwhispr) ![](https://img.shields.io/github/stars/OpenWhispr/openwhispr?style=flat-square&label=%E2%98%85&color=777) | Linux, macOS, Windows | Hybrid | Whisper.cpp, Parakeet, BYOK cloud | Cross-platform dictation with local models, optional cloud providers, and a custom dictionary. |
| [Pindrop](https://github.com/watzon/pindrop) ![](https://img.shields.io/github/stars/watzon/pindrop?style=flat-square&label=%E2%98%85&color=777) | macOS | Local | WhisperKit | Offline menu bar dictation app with optional AI-based transcript cleanup. |
| [Speak to AI](https://github.com/AshBuk/speak-to-ai) ![](https://img.shields.io/github/stars/AshBuk/speak-to-ai?style=flat-square&label=%E2%98%85&color=777) | Linux | Local | Whisper.cpp | Minimal Linux dictation tool that inserts text into the active window and can also run from the CLI. |
| [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) ![](https://img.shields.io/github/stars/kstonekuan/tambourine-voice?style=flat-square&label=%E2%98%85&color=777) | macOS, Windows | Hybrid | Faster Whisper, BYOK cloud | Voice interface for any app with configurable STT and LLM providers. |
| [Transcribro](https://github.com/soupslurpr/Transcribro) ![](https://img.shields.io/github/stars/soupslurpr/Transcribro?style=flat-square&label=%E2%98%85&color=777) | Android | Local | Whisper.cpp | Private and on-device speech recognition keyboard and service for Android. |
| [TypeWhisper](https://github.com/TypeWhisper/typewhisper-mac) ![](https://img.shields.io/github/stars/TypeWhisper/typewhisper-mac?style=flat-square&label=%E2%98%85&color=777) | macOS | Hybrid | Whisper (local and/or cloud) | Voice typing app with both local and cloud engine options. |
| [Vibe](https://github.com/thewh1teagle/vibe) ![](https://img.shields.io/github/stars/thewh1teagle/vibe?style=flat-square&label=%E2%98%85&color=777) | Linux, macOS, Windows | Local | Whisper.cpp | Desktop app to transcribe audio and video offline using OpenAI Whisper. |
| [Vocalinux](https://github.com/jatinkrmalik/vocalinux) ![](https://img.shields.io/github/stars/jatinkrmalik/vocalinux?style=flat-square&label=%E2%98%85&color=777) | Linux | Local | Whisper.cpp, Whisper, Vosk | Linux dictation with distro-specific setup guides and Vulkan acceleration notes. |
| [VoiceInk](https://github.com/Beingpax/VoiceInk) ![](https://img.shields.io/github/stars/Beingpax/VoiceInk?style=flat-square&label=%E2%98%85&color=777) | macOS | Hybrid | WhisperKit, BYOK | Native macOS dictation with per-app tuning, a custom dictionary, and optional commercial distribution. |
| [VoiceTypr](https://github.com/moinulmoin/voicetypr) ![](https://img.shields.io/github/stars/moinulmoin/voicetypr?style=flat-square&label=%E2%98%85&color=777) | macOS, Windows | Local | Whisper-based | Voice-to-text dictation built with Tauri; the repository is open source, but binaries require a one-time license purchase. |
| [Voquill](https://github.com/josiahsrc/voquill) ![](https://img.shields.io/github/stars/josiahsrc/voquill?style=flat-square&label=%E2%98%85&color=777) | Linux, macOS, Windows | Hybrid | Whisper.cpp, BYOK cloud | Cross-platform voice typing with a personal glossary and AI-assisted cleanup. |
| [VOXD](https://github.com/jakovius/voxd) ![](https://img.shields.io/github/stars/jakovius/voxd?style=flat-square&label=%E2%98%85&color=777) | Linux | Local | Whisper.cpp | Linux dictation with GUI, tray, and CLI modes plus optional LLM post-processing. |
| [VoxType](https://github.com/peteonrails/voxtype) ![](https://img.shields.io/github/stars/peteonrails/voxtype?style=flat-square&label=%E2%98%85&color=777) | Linux | Hybrid | Whisper.cpp, Parakeet, Moonshine, SenseVoice | Push-to-talk Linux dictation with seven engine choices, CJK support, and Wayland-optimized text insertion. |
| [WhisperBoard](https://github.com/Saik0s/Whisperboard) ![](https://img.shields.io/github/stars/Saik0s/Whisperboard?style=flat-square&label=%E2%98%85&color=777) | iOS | Local | Whisper.cpp | iOS app for recording speech and producing text with downloadable Whisper models. |
| [Whisper IME](https://github.com/woheller69/whisperIME) ![](https://img.shields.io/github/stars/woheller69/whisperIME?style=flat-square&label=%E2%98%85&color=777) | Android | Local | Whisper.cpp | Android keyboard and standalone app powered by Whisper, fully offline, and available on F-Droid. |
| [whisper-writer](https://github.com/savbell/whisper-writer) ![](https://img.shields.io/github/stars/savbell/whisper-writer?style=flat-square&label=%E2%98%85&color=777) | Linux, macOS, Windows | Hybrid | Faster Whisper, OpenAI API | Hotkey-driven dictation that auto-types into the active window with several recording modes. |
| [whisper_dictation](https://github.com/themanyone/whisper_dictation) ![](https://img.shields.io/github/stars/themanyone/whisper_dictation?style=flat-square&label=%E2%98%85&color=777) | Linux | Local | Whisper.cpp | Feature-rich Linux voice keyboard with dictation, voice commands, and webcam integration. |

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

## Inclusion Notes

- Entries are linked to their source repository rather than landing pages or app-store listings.
- Some projects on this list also offer paid binaries or hosted features. They still belong here if the underlying repository is open source.
- Submissions are held to a minimum maturity bar. See [CONTRIBUTING.md](CONTRIBUTING.md) before opening a PR.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding, updating, or removing entries.

## License

[MIT](LICENSE)
