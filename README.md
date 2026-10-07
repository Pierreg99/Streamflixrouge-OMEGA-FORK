<div align="center">

# Streamflixrouge-OMEGA-FORK

<p><strong>Streamflix (Reborn): Android-Streaming-App in Kotlin, Community-Fortführung.</strong></p>
<p>
<img alt="Kotlin: 99%" src="https://img.shields.io/badge/Kotlin-99%25-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white">
<img alt="Lizenz: Apache-2.0" src="https://img.shields.io/badge/Lizenz-Apache--2.0-2E7D32?style=for-the-badge">
<img alt="Sichtbarkeit: Öffentlich" src="https://img.shields.io/badge/Sichtbarkeit-%C3%96ffentlich-0B7285?style=for-the-badge">
</p>
<p>
<a href="https://github.com/Pierreg99/Streamflixrouge-OMEGA-FORK/actions/workflows/release.yml"><img alt="release.yml" src="https://github.com/Pierreg99/Streamflixrouge-OMEGA-FORK/actions/workflows/release.yml/badge.svg"></a>
</p>
<p><a href="#schnellstart">Schnellstart</a> · <a href="#projektstruktur">Projektstruktur</a> · <a href="#english-summary">English</a></p>
</div>

---

## Inhaltsverzeichnis

- [Überblick](#überblick)
- [Features](#features)
- [Schnellstart](#schnellstart)
- [Architektur](#architektur)
- [Projektstruktur](#projektstruktur)
- [Dokumentation](#dokumentation)
- [Projektdetails](#projektdetails)
- [English summary](#english-summary)
- [Lizenzhinweis](#lizenzhinweis)

## Überblick

Streamflix (Reborn): Android-Streaming-App in Kotlin, Community-Fortführung.

| Merkmal | Wert |
| --- | --- |
| Sprachen | Kotlin (99%) |
| Dateien im Repository | 673 |
| CI-Workflows | 1 |
| Lizenz | [LICENSE](LICENSE) |

## Features

- Automatisierung über GitHub Actions: `release.yml`
- 3 Testdateien im Repository
- Android-Build mit Gradle

## Schnellstart

```bash
git clone https://github.com/Pierreg99/Streamflixrouge-OMEGA-FORK.git
cd Streamflixrouge-OMEGA-FORK
```

**Android**

```bash
./gradlew assembleDebug
```

## Architektur

Übersicht der wichtigsten Verzeichnisse nach Anzahl der enthaltenen Dateien.

```mermaid
flowchart LR
    R(["Streamflixrouge-OMEGA-FORK"])
    R --> D0["app/<br/>622 Dateien"]
    R --> D1["navigation/<br/>18 Dateien"]
    R --> D2["retrofit-jsoup-converter/<br/>9 Dateien"]
    R --> D3["supabase/<br/>3 Dateien"]
    R --> D4["gradle/<br/>2 Dateien"]
    R --> D5["moviblast-plugin/<br/>2 Dateien"]
    CI[["GitHub Actions<br/>1 Workflows"]] -.-> R
```

## Projektstruktur

```text
Streamflixrouge-OMEGA-FORK/
├── .github/  (5 Dateien)
│   ├── docs/
│   ├── ISSUE_TEMPLATE/
│   └── workflows/
├── app/  (622 Dateien)
│   ├── src/
│   ├── .gitignore
│   ├── build.gradle
│   └── proguard-rules.pro
├── gradle/  (2 Dateien)
│   └── wrapper/
├── moviblast-plugin/  (2 Dateien)
│   ├── plugin.js
│   └── test_provider.py
├── navigation/  (18 Dateien)
│   ├── src/
│   ├── .gitignore
│   ├── build.gradle
│   ├── consumer-rules.pro
│   └── proguard-rules.pro
├── retrofit-jsoup-converter/  (9 Dateien)
│   ├── src/
│   ├── .gitignore
│   ├── build.gradle
│   ├── consumer-rules.pro
│   └── proguard-rules.pro
├── supabase/  (3 Dateien)
│   ├── migrations/
│   └── README.md
├── .gitignore
├── build.gradle
├── gradle.properties
├── gradlew
├── gradlew.bat
├── LICENSE
├── lint.xml
├── README.md
├── settings.gradle
├── streamflix-main.zip
├── supabase_installation.md
└── SUPABASE_PROFILE_MERGE_GUIDE.md
```

## Dokumentation

- [supabase_installation.md](supabase_installation.md)
- [SUPABASE_PROFILE_MERGE_GUIDE.md](SUPABASE_PROFILE_MERGE_GUIDE.md)

## Projektdetails

Der folgende Abschnitt übernimmt die bisherige Projektdokumentation.

<h1 align="center">Streamflix Reborn</h1>

<p align="center">
  <img src="./app/src/main/res/mipmap-xxxhdpi/ic_launcher.png" height="100px" />
  <br />
  <strong> Reborn Version</strong> - Community continuation of the original Streamflix project
  <br />
  An open-source Android TV and mobile app for educational streaming interface, made with Android Studio, in Kotlin
  <br />
  <a href="https://github.com/streamflix-reborn2/streamflix/releases/latest">
    <strong>Download app »</strong>
  </a>
  <br />
  <br />
  <a href="https://github.com/streamflix-reborn2/streamflix/issues">Report Bug</a>
  ·
  <a href="https://github.com/streamflix-reborn2/streamflix/issues">Request Feature</a>
</p>

<details>
  <summary>Table of Contents</summary>

- [About the project](#about-the-project)
  - [What is Streamflix Reborn?](#-what-is-streamflix-reborn2)
  - [Features](#features)
  - [Built with](#built-with)
- [Getting started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
- [Development](#development)
- [Contributing](#contributing)
- [Legal Disclaimer](#legal-disclaimer)
- [Credits & Authors](#credits--authors)
- [License](#license)
</details>

## About the project

<p align="center">
  <img src="./.github/docs/screenshot.png" alt="Streamflix Preview">
</p>

**Streamflix Reborn** is an independent continuation of the original Streamflix project created by [Lory-Stan TANASI](https://github.com/stantanasi). This reborn version maintains the same educational purpose and functionality while ensuring continued development and support.

### What is Streamflix Reborn?

- **Independent Continuation**: This is an independent continuation of the original Streamflix project
- **Same Vision**: Maintains the original educational and open-source philosophy
- **Enhanced Support**: Continued development and bug fixes by an independent developer
- **Respectful Fork**: Built with full respect for the original creator's work

Streamflix Reborn is an open-source Android TV and mobile app that provides a user interface for accessing publicly available streaming content from various third-party providers.

This app is designed for educational purposes and personal use only. Users are responsible for ensuring they have proper authorization to access any content they view through this application.

The interface aggregates content from multiple sources and provides a convenient way to browse available streaming options.

### Features

- Open-source and ad-free interface
- Aggregates content from multiple third-party providers
- No account required for the app interface
- Educational and personal use only
- Optimized UI & UX
- Multiple providers
- Resume from last playback position
- In-app update

### Built with

- [Android Studio](https://developer.android.com/studio)
- [Kotlin](https://kotlinlang.org)
- [Retrofit](https://square.github.io/retrofit)
- [ExoPlayer](https://exoplayer.dev)
- Leanback
- Coroutines
- MVVM Architecture
- Android Architecture Components

## Getting started

### Prerequisites

Install [Android Studio](https://developer.android.com/studio)

### Setup

1. Clone the project to your local machine

```bash
git clone https://github.com/streamflix-reborn2/streamflix.git
```

2. Open the project in Android Studio

## Development

1. Select the device that you want to run the app

2. Click **Run**

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'feat: add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a pull request

## Legal Disclaimer

**IMPORTANT: This application is for educational and personal use only.**

- Streamflix does not host, store, or distribute any copyrighted content
- All content is sourced from third-party providers and websites
- Users are solely responsible for ensuring they have legal rights to access any content
- The developers do not endorse or encourage copyright infringement
- Users must comply with all applicable laws in their jurisdiction
- Any legal issues should be directed to the actual content providers
- This app functions as a search engine aggregator only
- No copyrighted material is stored on our servers

## Legal Notice

This application is provided "as is" for educational purposes. The developers:
- Do not claim ownership of any content
- Do not profit from copyrighted material
- Do not control third-party content providers
- Encourage users to support content creators through legal means
- Recommend using official streaming services when available

## Credits & Authors

### Original Creator
- **[Lory-Stan TANASI](https://github.com/stantanasi)** - Original Streamflix project creator

### Reborn Development
- **Independent Developer** - Streamflix Reborn maintainer
- **Special thanks** to the original creator for the excellent foundation

## License

This project is licensed under the `Apache-2.0` License - see the [LICENSE](LICENSE) file for details

### Original Project
<p align="center">
  <br />
  © 2022 Lory-Stan TANASI. All rights reserved
</p>

### Reborn Project
<p align="center">
  <br />
  © 2025 Streamflix Reborn. Built with respect for the original work.
</p>

## English summary

Streamflix (Reborn): Kotlin Android streaming app, community continuation.

Clone the repository and follow the commands in [Schnellstart](#schnellstart); the [project layout](#projektstruktur) shows where the code lives. Further documents are listed under [Dokumentation](#dokumentation).

## Lizenzhinweis

Siehe [LICENSE](LICENSE).
