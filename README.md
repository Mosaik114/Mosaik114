### Hi, I'm Mazgin 👋

Business informatics (Wirtschaftsinformatik) student at **Kiel University (CAU)** in Kiel,
Germany. In my free time I build tools that I use every day — mostly around **local AI, speech
recognition and Windows desktop software** — and I care about measuring what I build and
testing it properly.

I'm looking for opportunities in **AI-related software teams**.

---

#### How I build

I work **AI-native**: coding agents — mainly **Claude Code**, also OpenAI Codex — write much of
the code, and my job is everything around it:

- **Scope the problem** and decide the architecture and trade-offs (e.g. why Mosaik Capture is a
  tiny Rust host plus a WPF engine, or why Hams keeps audio processing on the GPU)
- **Direct the agents** in small, reviewable steps instead of one-shot prompts
- **Verify instead of trust:** tests for every behaviour, CI on every push, measurements before
  and after a change (Hams: latency 3.09 s → 0.72 s, word error rate per model)
- **Review independently:** Mosaik Capture went through ten rounds of independent code
  review; the real bugs they found (lost audio after 93 minutes, a pause/resume race, a
  double-save on double-click) were fixed and covered by tests

My role is closer to a tech lead than a typist: I read and adjust code, but mainly I own the
scope, the architecture and the quality bar — and I can explain why each part is built the way
it is. The agents make me faster; they don't make the decisions.

---

#### Featured projects

**[Kalino](https://github.com/Mosaik114/kalino)** — iPhone app for learning languages: Arabic, German and English, from the first letter to real texts  
Nine courses, each language learnable from the other two or from itself. Animated, hand-painted lessons,
spaced-repetition flashcards and a graded reader, all drawn in code. Private iCloud sync, on-device
StoreKit 2, no tracking and no server. In TestFlight with 1,500+ logic tests. Source code is private.  
`Swift` · `SwiftUI` · `SwiftData` · `CloudKit` · `StoreKit 2` · `Core Text`

**[Hams](https://github.com/Mosaik114/hams-bachelorprojekt)** — local, privacy-first voice input for Windows and Linux  
Hotkey → speak → corrected text appears at the cursor. faster-whisper on the GPU plus an
Ollama LLM for clean-up, all on the machine. Bachelor project at CAU Kiel: end-to-end latency
cut from **3.09 s to 0.72 s**, with measured word error rates and 1,500+ tests in CI.  
`Python` · `faster-whisper` · `CUDA` · `Ollama` · `Tkinter` · `Wayland portals`

**[Mosaik Capture](https://github.com/Mosaik114/mosaik-capture)** — keyboard-first screenshot and screen-recording tool for Windows  
A small Rust tray app drives a C#/WPF engine: freeze-frame capture, annotation editor with
shape recognition, offline OCR, GPU recording via Desktop Duplication with audio kept in sync
across pauses, trimming and GIF export. 560+ tests incl. real ffmpeg runs and pixel comparisons.  
`Rust` · `C#` · `WPF` · `Win32` · `WASAPI` · `ffmpeg`

---

#### Tech I work with

**AI-assisted development:** Claude Code · OpenAI Codex · agentic workflows (plan → implement → test → review)  
**Languages:** Python · Rust · C# · TypeScript · Swift  
**AI / audio:** faster-whisper · CTranslate2 · Ollama · WASAPI · ffmpeg  
**Engineering:** GitHub Actions CI · pytest · xUnit · cargo test · Win32 / COM interop · Linux (Wayland)

#### Contact

📫 [mazgin.ahmad@outlook.com](mailto:mazgin.ahmad@outlook.com)
