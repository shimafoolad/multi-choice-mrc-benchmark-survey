# 📊 Multi-Choice MRC Datasets — Part 1 (2016–2018)

> Source: Table 1 of the survey paper.  
> **ACC** = Accuracy | **F1/EM** = F1 / Exact Match  
> **Solved**: ✔ model surpassed human performance | ✗ not yet solved | — no human baseline available

---

| Year | Dataset | Vocab Size | Questions | Context Size | Data Source | Metric | Human (%) | SOTA (%) | Solved | Dataset Link |
|------|---------|-----------|-----------|--------------|-------------|--------|-----------|----------|--------|--------------|
| 2016 | [CBT](http://www.thespermwhale.com/jaseweston/babi/CBTest.tgz) | 53.6k | 687k | 108 books | Stories, Narrative | ACC | 81.6 | 74.9 | ✗ | [↗](http://www.thespermwhale.com/jaseweston/babi/CBTest.tgz) |
| 2016 | [MovieQA](https://github.com/makarandtapaswi/MovieQA_CVPR2016) | 21k | 15k | 408 movies | Plots, Subtitles, Video clips, Scripts, DVS | ACC | — | 42.53 | — | [↗](https://github.com/makarandtapaswi/MovieQA_CVPR2016) |
| 2016 | [WDW](https://tticnlp.github.io/who_did_what/) | 347k | 330k | 206k | Gigaword | ACC | 84 | 72.6 | ✗ | 🔒 Not public |
| 2017 | [BookTest](https://ibm.ent.box.com/v/booktest-v1) | 200k | 14M | 13.5k books | Project Gutenberg | ACC | 81.6 | 83.7 | ✔ | [↗](https://ibm.ent.box.com/v/booktest-v1) |
| 2017 | [Quasar-S](https://github.com/bdhingra/quasar) | 987k | 37k | — | Stack Overflow | ACC | 50 | 33.6 | ✗ | [↗](https://github.com/bdhingra/quasar) |
| 2017 | [WikiHop](http://qangaroo.cs.ucl.ac.uk/) | 304k | 51k | 49k | Wikipedia | ACC | — | 84.4 | — | [↗](http://qangaroo.cs.ucl.ac.uk/) |
| 2017 | [RACE](https://www.cs.cmu.edu/~glai1/data/race/) | 136k | 97k | 27k | English exam | ACC | 94.5 | 91.4 | ✗ | [↗](https://www.cs.cmu.edu/~glai1/data/race/) |
| 2017 | [SciQ](https://allenai.org/data/sciq) | 23k | 13k | 13k | Science exam | ACC | 87.8 | 96.6 | ✔ | [↗](https://allenai.org/data/sciq) |
| 2018 | [RecipeQA-text](https://hucvl.github.io/recipeqa/) | 63k | 36k | 19k recipes | Instructables.com | ACC | 73.6 | 47.5 | ✗ | [↗](https://hucvl.github.io/recipeqa/) |
| 2018 | [CliCR](https://github.com/clips/clicr) | 122k | 105k | 12k | BMJ Clinical Case Reports | F1/EM | 53.7/35 | 33.9/24.5 | ✗ | [↗](https://github.com/clips/clicr) |
| 2018 | [CLOTH](https://www.cs.cmu.edu/~glai1/data/cloth/) | 37k | 99k | 7k | English Exam | ACC | 85.9 | 70.7 | ✗ | [↗](https://www.cs.cmu.edu/~glai1/data/cloth/) |
| 2018 | [ReCoRD](https://sheng-z.github.io/ReCoRD-explorer/) | 139k | 121k | 73k | News article | F1/EM | 91.7/91.3 | 96.4/95.9 | ✔ | [↗](https://sheng-z.github.io/ReCoRD-explorer/) |
| 2018 | [BioRead](https://archive.org/details/bioread_dataset.tar) | 3.9M | 16.4M | 16.4M | PubMed Central | ACC | — | 51.19 | — | [↗](https://archive.org/details/bioread_dataset.tar) |
| 2018 | [MultiRC](https://cogcomp.seas.upenn.edu/multirc/) | 23k | 6k | 871 | News and other web pages | F1 | 81.8 | 89.6 | ✔ | [↗](https://cogcomp.seas.upenn.edu/multirc/) |
| 2018 | [ARC](https://allenai.org/data/arc) | 4M | 7k | 14M | Science exam | ACC | — | 86.9 | — | [↗](https://allenai.org/data/arc) |
| 2018 | MedQA | — | — | 243k | Medical exam | ACC | — | 75.3 | — | — |
| 2018 | MCScript | 8k | 32k | 2k | Scripts, CRW | ACC | 98.2 | 84.8 | ✗ | — |

---

## 📝 Notes

- **WDW** is not publicly available, limiting its utility for reproducible research.
- **BioRead** and **BioMRC** are restricted to the medical domain (PubMed Central / PUBTATOR).
- **CBT** and **BookTest** are the largest general-domain datasets but use older sources (Project Gutenberg).
- **ReCoRD** and **WikiHop** do not release test data publicly to preserve leaderboard integrity.

---

➡️ Continue to [datasets_part2.md](datasets_part2.md) for datasets from 2019–2023.  
🔗 See [leaderboards.md](leaderboards.md) for all download and leaderboard links.
