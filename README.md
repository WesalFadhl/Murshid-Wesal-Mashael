<div align="center">

# Murshid Mini
### LLM Application Engineering · SDA-AIE-213

**Build from scratch. Keep one notebook. Finish one project.**

A guided four-day learning journey by **Meaad Al-Marri**

[Start learning](#start-here) · [Daily labs](#your-four-day-roadmap) · [Video learning path](docs/videos.md) · [Expected results](expected/README.md) · [Submit your project](docs/git.md)

</div>

---

## What you will build

A small fictional service assistant that answers known service questions, reads application status through an authorized tool, rejects unsuitable inputs, tests its behavior and caches public answers safely. Each day extends the **same project in the same saved Colab notebook**. Day 4 completes that project; there is no separate capstone.

| Learning level | Time | Environment | Cost |
|---|---|---|---|
| Beginner to intermediate; basic Python familiarity | 4 days × 4 hours, including prayer breaks and a daily 1-hour lab | Google Colab · Python 3 · CPU | No paid API, key, GPU, model download or extra package |

> **Know what this project is:** `mode=mock`. `FakeClient` is a finite, deterministic simulator, **not a live language model**. You are learning the engineering around an LLM-shaped interface. The notebook does not train a model, assess live LLM quality or implement production security. All data is synthetic.

## Independent extensions and extra homework

The required four-day mock project below remains unchanged. For a separately runnable real CPU model demonstration, additional tool-protocol and evaluation homework, worked solutions, observed outputs and intentional error examples, open the [independent extension learning path](extensions/README.md). These optional activities use separate notebooks outside the core lab hour. Real-model activities require library and model downloads; no API key or paid inference service is required. Follow the [extension learning roadmap](extensions/OBJECTIVES.md), [video path](extensions/VIDEOS.md), and [self-check](extensions/VERIFICATION.md).

## Start here

**New to Python, Colab or GitHub?** Begin with the [ordered video learning path](docs/videos.md), then return here. Videos are optional preparation and reinforcement, not extra graded work or prerequisites involving paid services.

1. **Prepare:** read [Setup and recovery](docs/setup.md). Use Python 3 with CPU/no accelerator. Nothing needs installing.
2. **Create once:** open [Google Colab](https://colab.research.google.com/) and create a blank notebook named `murshid_your_name.ipynb`. Save it in your own Drive.
3. **Build Day 1:** open the [Day 1 guide](docs/day-1.md) beside Colab. Add its labeled code blocks one at a time; predict, run, inspect and explain the result.
4. **Keep building:** return to **your original saved notebook** each day. Append the next day's cells below the earlier ones. Do not create four projects or overwrite your progress with the reference.
5. **Save evidence:** download your notebook and the day's JSON outputs before leaving. Commit each milestone to your own repository with a meaningful message.

**GitHub is your learning guide; Colab is your code workspace.** Explanations, slide mappings, dataset documentation and expected results stay here. The notebook uses code cells only, with short code comments and printed outputs.

<details>
<summary><strong>Need the complete reference for comparison or recovery?</strong></summary>

[Open the reference in Colab](https://colab.research.google.com/github/almiyead-rgb/murshid-llm-application-engineering-sda-aie-213/blob/main/notebooks/murshid.ipynb) · [View it on GitHub](notebooks/murshid.ipynb)

Save your own copy before editing. Use this to check work or recover a broken cell, not to skip building the stages. Only run through the day you are studying. If the link does not open, in Colab choose File → Open notebook → GitHub, paste this repository URL, select `notebooks/murshid.ipynb`, and save your copy.

</details>

## Your four-day roadmap

Slides 1–16 provide concepts and activities; slides 17–20 guide the day's lab. Each guide maps its steps to the relevant slide ranges in the final **20-slides-per-day** course content.

| Day | Build today | Notebook cells | Guide and code | Compare your result |
|---|---|---:|---|---|
| **1 · Foundations** | Synthetic directory, mock client, `ask`, response contract | 1–3 | [Guide](docs/day-1.md) · [Code](labs/day1.py) | [Three known answers](expected/baseline_results.json); blank input adds no mock call |
| **2 · Structure and tools** | Validated ticket, read-only status lookup, ownership check | 4–6 | [Guide](docs/day-2.md) · [Code](labs/day2.py) | [Five scenarios](expected/day2_results.json); no unauthorized status disclosure or mutation |
| **3 · Guard and test** | Versioned prompt artifact, guards, pipeline, ten golden cases | 7–10 | [Guide](docs/day-3.md) · [Code](labs/day3.py) | [10/10 fixed behavioral cases](expected/day3_results.json) |
| **4 · Measure and finish** | Public exact cache, measurements, regression, export | 11–14 | [Guide](docs/day-4.md) · [Code](labs/day4.py) | [3→1 mock calls; 66.7% hits](expected/day4_results.json) · [Final report](expected/final_report.json) |

**Daily schedule:** 150 minutes of teaching and activities + 30 minutes reserved for two prayer breaks + 60 minutes lab. Actual break positions follow local prayer times. Videos are outside this lab schedule unless the instructor selects an excerpt.

### The learning loop

**Read → predict → build → run → compare → explain → save.**

The code is provided in small labeled blocks. Type or copy each block into a new cell, understand it, and test it before continuing. Explain one decision to a partner and document a small change without weakening tests. Helpers for saving JSON, reference extraction, timing and export keep the lab realistic for a one-hour session. Running copied code alone does not demonstrate understanding.

## Save your work and submit one repository link

Keep **one cumulative Colab notebook for the core project** and **a separate Drive-saved Colab notebook for each homework**. Upload your project, completed homework and results into your own GitHub repository. Then send your repository's root link to the instructor through her specified submission channel, checking that she can access it.

Follow the [beginner's guide to saving, uploading and submitting](docs/git.md): suggested filenames, folder structure, GitHub upload steps and a final access/privacy checklist are provided there.

## Extra homework by day

Open the section for your current day. Each has the task, how to run, the expected result, and links to the solution and video. Use separate notebooks for these optional activities; keep your cumulative core project intact.

[Day 1: real model](docs/day-1.md#extra-homework) · [Day 2: tools](docs/day-2.md#extra-homework) · [Day 3: error handling](docs/day-3.md#extra-homework) · [Day 4: evaluation](docs/day-4.md#extra-homework)

## Your learning library

| I need… | Go to… |
|---|---|
| Videos in a sensible order from the basics | [Video learning path](docs/videos.md) |
| Environment setup, saving or runtime recovery | [Setup and troubleshooting](docs/setup.md) |
| What the data means and where it comes from | [Dataset card](data/README.md) · [Synthetic data](data/synthetic_data.json) |
| What the application components do | [Technical documentation](docs/technical.md) |
| Expected outputs and what may vary | [Results guide](expected/README.md) |
| How to use Git and prepare my own repository | [Versioning and submission](docs/git.md) |
| The finished code-only notebook | [Reference notebook](notebooks/murshid.ipynb) |
| Automated checks | [Tests](tests/test_notebook.py) |

## Understand the dataset before coding

No dataset download is required. The small teaching dataset is embedded in the code:

- A public service directory with an Arabic and an English answer.
- `REF-1001`, owned by fictional `demo-user-1`, with status `under_review`.
- `REF-1002`, owned by fictional `demo-user-2`, with status `approved`.
- `REF-9999`, intentionally absent, for a negative test.

The session fixture is `demo-user-1`. Knowing a reference number does **not** prove ownership. The read-only tool checks the trusted fixture before returning a status. These rules are educational, not real authentication. See the [dataset card](data/README.md) for fields, boundaries and privacy rules. Never add actual ministry records or personal data.

## Compare results honestly

Run your notebook from the top and compare its outputs with the [reference results](expected/README.md). Check the ten golden cases, then verify the cache experiment and the saved final report. A correct refusal counts as a successful test when the request should be rejected.

- **Compare:** answer fields, status codes, tool-call counts, pass/fail results and cache-hit sequence.
- **Do not require exact matches:** UUID trace IDs and Python execution times.
- **Do not infer:** real LLM quality, comprehensive security, a measured API speedup or actual financial savings.

Before submitting, save your work, restart your Colab runtime, and run the notebook cells in order. Use [setup and recovery](docs/setup.md) if a cell fails. Save your own results; opening the reference notebook’s stored output is not the same as running your copy.

<details>
<summary><strong>Run tests locally or rebuild the reference notebook</strong></summary>

Use Python 3.9+ from the repository directory:

```bash
python -m unittest discover -s tests -v
```

After editing lab source files:

```bash
python tools/build_notebook.py
python tools/record_reference.py
python -m unittest discover -s tests -v
```

Run scripts in one shared process or run notebook cells sequentially; Day 2 depends on Day 1. See [setup](docs/setup.md) for the local runner. Rebuilding clears notebook outputs; `record_reference.py` regenerates observed outputs.

</details>

## Finish with a repository you can explain

Use the full [submission checklist](docs/git.md). Your own repository should contain:

- A clear project description and professional README with setup, use and limitations.
- The one cumulative notebook you built across the four days.
- Synthetic-data and technical documentation.
- Your own generated results and honest evaluation report.
- Meaningful daily Git commits demonstrating progress.
- Attribution to **LLM Application Engineering · SDA-AIE-213**, instructor **Meaad Al-Marri**, and the relevant [SDAIA Academy GitHub account](https://github.com/SDAIAAcademy).

The generated ZIP contains JSON outputs, **not your notebook**. Download and save the notebook separately. Review all files for private information before sharing. The repository does not claim Academy endorsement or certification of the implementation.

## Contribute to the Saudi technical community

Explore high-quality Saudi projects, star work you genuinely value, follow relevant accounts, contribute useful improvements, open constructive issues and pull requests, fork when appropriate, and share outstanding projects. These are voluntary community activities, **not grading requirements**. Respect each project's contribution guide and license.
