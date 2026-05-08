# 🗂️ Dataset Classification Taxonomy

This survey introduces a **6-dimensional classification** to characterize multi-choice MRC benchmark datasets. Each dimension captures a distinct aspect of dataset structure and difficulty.

---

## The 6 Dimensions

```
┌─────────────────────────────────────────────────────────┐
│               MRC Dataset Classification                │
├──────────────┬──────────────┬──────────────┬────────────┤
│ Corpus Style │    Domain    │  Complexity  │Context Style│
├──────────────┴──────────────┴──────────────┴────────────┤
│            Question Style      │       Answer Style      │
└────────────────────────────────┴────────────────────────┘
```

---

### 1. 📄 Corpus Style

How the source text is structured and presented.

| Style | Description | Example Datasets |
|-------|-------------|-----------------|
| Textual | Text-based content | CBT, RACE, SciQ |
| Multi-modal | Incorporates images, videos, or other media alongside text | MovieQA, RecipeQA |

---

### 2. 🌍 Domain

The subject area the content covers.

| Domain | Description | Example Datasets |
|--------|-------------|-----------------|
| Open | Diverse subjects, general knowledge | WikiHop, RACE, CBT |
| Closed | Specific domains | CliCR, BioRead, BioMRC (biomedical), SciQ (science) |

---

### 3. ⚙️ Complexity

The level of reasoning required to answer correctly.

| Level | Reasoning Type | Example Datasets |
|-------|---------------|-----------------|
| Simple | Straightforward comprehension, direct retrieval | CBT, BookTest, SciQ |
| Complex | Intricate analysis and integration of information | RACE, CLOTH, ARC |
| Commonsense | Requires implicit and real-world knowledge | ReCoRD, DREAM, CosmosQA |
| Multi-hop | Synthesizing information across multiple passages | WikiHop, MultiRC, QASC |
| Logical | Systematic application of formal logic | ReClor, LogiQA, RULE |

> **Note**: Complexity is one of the strongest predictors of the human–SOTA performance gap. High-complexity datasets (ReClor, LogiQA) show the largest remaining gaps.

---

### 4. 📑 Context Style

The format and length of the input passage(s).

| Style | Description | Example Datasets |
|-------|-------------|-----------------|
| Dialogue | Conversational exchanges | DREAM |
| Multimodal | Image-text or video-text combinations | MovieQA, RecipeQA |
| Single paragraph | Natural text in single paragraph | CBT, SciQ, ReClor |
| Multi paragraph | Natural text in multiple paragraphs | RACE, MultiRC, WikiHop |

---

### 5. ❓ Question Style

How questions are formulated.

| Style | Description | Example Datasets |
|-------|-------------|-----------------|
| Cloze | Fill-in-the-blank, sentence with missing word/phrase | ReCoRD, CBT, CLOTH |
| Tuple | (?, property, subject) triples | WikiHop |
| Natural | Typical query structure | RACE, SciQ, DREAM |

---

### 6. 💬 Answer Style

The format of the correct answer and distractors.

| Style | Description | Example Datasets |
|-------|-------------|-----------------|
| Static | Fixed number of options | RACE (4 options), CBT (10 options) |
| Dynamic | Varying number of options per question | MultiRC, ARC |
| Entity | Answer chosen from entity candidates | Quasar-S, CliCR, ReCoRD |

Additionally, answer types include: Verb, Pronoun, Named Entity, Common Noun, Phrase, Sentence, Word, Yes/No, Biomedical Entity, Clinical Entity, Person Named Entity.

---

## Example: Applying the Taxonomy

Here are illustrative examples of datasets for each category along with their types.

| Dataset | Corpus Style | Domain | Complexity | Context Style | Question Style | Answer Style | Answer Type |
|---------|-------------|--------|------------|---------------|----------------|--------------|-------------|
| CBT | Textual | Open | Complex | Single paragraph | Cloze | Static (10 options) | Verb, Pronoun, Named Entity, Common Noun |
| RACE | Textual | Open | Complex | Multi paragraph | Natural | Static (4 options) | Phrase, Sentence |
| SciQ | Textual | Closed (science) | Simple | Single paragraph | Natural | Static (4 options) | Word, Phrase |
| MultiRC | Textual | Open | Multi-hop | Multi paragraph | Natural | Dynamic | Phrase, Sentence |
| ARC | Textual | Open | Complex | Single paragraph | Natural | Dynamic | Word, Phrase, Sentence |
| MedQA | Textual | Closed (medical) | Complex | Multi paragraph | Natural | Static (5 options) | Word, Phrase |
| MCScript | Textual | Open | Commonsense | Single paragraph | Natural | Static (2 options) | Yes/No, Phrase, Sentence |
| MCScript2.0 | Textual | Closed (narrative) | Commonsense | Single paragraph | Natural | Static (2 options) | Yes/No, Phrase, Sentence |
| RACE-C | Textual | Open | Complex | Multi paragraph | Natural | Static (4 options) | Sentence |
| DREAM | Textual | Open | Commonsense | Dialogue | Natural | Static (3 options) | Word, Phrase, Sentence |
| CosmosQA | Textual | Open | Commonsense | Single paragraph | Natural | Static (4 options) | Sentence |
| ReClor | Textual | Open | Logical | Single paragraph | Natural | Static (4 options) | Sentence |
| QuAIL | Textual | Open | Commonsense | Multi paragraph | Natural | Dynamic | Phrase, Sentence |
| QASC | Textual | Open | Multi-hop | Multi paragraph | Natural | Static (4 options) | Word, Phrase |
| WDW | Textual | Open | Simple | Single paragraph | Cloze | Entity | Person Named Entity |
| BookTest | Textual | Open | Simple | Single paragraph | Cloze | Static (10 options) | Named Entity, Common Noun |
| Quasar-S | Textual | Open | Simple | Multi paragraph | Cloze | Entity | Named Entity |
| MovieQA | Multi-Modal | Open | Complex | Image, Dialogue | Natural | Static (5 options) | Phrase, Sentence |
| RecipeQA-text | Multi-Modal | Closed (cooking recipe) | Complex | Image, Recipe | Cloze | Static (4 options) | Phrase |
| CliCR | Textual | Closed (clinical) | Complex | Single paragraph | Cloze | Entity | Clinical Entity |
| CLOTH | Textual | Open | Complex | Single paragraph | Cloze | Static (4 options) | Word |
| ReCoRD | Textual | Open | Commonsense | Single paragraph | Cloze | Entity | Named Entity |
| WikiHop | Textual | Open | Multi-hop | Multi paragraph | Tuple | Entity | Named Entity |
| BioMRC | Textual | Closed (biomedical) | Simple | Single paragraph | Cloze | Entity | Biomedical Entity |
| BioRead | Textual | Closed (medical) | Simple | Single paragraph | Cloze | Entity | Biomedical Entity |
| Shmoop | Textual | Open | Simple | Multi paragraph | Cloze | Entity | Named Entity |
| LogiQA | Textual | Open | Logical | Single paragraph | Natural | Static (4 options) | Sentence |
| LogiQA2.0 | Textual | Open | Logical | Single paragraph | Natural | Static (4 options) | Sentence |
| ExpMRC-RACE+ | Textual | Open | Complex | Multi paragraph | Natural | Static (4 options) | Phrase, Sentence |
| RULE | Textual | Open | Logical | Single paragraph | Natural | Static (4 options) | Sentence |

---

> 💡 This taxonomy is designed to help researchers **select appropriate datasets** based on the specific capabilities they wish to evaluate or train for.
