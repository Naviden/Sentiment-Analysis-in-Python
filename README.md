# Sentiment Analysis in Python

A comprehensive educational repository covering sentiment analysis techniques — from lexicon-based methods to large language models. Designed for teaching and self-study, with theoretical background and executable Jupyter notebooks for each approach.

## Repository Structure

```
.
├── Theory/
│   ├── Basic Concepts.md                          # Fundamentals of sentiment analysis
│   └── Approaches.md                              # Overview of all approaches with comparison table
├── Tools/
│   ├── 01 - Knowledge-Based Approach.ipynb             # Simple custom-lexicon sentiment scoring
│   ├── 02 - VADER in Detail.ipynb                      # VADER lexicon-based analysis walkthrough
│   ├── 03 - TextBlob in Detail.ipynb                   # TextBlob polarity and subjectivity analysis
│   ├── 04 - VADER, Naive Bayes, and LSTM.ipynb         # Benchmark comparison on IMDB reviews
│   ├── 05 - Sentence-BERT.ipynb                        # SBERT embeddings + classification
│   ├── 06 - LLM Sentiment Analysis (OpenRouter).ipynb  # Zero/few-shot with LLMs via API
│   └── 07 - Case Study.ipynb                           # Applied analysis of literary texts (no labels)
├── Data/
│   ├── A.txt                    # Alice's Adventures in Wonderland (full text)
│   └── K.txt                    # The Metamorphosis by Franz Kafka (full text)
├── requirements.txt
└── README.md
```

## Methods Covered

| Method | Notebook | Approach Type |
|--------|----------|---------------|
| Custom Lexicon | `01 - Knowledge-Based Approach.ipynb` | Knowledge-based |
| VADER | `02 - VADER in Detail.ipynb` | Knowledge-based (rule-enhanced) |
| TextBlob | `03 - TextBlob in Detail.ipynb` | Knowledge-based |
| Naive Bayes + BoW | `04 - VADER, Naive Bayes, and LSTM.ipynb` | Machine learning |
| LSTM Neural Network | `04 - VADER, Naive Bayes, and LSTM.ipynb` | Deep learning |
| Sentence-BERT | `05 - Sentence-BERT.ipynb` | Transfer learning |
| LLM Prompting (OpenRouter) | `06 - LLM Sentiment Analysis (OpenRouter).ipynb` | Large language models |
| Applied Case Study | `07 - Case Study.ipynb` | Applied / no ground truth |

## Getting Started

### Prerequisites

- Python 3.9+
- Basic familiarity with Python and machine learning concepts

### Installation

```bash
git clone https://github.com/Naviden/Sentiment-Analysis-in-Python.git
cd Sentiment-Analysis-in-Python
pip install -r requirements.txt
```

For the LLM notebook, you will also need an [OpenRouter](https://openrouter.ai/) API key:

```bash
export OPENROUTER_API_KEY="your-key-here"
```

### Dataset

The notebooks in `Tools/` use the [IMDB Reviews dataset](https://ai.stanford.edu/~amaas/data/sentiment/) (Maas et al., 2011), loaded automatically via `tensorflow_datasets`. The Case Study notebook uses two literary texts included in `Data/`: *Alice's Adventures in Wonderland* and *The Metamorphosis*.

## Suggested Learning Path

1. **Theory** — Read `Basic Concepts.md` and `Approaches.md`
2. **`01`** — Build a minimal lexicon-based classifier from scratch
3. **`02`** — Explore VADER in depth
4. **`03`** — Explore TextBlob in depth
5. **`04`** — Compare VADER, Naive Bayes, and LSTM on a labeled benchmark (IMDB)
6. **`05`** — Sentence-BERT: transfer learning without fine-tuning
7. **`06`** — LLM prompting via OpenRouter (zero-shot, few-shot, chain-of-thought)
8. **`07`** — Case Study: apply the tools to literary texts with no ground truth

## References

- Hutto, C.J. & Gilbert, E.E. (2014). VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. *ICWSM*.
- Maas, A.L., et al. (2011). Learning Word Vectors for Sentiment Analysis. *ACL*.
- Reimers, N. & Gurevych, I. (2019). Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks. *EMNLP*.
- Brown, T., et al. (2020). Language Models are Few-Shot Learners. *NeurIPS*.
- Wei, J., et al. (2022). Chain-of-Thought Prompting Elicits Reasoning in Large Language Models. *NeurIPS*.
- Reagan, A.J., et al. (2016). The emotional arcs of stories are dominated by six basic shapes. *EPJ Data Science*.

## License

This project is intended for educational purposes.

## Contributing

Contributions are welcome. Please open an issue or submit a pull request.
