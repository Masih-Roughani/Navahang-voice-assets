# Browser extension privacy policy

Last updated: 2026-10-19

The extension reads the page that the user explicitly asks it to read. Page text, selected text, language detection, diacritization, phonemization, summarization, translation and audio generation are processed locally in the extension and are not sent to an extension server or analytics service.

The extension stores only local preferences, downloaded voice files and short-lived session state in Chrome storage. Session state can include the current page selection while an action is running and is removed by Chrome when the session ends. The extension does not sell, share or use page content for advertising, profiling or training.

No voice weight is bundled with or downloaded during extension installation. When the user first plays a voice, Chrome requests its weight from this repository's GitHub Releases. A pinned official upstream URL may be used only if the release asset is unavailable. Those hosts may receive the normal network request metadata required to serve the file. Voice files are cached locally and can be removed by clearing the extension's data.

The extension requests access to ordinary `http` and `https` pages only so it can capture the text selected by the user, inspect the page when no selection exists, and draw the optional word underline. It does not read restricted browser pages such as `chrome://` pages.

For privacy questions, open an issue in this repository. The extension's development source repository is private and is not used to deliver voice files.
