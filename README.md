# robotis-convivium-demo

Static hosting for the **Phase 1 end-to-end demo** of the Robot Video → LeRobot
pipeline. The page (`index.html`) is a self-contained, dependency-free demo —
no build step, no external assets, works offline. Section titles and captions are
bilingual (English / Korean).

It opens with an **animated pipeline belt**: an episode card rides the nine pipeline
stages left to right, and at **Validation** a trainability level (L0–L4) is *computed*
and the **Router** sends it where that level allows. The belt cycles through four
sources — `collected.public_web` (permissive and license-blocked), `simulated`, and
`real` — so you watch the same pipe resolve to different rungs: a video-only clip is
blocked to pretraining, a license-unknown clip is hard-blocked to `archive_only`, and a
real-robot demo reaches the top of the ladder. Play/pause, a speed slider, and a source
picker drive it.

Below the belt, the static walkthrough remains — the three core ideas, the live
`examples/run_phase1.py` output, the byte-for-byte input/output artifact, the
trainability ladder (which the belt highlights in sync), and the three-phase roadmap.

**Live page:** https://e3f-six.github.io/robotis-convivium-demo/

The pipeline source, design docs, and tests live in the main (private) repository.
