# Extraction of Future Statements A Multilingual Benchmark


This repository contains the dataset for the paper titled "Extraction of Future Statements: A Multilingual Benchmark". The dataset provides gold-standard annotations for future-looking statements extracted from news articles in three languages.

---

## Datasets

The repository contains the following three files:

* `goldEN.json`: The annotated dataset for English news articles.
* `goldDE.json`: The annotated dataset for German news articles.
* `goldFR.json`: The annotated dataset for French news articles.

---

## Data Structure

Each JSON file contains an array of objects. Each primary object has the following structure:

* `original_text`: A string containing the full text of the source news article.
* `extracted`: An array of objects, where each object represents a single extracted future statement with the fields described below.

### Fields of an Extracted Statement

Each JSON object represents a single extracted future statement and contains the following fields:

| Field                          | Description |
| **Event Variable**             | The specific entity or variable the prediction is about. |
| **Event Category**             | The category of the predicted event. |
| **Predicted Attribute**        | Qualitative details about the event. |
| **Magnitude / Predicted Value**| The predicted numerical value or percentage. |
| **Predictor**                  | The person or organization making the prediction. |
| **Event Date**                 | The expected date or the mentioned timeframe of the predicted event. |
| **Article Date**               | The publication date of the article, if available. |
| **Assumptions / Preconditions**| Conditions or assumptions required for the event to occur. |
| **Enabling Factor**            | Condition which facilitate the predicted outcome (used in few-shot/CoT). |
| **Blocking Factor**            | Condition which hinders the predicted outcome (used in few-shot/CoT). |
| **Credibility of Source**      | Assessment of the source’s reliability (0.0 to 1.0). |
| **Credibility rationale**      | A brief justification for your rating. |
| **Rationale**                  | The explanation given in the article to support the prediction. |
| **Modality**                   | The degree of certainty expressed (0.0 to 1.0). |
| **Modality evidence**          | The specific phrase or expression justifying the rating. |

---
