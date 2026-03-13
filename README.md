# Sentiment Analysis in Python

A comprehensive educational repository covering sentiment analysis techniques — from lexicon-based methods to large language models. Designed for teaching and self-study, with theoretical background and executable Jupyter notebooks for each approach.

## Repository Structure

```
.
├── Theory/
│   ├── Basic Concepts.md                          # Fundamentals of sentiment analysis
│   └── Approaches.md                              # Overview of all approaches with comparison table
├── Tools/
│   ├── Knowledge-Based Approach.ipynb             # Simple custom-lexicon sentiment scoring
│   ├── VADER in Detail.ipynb                      # VADER lexicon-based analysis walkthrough
│   ├── Textblob in Detail.ipynb                   # TextBlob polarity and subjectivity analysis
│   ├── Tools.ipynb                                # VADER, Naive Bayes, and LSTM on IMDB reviews
│   ├── Sentence-BERT Sentiment Analysis.ipynb     # SBERT embeddings + classification
│   ├── LLM Sentiment Analysis (OpenRouter).ipynb  # Zero/few-shot with LLMs via API
│   └── Case Study.ipynb                           # Multi-method comparison on literary texts
├── Data/
│   ├── A.txt                    # Alice's Adventures in Wonderland (full text)
│   └── K.txt                    # The Metamorphosis by Franz Kafka (full text)
├── requirements.txt
└── README.md
```

## Methods Covered

| Method | Notebook | Approach Type |
|--------|----------|---------------|
| Custom Lexicon | `Tools/Knowledge-Based Approach.ipynb` | Knowledge-based |
| VADER | `Tools/VADER in Detail.ipynb` | Knowledge-based (rule-enhanced) |
| TextBlob | `Tools/Textblob in Detail.ipynb` | Knowledge-based |
| Naive Bayes + BoW | `Tools/Tools.ipynb` | Machine learning |
| LSTM Neural Network | `Tools/Tools.ipynb` | Deep learning |
| Sentence-BERT | `Tools/Sentence-BERT Sentiment Analysis.ipynb` | Transfer learning |
| LLM Prompting (OpenRouter) | `Tools/LLM Sentiment Analysis (OpenRouter).ipynb` | Large language models |

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

1. **Theory** — Read `Basic Concepts.md` and `Approaches.md` for foundational understanding
2. **Lexicon methods** — Work through the Knowledge-Based, VADER, and TextBlob notebooks
3. **Machine learning** — Follow the Naive Bayes and LSTM sections in `Tools.ipynb`
4. **Transformer embeddings** — Explore the Sentence-BERT notebook
5. **LLM prompting** — Experiment with zero-shot, few-shot, and chain-of-thought in the OpenRouter notebook
6. **Applied analysis** — Run the Case Study to compare VADER, TextBlob, and SBERT on literary texts

## References

- Hutto, C.J. & Gilbert, E.E. (2014). VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. *ICWSM*.
- Maas, A.L., et al. (2011). Learning Word Vectors for Sentiment Analysis. *ACL*.
- Reimers, N. & Gurevych, I. (2019). Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks. *EMNLP*.
- Brown, T., et al. (2020). Language Models are Few-Shot Learners. *NeurIPS*.
- Wei, J., et al. (2022). Chain-of-Thought Prompting Elicits Reasoning in Large Language Models. *NeurIPS*.

## License

This project is intended for educational purposes.

## Contributing

Contributions are welcome. Please open an issue or submit a pull request.
