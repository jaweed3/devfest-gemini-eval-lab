# Can Gemini Actually See?

A hands-on workshop for building a multimodal AI evaluation lab with Gemini.

> A demo can look convincing and still be wrong. This workshop shows how to measure the difference.

## Workshop proposal

**Can Gemini Actually See? Building a Multimodal AI Evaluation Lab**

Participants will build a small evaluation pipeline for Gemini's multimodal vision capabilities. Starting from a labeled image dataset, they will send images to Gemini, enforce structured JSON output, compare predictions with ground-truth labels, and inspect failure cases such as overconfidence, hallucinated visual evidence, ambiguous inputs, and prompt sensitivity.

The session goes beyond image description demos. Participants will experiment with zero-shot and few-shot prompts, evidence fields, confidence estimates, and abstention for uncertain inputs. They will then calculate accuracy, per-class performance, confusion patterns, latency, and abstention rate with a lightweight evaluator.

The central engineering question is: **how do we evaluate a multimodal AI system beyond a convincing demo?** Attendees will leave with a working Gemini-based evaluation pipeline and a repeatable method for testing multimodal AI applications before deployment.

## Session details

- **Format:** Hands-on workshop
- **Duration:** Up to 90 minutes
- **Audience:** Intermediate
- **Prerequisites:** Basic Python familiarity; no prior ML research experience required
- **Platform:** Google AI Studio and Gemini API
- **Status:** Draft proposal for DevFest Cloud Surabaya 2026

## Learning outcomes

Participants will learn to:

1. Build a Gemini image-evaluation pipeline.
2. Request structured JSON instead of free-form responses.
3. Compare model predictions against ground truth.
4. Measure accuracy and per-class performance.
5. Analyze overconfident errors and hallucinated evidence.
6. Add abstention for uncertain inputs.
7. Distinguish a prototype, a benchmark, and reliable evidence.

## Planned workshop flow

1. **The demo trap** — why a fluent answer is not evidence.
2. **First vision prompt** — run a zero-shot Gemini experiment.
3. **Structured output** — define prediction, evidence, confidence, and abstention fields.
4. **Automatic evaluation** — calculate metrics and inspect a confusion matrix.
5. **Prompt experiments** — compare zero-shot, few-shot, and uncertainty-aware prompts.
6. **Failure analysis** — investigate wrong, inconsistent, and overconfident responses.
7. **Deployment discussion** — decide what should be measured before shipping.

## Safety and scope

The demo uses an educational image-classification dataset. It is not a medical, veterinary, or diagnostic system. The workshop emphasizes uncertainty, evaluation, and responsible interpretation rather than presenting Gemini's output as ground truth.

## Repository structure

```text
prompts/       Prompt variants used in the workshop
sample_data/   Small labeled demo dataset
src/           Evaluation code (to be added)
notebooks/     Guided experiments (to be added)
```

## License

Code and original workshop materials are released under the MIT License. Dataset images retain the license and attribution requirements of their original source; see `sample_data/README.md` when sample data is added.
