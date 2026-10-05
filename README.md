# MagBERT-NER-AR — Tutorial

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assoudi-typica-ai/magbert-ner-ar-tutorial/blob/main/MagBERT_NER_AR_Tutorial.ipynb)

A short, ready-to-run tutorial for [**MagBERT-NER-AR**](https://huggingface.co/TypicaAI/MagBERT-NER-AR), an Arabic (Modern Standard Arabic) named entity recognition model trained on a corpus curated from **Moroccan newspapers**. It works on standard Arabic news text and is especially well adapted to Moroccan entities: names, cities and provinces, institutions, laws and date conventions.

Click the badge above to open the notebook in Google Colab. No setup is required: the model is downloaded from the Hugging Face Hub, and the notebook runs on CPU or GPU.

## What the notebook covers

1. Loading the model with 🤗 Transformers
2. Quick start with the `pipeline` API
3. A BILUO-aware helper that returns clean multi-word entities
4. Right-to-left entity visualization with displaCy
5. Results on Moroccan-context news examples (institutions, local administration, events, laws, sport, regions)
6. The same sentence with Moroccan, Egyptian and Levantine date conventions
7. Batch processing into a pandas DataFrame
8. A text box to try your own sentence

## Run locally

```bash
git clone https://github.com/assoudi-typica-ai/magbert-ner-ar-tutorial.git
cd magbert-ner-ar-tutorial
pip install transformers torch spacy pandas jupyter
jupyter notebook MagBERT_NER_AR_Tutorial.ipynb
```

## Model

| | |
|---|---|
| Model | [TypicaAI/MagBERT-NER-AR](https://huggingface.co/TypicaAI/MagBERT-NER-AR) |
| Base model | [asafaya/bert-base-arabic](https://huggingface.co/asafaya/bert-base-arabic) |
| Language | Modern Standard Arabic (Arabic script) |
| Tagging scheme | BILUO |
| History | First trained April 2021, retrained August 2023 (v0.1.1) |

Out of scope: Moroccan Darija, Arabizi and Latin-script text.

## License

The tutorial code in this repository is released under the MIT License. The **model** has its own license; see the [model card](https://huggingface.co/TypicaAI/MagBERT-NER-AR).

## Contact

**Hicham Assoudi** — [Typica.ai](https://typica.ai) · assoudi@typica.ai · [LinkedIn](https://www.linkedin.com/in/assoudi) · 🤗 [TypicaAI](https://huggingface.co/TypicaAI)
