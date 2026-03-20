# Interview Lens

**AI-powered user interview analyzer built with Claude.**  
Turn raw transcripts and messy notes into structured UX insights — themes, pain points, key quotes, and product opportunities — in seconds.

🔗 [Live Demo](https://yourusername.github.io/interviewlens) &nbsp;·&nbsp; [Report a Bug](https://github.com/yourusername/interviewlens/issues)

---

## What It Does

User interviews generate a lot of raw, unstructured information. Synthesizing that information into something actionable — themes, opportunities, quotes worth sharing — typically takes hours of manual work.

Interview Lens automates that synthesis. Paste a transcript or notes, add optional context about your product and research goals, and Claude returns a structured analysis you can act on immediately.

### Analysis Output

| Section | Description |
|---|---|
| **Summary** | 2–3 sentence synthesis of the interview |
| **Key Themes** | Recurring patterns with supporting evidence |
| **Pain Points** | Specific struggles, rated by severity (high / medium / low) |
| **Key Quotes** | Notable participant quotes tagged by type (insight, blocker, desire, etc.) |
| **Opportunities** | Product or experience improvements grounded in the interview |
| **Follow-up Questions** | Suggested questions to explore in the next session |
| **Sentiment Score** | Visual indicator of overall participant sentiment |

---

## Who It's For

- **Product managers** who conduct discovery interviews and need to synthesize findings quickly
- **UX researchers** looking to speed up analysis without losing rigor
- **Designers** who run usability tests and want structured takeaways
- **Founders** doing early customer discovery
- **Students and bootcamp grads** building a UX or PM portfolio

---

## How to Use It

### 1. Get an Anthropic API Key
Create a free account at [console.anthropic.com](https://console.anthropic.com), navigate to **API Keys**, and generate a new key. New accounts receive free credits to get started.

> **Privacy note:** Your API key is used only within your browser session. It is never stored, logged, or transmitted anywhere other than directly to Anthropic's API.

### 2. Paste Your Transcript
Copy and paste a raw interview transcript, notes, or rough bullet points into the text area. The analyzer works with formal transcripts, informal notes, and everything in between.

### 3. Add Context (Optional)
Providing context helps Claude tailor the analysis. Fields include:
- **Product / Domain** — e.g. *habit-tracking app*
- **Research Goal** — e.g. *understand drop-off at onboarding*
- **Participant Role** — e.g. *first-time user*
- **Session Type** — e.g. *usability test*, *discovery interview*

### 4. Analyze
Hit **Analyze Interview** and review the structured output on the right panel. The analysis is generated in real time using Claude Sonnet.

---

## Running Locally

This is a zero-dependency, single-file application. No build step, no package manager.

```bash
git clone https://github.com/yourusername/interviewlens.git
cd interviewlens
open index.html
```

Or serve it locally with any static file server:

```bash
npx serve .
# or
python -m http.server 8000
```

---

## Deploying

The app is a single `index.html` file and deploys to any static hosting provider.

**GitHub Pages**
1. Push the repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your app will be live at `https://yourusername.github.io/interviewlens`

**Other options:** Vercel, Netlify, Cloudflare Pages — drag and drop `index.html` and you're done.

---

## Tech Stack

- **Vanilla HTML/CSS/JS** — no frameworks, no dependencies
- **[Claude claude-sonnet-4-20250514](https://www.anthropic.com/claude)** via the Anthropic Messages API
- **Google Fonts** — DM Serif Display, DM Sans, DM Mono

---

## Potential Future Improvements

These are directions worth exploring as the project evolves:

**Multi-interview synthesis**  
Upload several transcripts at once and surface patterns across participants — the real power of qual research is in cross-interview themes, not single sessions.

**Export to PDF / Notion / Confluence**  
Let researchers push the structured output directly into their documentation tools rather than copying manually.

**Tagging and filtering**  
Allow users to tag participants by persona, cohort, or product area and filter insights accordingly.

**Backend with authentication**  
Move the API key server-side so end users don't need their own Anthropic account. Pair with a simple login to enable saved sessions and history.

**Highlight detection**  
Automatically flag the most quotable moments in a transcript before full analysis — useful for long sessions.

**Custom analysis frameworks**  
Let teams define their own synthesis templates (e.g. Jobs to Be Done, JTBD, Opportunity Solution Trees) rather than using a fixed output structure.

**Comparison view**  
Side-by-side analysis of two interviews to identify where participant experiences converge or diverge.

---

## Contributing

Pull requests are welcome. For significant changes, please open an issue first to discuss what you'd like to change.

---

## License

[MIT](LICENSE)

---

*Built as a portfolio project to demonstrate AI-native product thinking and Claude API integration.*

