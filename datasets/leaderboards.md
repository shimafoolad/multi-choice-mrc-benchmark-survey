# 🔗 Dataset Download & Leaderboard Links

> Only **41.37%** of the 30 surveyed datasets provide leaderboards and public download links.  
> Source: Tables 3 & 4 of the survey paper.

---

## Part 1 (2016–2018 Datasets)

| Year | Dataset | Download Link | Leaderboard Link | Test Data Public? |
|------|---------|--------------|-----------------|-------------------|
| 2017 | RACE | [↗ Download](http://www.cs.cmu.edu/~glai1/data/race/RACE.tar.gz) | [↗ Leaderboard](http://www.qizhexie.com/data/RACE_leaderboard.html) | ✔ |
| 2017 | WikiHop | [↗ Download](http://bit.ly/2m0W32k) | [↗ Leaderboard](https://qangaroo.cs.ucl.ac.uk/leaderboard.html) | ✗ |
| 2018 | MultiRC | [↗ Download](https://dl.fbaipublicfiles.com/glue/superglue/data/v2/MultiRC.zip) | [↗ SuperGLUE Leaderboard](https://super.gluebenchmark.com/leaderboard) | ✔ |
| 2018 | ARC | [↗ Download](https://ai2-public-datasets.s3.amazonaws.com/arc/ARC-V1-Feb2018.zip) | [↗ Leaderboard](https://leaderboard.allenai.org/arc/submissions/public) | ✔ |
| 2018 | RecipeQA-text | [↗ Download](https://hucvl.github.io/recipeqa/) | [↗ Leaderboard](https://hucvl.github.io/recipeqa/) | ✔ |
| 2018 | ReCoRD | [↗ Download](https://sheng-z.github.io/ReCoRD-explorer/) | [↗ ReCoRD](https://sheng-z.github.io/ReCoRD-explorer/) / [↗ SuperGLUE](https://super.gluebenchmark.com/leaderboard) | ✗ |

---

## Part 2 (2019–2022 Datasets)

| Year | Dataset | Download Link | Leaderboard Link | Test Data Public? |
|------|---------|--------------|-----------------|-------------------|
| 2019 | DREAM | [↗ Download](https://github.com/nlpdata/dream) | [↗ Leaderboard](https://dataset.org/dream) | ✔ |
| 2019 | CosmosQA | [↗ Download](https://github.com/wilburOne/cosmosqa/tree/master/data/) | [↗ Leaderboard](https://leaderboard.allenai.org/cosmosqa/submissions/public) | ✔ |
| 2020 | ReClor | [↗ Download](https://github.com/yuweihao/reclor/releases/download/v1/reclor_data.zip) | [↗ Leaderboard](https://eval.ai/web/challenges/challenge-page/503/leaderboard/1347) | ✔ |
| 2020 | QuAIL | [↗ Download](https://github.com/text-machine-lab/quail/) | [↗ Leaderboard](https://text-machine.cs.uml.edu/lab2/projects/quail/) | ✔ |
| 2020 | QASC | [↗ Download](https://ai2-public-datasets.s3.amazonaws.com/qasc/qasc_dataset.tar.gz) | [↗ Leaderboard](https://leaderboard.allenai.org/qasc/submissions/public) | ✔ |
| 2022 | ExpMRC-RACE+ | [↗ Download](https://github.com/ymcui/expmrc/tree/main/data/race) | [↗ Leaderboard](https://ymcui.com/expmrc/) | ✔ |

---

## ⚠️ Datasets Without Public Access

The following datasets from the survey either lack a public download link or have restricted access:

| Dataset | Reason |
|---------|--------|
| WDW (Who-Did-What) | Not publicly available |
| MedQA | No public link listed in survey |
| MCScript | No public link listed in survey |
| MCScript2.0 | No public link listed in survey |

---

## 🔒 Datasets Withholding Test Sets

**ReCoRD** and **WikiHop** do not release test data publicly to preserve the integrity of leaderboard evaluation. Researchers must submit predictions to the official evaluation servers.

---

## 🧩 Multi-Task Benchmarks Including MRC

Some MRC datasets are also part of broader multi-task benchmarks:

| Benchmark | Included MRC Datasets | Link |
|-----------|----------------------|------|
| SuperGLUE | ReCoRD, MultiRC | [↗](https://super.gluebenchmark.com/) |

---

> 💡 **Tip for researchers**: For the most up-to-date SOTA results, check [paperswithcode.com](https://paperswithcode.com/task/machine-reading-comprehension) and [eval.ai](https://eval.ai/) alongside the leaderboards listed above.
