# Navahang privacy policy

Last updated: 2026-10-21

Navahang reads the page that the user explicitly asks it to read. By default, page text, selected text, language detection, diacritization, phonemization, summarization, translation and audio generation are processed locally in the extension and are not sent to a Piper server or an analytics service.

The user may explicitly choose an **OpenAI-compatible API**, select a preset or enter a custom Base URL, and paste their own API key. The endpoint settings and key are saved only in `chrome.storage.local`; the key is sent only to the Base URL displayed in settings as a bearer credential and can be cleared at any time. It is never sent to the Navahang developer or included in reading session payloads. The user separately controls whether the selected endpoint may receive text for important-content selection, summaries, translations, questions/explanations, and voice generation. Features whose API scope is disabled continue to use Built-in AI or local processing. When API voice generation is enabled, Navahang clearly identifies it as AI-generated and sends each spoken segment to the separately displayed speech Base URL to request a WAV or another selected compatible audio format. The selected service's own data controls and retention terms apply to these opt-in requests.

The extension stores only local preferences (including optional compatible-API endpoint settings and key), downloaded voice files and short-lived session state in Chrome storage. Session state can include the current page selection while an action is running and is removed by Chrome when the session ends. The extension does not sell, share or use page content for advertising, profiling or training.

No voice weight is bundled with or downloaded during extension installation. When the user first plays a voice, Chrome requests its weight from the public Navahang voice-assets GitHub Releases repository. A pinned official upstream URL may be used only if the release asset is unavailable. Those hosts may receive the normal network request metadata required to serve the file. Voice files are cached locally and can be removed by clearing the extension's data.

The extension requests access to ordinary `http` and `https` pages only so it can capture the text selected by the user, find important page text when no selection exists, and draw the optional word underline. It does not read restricted browser pages such as `chrome://` pages.

For privacy questions, open an issue in the public [voice-assets and support repository](https://github.com/Masih-Roughani/Navahang-voice-assets/issues). The extension's development source repository is private.
