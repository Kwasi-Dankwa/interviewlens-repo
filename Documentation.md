# ITERATION I -  IMPORT FEATURE/FURTHER UI UPDATES
This first iteration was about improving what already works, I added a section that allows the user to add pdf, doc and txt files.

# ITERATION II - Better Input Handling/ More Useful Output/ FURTHER UI UPDATES
* Dark mode — toggle in the header, preference saved to localStorage so it persists across visits.
* Multi-file upload + synthesis — drop in 2–5 transcripts (PDF, DOCX, TXT mixed). Results come back in three tabs: Synthesis (cross-interview themes, shared pain points, top opportunities), Compare (side-by-side per-participant view + where they diverged), and individual breakdowns for each file.
* Confidence indicators — every theme now shows a 5-dot signal strength bar (low → strong), based on how dominant the pattern was across the transcript.
* Share Link — serializes the full analysis result into a base64 URL hash. Anyone opening that link sees the analysis instantly, no API key needed.
* Copy JSON — copies the raw structured output to clipboard, useful for pasting into Notion, Airtable, or feeding into another tool.
* Export PDF — triggers the browser's print dialog with a print stylesheet that hides the left panel and UI chrome, leaving just the analysis cards.
* History panel — every analysis is saved to localStorage. Click History in the header to browse, reload, or clear past sessions.
