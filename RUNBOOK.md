# Media Lab — Monday Run-of-Show (3h50m)

Students open ONE URL on their iPads and self-pace. You control the room only at
the ⏸ CHECKPOINT moments. Everything else runs itself.

## Before Monday (15 min of prep)

1. **Cloudflare Workers Paid** — confirm the $5/mo plan is active on the
   `hokulani-image` Worker. The free tier caps at ~125 images/day; 100 students
   will blow past that in the first 10 minutes of Prompt Lab.
   (Metered cost for a class day: roughly $1–3.)
2. **Post-test link** — edit `index.html`, search for `postTestLink`, and paste
   your Google Form URL into the `href`.
3. **Test on school Wi-Fi** — open the hub + generate one image in AI Image
   Studio from the actual network.
4. Queue the deepfake videos on your MacBook for the two checkpoint moments.

## The day

| Clock | Station | You do |
|---|---|---|
| 0:00 | 🏁 Start (10m) | Project the hub URL. Students open it, read how the day works. |
| 0:10 | 🕵️ Spot the AI (20m) | **⏸ CHECKPOINT:** play deepfake videos on the big screen. Then students do the in-hub check + table discussion. |
| 0:30 | 🧠 AI Decoded (25m) | Self-paced: concept cards, predictive-text game, check questions. Circulate. |
| 0:55 | ✨ Prompt Lab (40m) | Self-paced: invent eco-product, craft prompts, generate ad in AI Image Studio, peer feedback swap. |
| 1:35 | *Break (10m)* | |
| 1:45 | 📡 Algorithm (30m) | Self-paced: "you are the algorithm" feed game, generative-vs-analytical sort, discussion. |
| 2:15 | 🎬 Video Studio (70m) | The big build: Unsplash photos → script → CapCut → AI voiceover → captions → music → export. Every step has a screenshot in the hub. Early finishers have bonus challenges. |
| 3:25 | 🏆 Premiere (25m) | **⏸ CHECKPOINT:** volunteers AirDrop/show videos on the big screen. Toolbox-for-the-future section. |
| 3:50 | Post-test | Students do the 5-question practice quiz in the hub, then the real Google Form. |

## Post-test alignment (locked answers)

| Q | Taught at | Answer |
|---|---|---|
| 1. What is AI | 🧠 AI Decoded | d — machines that learn from data |
| 2. How AI generates | 🧠 AI Decoded (predictive game) | b — learns patterns from data |
| 3. "Curate" | 📡 Algorithm (feed game) | b — organize content on user data |
| 4. Generative vs analytical | 📡 Algorithm (sort game) | a — creates new vs interprets existing |
| 5. "Prompt" | ✨ Prompt Lab | a — instruction guiding the AI |

Each concept is taught three ways: a definition card, a hands-on game, and a
practice question with instant feedback. The final station repeats all five as
a practice test.

## If something breaks

- **Image Studio fails on school network** → it now routes through the
  Cloudflare Worker (fixed 2026-07-10), but if it dies, students continue with
  Unsplash photos; the prompt-writing learning still happens in Notes.
- **A student's hub loses progress** → progress is per-iPad (localStorage);
  they can just tap their station and continue. Nothing is stored on a server.
- **CapCut voice is premium-gated** → any voice without the purple gem is free
  (called out in the hub, step 5).
