# Xenolexia Foundation

> *Learn languages through the stories you love*

**Xenolexia** is a language learning app that helps you acquire new languages by reading. Instead of drilling vocabulary in isolation, you encounter new words in rich, familiar contexts—making acquisition natural and memorable.

Read books in your native language while learning Spanish, French, German, Japanese, or any of **28+ supported languages**. A portion of words (based on your proficiency level and density settings) appear in the target language. You infer meaning from context; hovering or tapping reveals the original word and lets you save it to your vocabulary. Build vocabulary and review with spaced repetition.

**Example (English → Spanish, beginner):**

> "She walked into the **casa** and set down her keys."  
> *Hover or tap "casa" → reveals "house"*

---

## Xenolexia Foundation

The **Xenolexia Foundation** is a non-profit organization that manages the Xenolexia apps and implementations across various platforms. The Foundation oversees development, ensures consistency across implementations, and maintains the shared vision of making language learning accessible through immersive reading.

---

## Implementations

Xenolexia is implemented in three separate codebases, each targeting different platforms and ecosystems:

| Implementation | Languages | Platforms |
|----------------|-----------|-----------|
| [**xenolexia-typescript**](https://github.com/Xenolexia-Foundation/xenolexia-typescript) | TypeScript | **Desktop** (Electron): Windows, macOS, Linux • **Mobile** (React Native): iOS, Android |
| ~~[**xenolexia-csharp**](https://github.com/Xenolexia-Foundation/xenolexia-csharp) | C# / .NET | **Desktop** (Avalonia): Windows, macOS, Linux~~ **abandoned** |
| ~~[**xenolexia-objc**](https://github.com/Xenolexia-Foundation/xenolexia-objc) | Objective-C | **macOS** (AppKit) • **iOS** (UIKit) • **Linux** (GNUStep)~~ **abandoned** |

### xenolexia-typescript

Monorepo with a shared TypeScript core (`ts-shared-core`), an Electron desktop app, and a React Native mobile app. Supports EPUB, TXT, MOBI; 28+ language pairs; spaced repetition (SM-2); vocabulary export (CSV, Anki, JSON).

### xenolexia-csharp

Cross-platform desktop app built with Avalonia UI and .NET. Single codebase for Linux, macOS, and Windows. Uses FOSS libraries only (VersOne.Epub, PdfPig, Fb2.Document). Supports EPUB, PDF, TXT, FB2; LibreTranslate; offline dictionary cache.

### xenolexia-objc

Native implementation for Apple platforms and Linux (GNUStep). Shared core logic with platform-specific UI. Targets macOS, iOS, and GNUStep-based Linux desktops.

---

## Core Features (Across Implementations)

- **Multi-format reading**: EPUB, PDF, TXT, FB2, MOBI (varies by implementation)
- **Proficiency-based word replacement**: Beginner, Intermediate, Advanced (CEFR)
- **28+ language pairs** via free translation APIs (LibreTranslate, MyMemory, Lingva)
- **Vocabulary management**: Save words, spaced repetition (SM-2), export to Anki/CSV/JSON
- **Customizable reader**: Fonts, themes (light/dark/sepia), margins, line spacing
- **Library**: Import local files, discover free ebooks (Project Gutenberg, Standard Ebooks, Open Library)

---

## License

AGPL-3.0 license.
