# Instructor Guide

## Before the course

- Run Lab 00 in a fresh Colab runtime.
- Confirm the versions in `requirements.txt` remain available.
- Verify current IBM Quantum sign-in and token-saving instructions.
- Test at least one operational backend before Lab 03.
- Prepare a simulator-only alternative in case hardware access or queues are unavailable.

## Suggested teaching pattern

Begin each lab with its competency statement. Demonstrate one example, then require learners to predict the next circuit before executing it. Pause after visualizations and ask learners to connect amplitudes, probabilities, counts, and physical interpretation.

## Hardware lab safeguards

- Ask learners to enter tokens with `getpass` or Colab Secrets.
- Do not project, print, share, or commit tokens.
- Explain that transpiled circuits may use the backend's full register size.
- Treat queue time, calibration drift, and imperfect results as learning evidence.

## Assessment guidance

Use the following broad rubric for coding and problem-solving tasks:

| Criterion | Weight |
|---|---:|
| Correct circuit construction | 30% |
| Correct execution and measurement workflow | 25% |
| Interpretation of results | 30% |
| Clarity and reproducibility | 15% |

## Reproducibility

Record the software versions, backend name, shot count, and execution date for assessed hardware work. Counts are stochastic and should not be graded against one exact numerical output.
