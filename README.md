# A2 Conversation Studio

A single-file, 15-hour A2 English speaking and vocabulary course: ten 90-minute sessions built around real-life themes.

**Live page:** open `index.html` directly, or serve the folder:

```bash
python -m http.server 8765
# http://127.0.0.1:8765/index.html
```

## What is inside

- **10 sessions × 90 minutes** with a timed plan, task lab, fluency sprint, worksheet and homework.
- **310 target words** in themed groups, each with a definition and an example.
- **310 speaking prompts** organised by theme, with space to type answers.
- **35 grammar clinic cards** matched to the session themes.
- **10 reading assignments** of 250+ words, each with 10 comprehension questions and an answer key.
- Self-test mode, per-session completion tracking and A4 print/PDF output.

## Interactive layer

All answers, ticks, reading self-checks, sprint reflections and notes are saved in this browser using `localStorage` — nothing is sent to a server.

- Type in any answer field; it saves automatically.
- Tick plan steps, task prompts, homework and reading self-checks.
- Use the **Notes** switch in the top bar for a floating scratchpad. Notes persist, and can be downloaded as a `.txt` file.
- Each fluency sprint has a one-minute timer.
- Use **Print / Save PDF** for a clean A4 version. Answers and notes are left out of the printout; worksheet lines print as writing lines.

Clearing browser data for this page will remove saved answers and notes.

## Structure

Everything lives in `index.html`: styles, the `CURRICULUM` data, render functions and the interactive layer. No build step and no dependencies beyond the Google Fonts stylesheet (the page falls back to system fonts offline).
