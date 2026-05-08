# 📊 Multi-Choice MRC Datasets — Part 2 (2019–2023)

> Source: Table 2 of the survey paper.  
> **ACC** = Accuracy | **F1/EM** = F1 / Exact Match  
> **Solved**: ✔ model surpassed human performance | ✗ not yet solved | — no human baseline available

---

| Year | Dataset | Vocab Size | Questions | Context Size | Data Source | Metric | Human (%) | SOTA (%) | Solved | Dataset Link |
|------|---------|-----------|-----------|--------------|-------------|--------|-----------|----------|--------|--------------|
| 2019 | [MCScript2.0](https://github.com/mrcdata/race-c) | 12k | 20k | 3k | Narrative | ACC | 97.0 | — | ✗ | — |
| 2019 | [RACE-C](https://github.com/mrcdata/race-c) | 58k | 14k | 4k | English exam | ACC | — | — | — | [↗](https://github.com/mrcdata/race-c) |
| 2019 | [DREAM](https://dataset.org/dream/) | 10k | 10k | 6k | English exam (dialog) | ACC | 98.6 | 92.6 | ✗ | [↗](https://dataset.org/dream/) |
| 2019 | [CosmosQA](https://wilburone.github.io/cosmos) | 40k | 35.6k | 21.9k | Blogs, Narrative | ACC | 94 | 91.7 | ✗ | [↗](https://wilburone.github.io/cosmos) |
| 2019 | [Shmoop](https://www.cs.toronto.edu/~makarand/shmoop/) | — | 7k | 7k | Project Gutenberg | ACC | — | 40 | — | [↗](https://www.cs.toronto.edu/~makarand/shmoop/) |
| 2020 | [BioMRC](https://huggingface.co/datasets/viewer/?dataset=biomrc&config=biomrc_large_A) | — | 812k | 812k | PUBTATOR | ACC | — | 88 | — | [↗](https://huggingface.co/datasets/viewer/?dataset=biomrc&config=biomrc_large_A) |
| 2020 | [ReClor](https://whyu.me/reclor/) | 17k | 6k | 6k | GMAT/LSAT exam | ACC | 63.0 | 90.2 | ✔ | [↗](https://whyu.me/reclor/) |
| 2020 | [QuAIL](https://text-machine.cs.uml.edu/lab2/projects/quail/) | 17k | 15k | 800 | News, Stories, Fiction, Blogs | ACC | 60.0 | 53.4 | ✗ | [↗](https://text-machine.cs.uml.edu/lab2/projects/quail/) |
| 2020 | [QASC](https://allenai.org/data/qasc) | 1.6M | 10k | 17M | Science exam, WorldTree | ACC | 93 | 93 | ✔ | [↗](https://allenai.org/data/qasc) |
| 2020 | [LogiQA](https://github.com/lgw863/LogiQA-dataset) | — | 8.6k | 8.6k | Chinese Civil Service Exam | ACC | 86/95 | 49.17 | ✗ | [↗](https://github.com/lgw863/LogiQA-dataset) |
| 2022 | [ExpMRC-RACE+](https://ymcui.com/expmrc/) | — | 1k | 335 | RACE dataset | ACC | 84.4 | 50.86 | ✗ | [↗](https://ymcui.com/expmrc/) |
| 2023 | [LogiQA2.0](https://github.com/csitfun/LogiQA2.0) | — | 15.7k | 15.7k | Chinese Civil Service Exam | ACC | 84/98 | 54.93 | ✗ | [↗](https://github.com/csitfun/LogiQA2.0) |
| 2023 | [RULE](https://github.com/nii-cl/rule) | 9k | 4k | 943 | Exam | ACC | 81.5 | 69.2 | ✗ | [↗](https://github.com/nii-cl/rule) |

---

## 🔍 Key Observations

### Unsolved Datasets (significant human–SOTA gap)

These datasets have the largest gap between human and SOTA performance, making them the most interesting targets for future research:

| Dataset | Human (%) | SOTA (%) | Gap |
|---------|-----------|----------|-----|
| LogiQA | 86.0–95.0 | 49.17 | ~37–46 pts |
| LogiQA2.0 | 84.0–98.0 | 54.93 | ~29–43 pts |
| QuAIL | 60.0 | 53.4 | ~6.6 pts |
| ExpMRC-RACE+ | 84.4 | 50.86 | ~33.5 pts |
| DREAM | 98.6 | 92.6 | ~6 pts |

### Solved Datasets (model ≥ human)

| Dataset | Human (%) | SOTA (%) |
|---------|-----------|----------|
| ReClor | 63.0 | 90.2 |
| QASC | 93.0 | 93.0 |

---

## 📝 Notes

- **RACE-C** has no reported human or SOTA performance, making it difficult to assess current model ceiling.
- **LogiQA** and **LogiQA2.0** use Chinese Civil Service Exams — models show the largest performance gap here, suggesting logical/formal reasoning remains a major open challenge.
- **ReClor** is notable: human performance is unusually low (63%), yet models now exceed it (90.2%), suggesting the dataset may reward pattern-matching over true logical reasoning.
- **QuAIL** blends four source types (news, stories, fiction, blogs), making it one of the most diverse small-scale datasets.

---

⬅️ Back to [datasets_part1.md](datasets_part1.md)  
🔗 See [leaderboards.md](leaderboards.md) for all download and leaderboard links.
