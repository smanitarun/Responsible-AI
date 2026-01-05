# Responsible AI — Red-Teaming Study (Confident-but-Wrong Hallucinations)# Responsible AI — Task B Red-Teaming Study (Confident-but-Wrong Hallucinations)



A controlled red-teaming study comparing hallucination behavior across **4 LLMs** using **2 hook questions** and **2 prompt versions**.This repository contains a controlled red-teaming study of an LLM focused on “confident but wrong” hallucinations.

It includes:

## Study Design- A locked experimental protocol (5 anchor questions × 3 prompt versions = 15 runs)

| Parameter | Value |- A prompt pack (v1 baseline → v2 mitigation → v3 optimized responsible format)

|-----------|-------|- A scoring rubric and results table template

| Models | GPT-5.2, o4-mini, Qwen 3 30B, Codestral 22B |- Full prompt/response logs for the appendix

| Hooks | 2 (1A: fabricated specifics, 1B: false premise) |- Verification notes used to score correctness

| Prompt versions | v1 (raw question), v2 (optimized anti-hallucination) |- A paper draft following the required structure:

| Total runs | 4 models × 2 hooks × 2 versions = **16** |  Background/Introduction → Research Questions → Methods → Results → Discussion → Conclusion

| One-shot only | No follow-up questions |

## Study Design (Short)

## Folder Map- Model/platform: (fill: ChatGPT or academiccloud)

```- Trials: 15 total

protocol/       study-plan, anchor questions, prompt pack, scoring rubric- Items: 5 anchor questions (medicine/history/bibliography; ethics-safe)

data/           results.csv (one row per run)- Prompt versions: v1 (force guessing), v2 (don’t guess), v3 (calibrated responsible format)

appendix/logs/  run01.txt – run16.txt (verbatim prompt + response + scoring)- One-shot only: no follow-up questions

verification/   per-run verification notes- Verification: performed after responses using reputable sources

paper/          draft.md, figures/

ethics/         ethics-checklist.md## Folder Map

```- protocol/ : study plan, anchors, prompts, scoring rubric

- data/ : results.csv with per-run scores

## Quick Start- appendix/logs/ : full prompt + response logs (run01–run15)

1. Run each of the 16 experiments (see `protocol/prompt-pack.md` for exact prompts).- verification/sources/ : links + short verification notes per run

2. Paste prompt + response into the corresponding `appendix/logs/runXX.txt`.- paper/ : draft.md and figures/

3. Score immediately using `protocol/scoring-rubric.md`.- ethics/ : ethics checklist used to scope the study safely

4. Update `data/results.csv` with one row per run.
5. Add verification notes in `verification/sources/runXX.md`.
6. Analyze and write up in `paper/draft.md`.
