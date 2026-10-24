# Product Reviews Sentiment Analysis — Report Template

## 1. Introduction
This project applies sentiment analysis to online product reviews to understand customers' opinions.

## 2. Dataset and source
Dataset: Cleanlab Amazon Reviews, hosted on Hugging Face: https://huggingface.co/datasets/Cleanlab/amazon-reviews
The notebook selects up to 2,500 unique, non-empty reviews. This is an existing public dataset rather than a fresh scrape performed by the project team.

## 3. Methodology
The reviews are processed using VADER sentiment analysis. Compound scores are assigned to three classes: Positive (score >= 0.05), Negative (score <= -0.05), and Neutral (otherwise).

## 4. Results
After running the notebook, insert the actual count and percentage for each class from the summary table:
- Positive: [insert actual count and percentage]
- Negative: [insert actual count and percentage]
- Neutral: [insert actual count and percentage]

Insert `sentiment_distribution.png` here.

## 5. Discussion
Discuss which class is largest, what that suggests about the reviews in this dataset, and possible reasons. Base all claims on the output produced by the notebook.

## 6. Limitations
The dataset covers product reviews broadly rather than one single product. VADER can misclassify sarcasm, complex context, and some domain-specific phrases. The dataset is public and pre-existing, not freshly scraped for this project.

## 7. Conclusion
Summarize the observed sentiment distribution using the actual output. Suggest that product teams review recurring negative feedback to identify areas for improvement.

## References
Cleanlab. (n.d.). *Amazon Reviews dataset*. Hugging Face. https://huggingface.co/datasets/Cleanlab/amazon-reviews
Hutto, C. J., & Gilbert, E. (2014). VADER: A parsimonious rule-based model for sentiment analysis of social media text.
