<picture>
  <source media="(prefers-color-scheme: dark)" srcset="banner-dark.svg">
  <img alt="Sreya Sivan. AI engineer. Retrieval, extraction and evaluation on real data." src="banner-light.svg" width="100%">
</picture>

I'm Sreya Sivan, an AI engineer in Coimbatore, India. I build systems that answer from real documents and measure whether they got it right.

## Now

Studying **Data Science with AI at DataMites** full time since June 2026: Python, machine learning, NLP, databases, big data foundations.

Building **[LabelLens](https://github.com/Sreyasivan/labellens)**: cited question answering and typed extraction over FDA drug labels, with an evaluation harness that runs on every push.

- 2,000 prescription labels from openFDA in Postgres with pgvector and full-text search, hybrid retrieval fused with reciprocal rank fusion.
- A 100-question set, every question verified against the label text before it counts. Retrieval recall@5 97/100; all 16 off-topic questions refused before the model is called.
- Extraction of contraindications, interactions and warnings into typed lists: 221 items, none containing words that are not in the label.
- A judged faithfulness metric whose judge is itself scored against hand-labelled pairs, so its number comes with its own accuracy.
- A local 3B model by default so label text never leaves the machine; OpenAI or Claude by changing environment variables.
- CLI, FastAPI service with generated docs, a plain web page, and CI that fails if recall drops.

The README has the numbers, what they do and do not prove, and the design decisions.

Also **[FAERS serious-outcome classifier](https://github.com/Sreyasivan/faers-serious-outcome)**: on
397,224 real FDA adverse-event reports from one quarter, predict death, life-threatening event or
hospitalisation. Logistic-regression baseline (AUROC 0.83) against gradient boosting (0.87), both
calibrated; two leaks found by EDA and removed, with the inflated score they would have given quoted
in the model card.

## Before that

**AI intern at [Prayag.ai](https://prayag.ai)**, Jun 2025 to Apr 2026. Built a business development agent in Python, automated data extraction from client emails with the GPT-4 API, and designed RAG chatbot architectures. That code is the company's, so it is not here.

**B.Tech in Information Technology**, Karpagam Institute of Technology, 2022 to 2026 (CGPA 8.00).

## Projects

- **[LabelLens](https://github.com/Sreyasivan/labellens)**: RAG, structured extraction and evals on FDA drug labels. Python, Postgres, pgvector, sentence-transformers, pydantic, FastAPI, pytest, GitHub Actions.
- **[FAERS serious-outcome classifier](https://github.com/Sreyasivan/faers-serious-outcome)**: tabular ML on real adverse-event reports with a model card. Python, pandas, scikit-learn, matplotlib, pytest.

## Open to

AI/ML engineer and data science roles in Coimbatore, Bengaluru, Chennai or remote.

## Elsewhere

[sreyasivan.me](https://sreyasivan.me) · [LinkedIn](https://www.linkedin.com/in/sreyasivan) · contact@sreyasivan.me
