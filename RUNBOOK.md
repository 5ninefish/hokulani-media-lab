# Media Lab — Monday Run-of-Show (v2, ~3h50m)

Students open ONE URL on their iPads: **https://5ninefish.github.io/hokulani-media-lab/**

Stations unlock **in order**, and inside each station content comes **one pane
at a time** (Back / dots / Next) — research-backed segmenting: students see one
chunk, do its activity, and Next stays locked until that pane's game or quiz is
done (a hint under the dots says what's left). The CapCut build is an 11-step
wizard, one screenshot per pane. You control the room only at the three
⏸ CHECKPOINT moments.

## Before Monday (15 min of prep)

1. **Deploy the chat backend** (one-time): the hub's Brainstorm Bot needs the
   updated worker pushed to Cloudflare. Open Terminal and run:
   ```
   cd "/Users/dalen/Desktop/CDS Work/Hokulani Lessons/hokulani-ai-image-studio/worker" && npx wrangler login
   ```
   (a browser window opens — click Allow), then tell PMCL "deploy the worker"
   — or run `npx wrangler deploy` yourself in the same folder.
   Until this is done the hub still works: the chat shows a friendly offline
   notice and auto-skips that requirement.
2. **Workers Paid** — already confirmed active. Chat + images for a class day
   is roughly $1–4 total.
3. **Test on school Wi-Fi** — open the hub, send one Brainstorm Bot message,
   generate one Image Studio image, try one project-Gmail Canva login.
4. Queue the deepfake videos AND the two ethics videos ("What is an Ethical
   AI?" Mozilla / "What is AI Ethics?") on your MacBook.

## The day

| Clock | Station | You do |
|---|---|---|
| 0:00 | 🏁 Start (10m) | Project the URL. Students open it and read how the day works. |
| 0:10 | 🕵️ Spot the AI (20m) | **⏸ CHECKPOINT 1:** deepfake videos on the big screen. Then: Real-or-AI tap game (Maggie Smith), check quiz, table talk. |
| 0:30 | 🧠 AI Decoded (25m) | Self-paced: predictive-text game + **train-your-own-spam-filter** game (students label data, watch the AI learn — including learning their mistakes). |
| 0:55 | ⚖️ Ethics (20m) | Bias hiring-AI game (skewed training data → unfair rankings). **⏸ CHECKPOINT 2:** the two ethics videos + table discussion (AI in hiring/loans, explainability). |
| 1:15 | *Break (10m)* | |
| 1:25 | ✨ Prompt Lab (45m) | Brainstorm Bot chat (vague vs. specific prompts) → prompt-builder chips → AI Image Studio → Canva poster (project Gmail; crown = paid). Canva AI = early-finisher bonus. |
| 2:10 | 📡 Algorithm (25m) | Feed-curation game, sentiment machine (type a post, watch it get classified), generative-vs-analytical sort. |
| 2:35 | 🎬 Video Studio (65m) | Unsplash photos → script → CapCut → AI voiceover → captions → music → export. Screenshots for all 11 steps. Students self-confirm script + export to unlock Premiere. |
| 3:40 | 🏆 Premiere (20m) | **⏸ CHECKPOINT 3:** volunteer videos on the big screen. Toolbox-for-the-future. Final 5-question practice quiz (must complete). |
| ~4:00 | Post-test | Students switch to Google Classroom for the official post-test. |

## Post-test alignment (locked answers)

| Q | Taught at (definition → game → quiz) | Answer |
|---|---|---|
| 1. What is AI | 🧠 AI Decoded | d — machines that learn from data |
| 2. How AI generates | 🧠 predictive text + spam trainer | b — learns patterns from data |
| 3. "Curate" | 📡 feed game | b — organize content on user data |
| 4. Generative vs analytical | 📡 sentiment machine + sort game | a — creates new vs interprets existing |
| 5. "Prompt" | ✨ Brainstorm Bot + prompt builder | a — instruction guiding the AI |

Ethics is required course content (not on the post-test): bias game + videos +
its own check quiz, all gated like every other station.

## If something breaks

- **Brainstorm Bot down** → hub shows an offline notice, auto-skips that
  requirement, students brainstorm in Notes. Nothing blocks.
- **Image Studio fails on school network** → routes through the Cloudflare
  Worker (fixed 2026-07-10); if it still dies, students use Unsplash images
  for the Canva ad — the prompt-writing learning already happened.
- **A student's iPad loses progress** → progress is per-iPad (localStorage);
  worst case they replay a station's games (fast).
- **CapCut voice premium-gated** → any voice without the purple gem is free
  (called out in the hub, step 5).
- **A student is stuck behind the gate** → every requirement is listed as
  chips above the green button, so you can see at a glance what's missing.
