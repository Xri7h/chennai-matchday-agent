# Chennai Matchday — CSK ticket-sales agent

[Download the complete submission ZIP](Chennai-Matchday-Submission-2026-11-22.zip) · [Watch the Loom demo](https://www.loom.com/share/3c6af046dd7d43e4b586fb49e6a28f17)

The ZIP contains all **67 project files**, with their original folder structure: runnable Node.js server and web UI, synthetic catalog and 60-lead seed file, a scored outreach plan for 20 repeat fans, evaluation inputs and results, latency reports and raw measurements, tests, bundled model assets and license notices. Local credentials, phone numbers, runtime stores, preference backups and browser artifacts are excluded. It passed a scan against private local configuration values and common credential patterns, and every archived file was verified against its SHA-256 manifest.

## Run

1. Download and extract the ZIP into an empty folder.
2. Install Node.js 22 or newer. No package installation is required.
3. In the extracted folder, run `node server.mjs`.
4. Open `http://127.0.0.1:4173`.

Read `README.md` and `SUBMISSION.md` inside the extracted project for configuration, deliverable links, model details and limitations. Optional keys go in a local `.env` created from the empty `.env.example`. Without hosted keys, the catalog and local semantic fallback remain usable. Real telephony requires the reviewer's own account and verified phone number; browser speech is also supported.

## Evidence

- D1: text conversation and outreach logic; browser speech and a separately configured Exotel phone demo.
- D2: all 20 repeat fans have score components, contact/skip, channel, timing, first message and reasons in `reports/outreach.csv` and `reports/outreach.md`.
- D3: 38 development turns plus 9 historical regression turns; a 76-turn local text benchmark, optimization measurements, provider comparison, failure analysis and raw JSON. Submission checks: 56/56 tests passed.
- D4: the supplied Loom recording is 5:31, exceeding the requested five-minute maximum by 31 seconds. It should be shortened for strict adherence.

The millisecond benchmark measures local HTTP text response time, excluding microphone recognition, speech synthesis, browser painting and carrier delay. A 40-turn live-phone latency study, carrier SMS delivery, live inventory/checkout and a staffed handoff remain unfinished or unverified. All fan data, fixtures and prices are synthetic assignment assumptions, not an official CSK service.

AI-tool assistance, runtime model roles, model/font/photo licenses and privacy boundaries are documented in the archived README and submission notes.
