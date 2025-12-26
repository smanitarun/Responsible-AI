# Responsible AI — Task B Red-Teaming Study (Confident-but-Wrong Hallucinations)

This repository contains a controlled red-teaming study of an LLM focused on “confident but wrong” hallucinations.
It includes:
- A locked experimental protocol (5 anchor questions × 3 prompt versions = 15 runs)
- A prompt pack (v1 baseline → v2 mitigation → v3 optimized responsible format)
- A scoring rubric and results table template
- Full prompt/response logs for the appendix
- Verification notes used to score correctness
- A paper draft following the required structure:
  Background/Introduction → Research Questions → Methods → Results → Discussion → Conclusion

## Study Design (Short)
- Model/platform: (fill: ChatGPT or academiccloud)
- Trials: 15 total
- Items: 5 anchor questions (medicine/history/bibliography; ethics-safe)
- Prompt versions: v1 (force guessing), v2 (don’t guess), v3 (calibrated responsible format)
- One-shot only: no follow-up questions
- Verification: performed after responses using reputable sources

## Folder Map
- protocol/ : study plan, anchors, prompts, scoring rubric
- data/ : results.csv with per-run scores
- appendix/logs/ : full prompt + response logs (run01–run15)
- verification/sources/ : links + short verification notes per run
- paper/ : draft.md and figures/
- ethics/ : ethics checklist used to scope the study safely
