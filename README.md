# Amazon Product Reviews Sentiment Analysis

## Project objective
Analyze 2,500 product reviews and categorize them as Positive, Negative, or Neutral using VADER sentiment analysis.

## Dataset
- Source: [Cleanlab Amazon Reviews on Hugging Face](https://huggingface.co/datasets/Cleanlab/amazon-reviews)
- The source page describes 5,000 training samples with `review_text` and an existing positive/negative label.
- This notebook selects up to 2,500 unique, non-empty review texts.
- This is a public pre-existing dataset, not a fresh scrape from Amazon. Please state that clearly in the submission.

## How to run without installing Python
1. Open [Google Colab](https://colab.research.google.com/).
2. Choose **File → Upload notebook**.
3. Upload `product_reviews_sentiment.ipynb` from this repository/ZIP.
4. Run each code cell from top to bottom (click the play icon beside each cell).
5. The final cell downloads `analysed_product_reviews.csv` and `sentiment_distribution.png`.

## Method
VADER calculates a compound sentiment score for each review:
- `>= 0.05`: Positive
- `<= -0.05`: Negative
- otherwise: Neutral

## Output
- `analysed_product_reviews.csv`: review text, compound score, and sentiment class
- `sentiment_distribution.png`: bar chart of positive, negative, and neutral reviews

## Limitations
VADER is a rule-based English-language sentiment tool and can misunderstand sarcasm, context, or domain-specific wording. The source dataset covers product reviews broadly; it is not restricted to one single product. Do not describe the data as personally scraped.
