# Emotions in Review: Leveraging Text Analytics for Enhanced Brand Insight

# Data Mining  
**Project By**: Suriya Subbiah Perumal  
  

---

## 📌 Overview

This project utilizes **Natural Language Processing (NLP)** and **semi-supervised machine learning** to extract emotional insights from customer reviews of two major brands. By combining **text analytics**, **sentiment analysis**, and the power of **Large Language Models (LLMs)** for translation and preprocessing, the study reveals how consumer emotions impact brand perception.

---

## 🧭 Methodology (CRISP-DM Framework)

1. **Business Understanding**: Analyze emotional tone in reviews for brand strategy.
2. **Data Understanding**: Identify language, review distribution, and anomalies.
3. **Data Preparation**:
   - HTML removal, punctuation cleaning
   - Translation using Google Translate API (`googletrans`)
   - NLP preprocessing (tokenization, stop-word removal, lemmatization via spaCy)
4. **Modeling**:
   - `SGDClassifier` for supervised learning
   - `SelfTrainingClassifier` for semi-supervised learning
5. **Evaluation**: Accuracy, Precision, Recall, F1-score
6. **Deployment**: Prediction dashboard and strategic visualization

---

## 🔍 NLP Pipeline

- **Language Detection**: `langdetect`  
- **Translation**: `googletrans` API  
- **Tokenization**: `nltk.word_tokenize()`  
- **Stop Word Removal**: `nltk.corpus.stopwords`  
- **Lemmatization**: `spaCy` (context-aware NLP)  
- **Vectorization**: `CountVectorizer`, `TF-IDF`  
- **Emotion Prediction Models**: `SGDClassifier`, `SelfTrainingClassifier`

---

## 🧠 Model Performance

| Model                 | Accuracy | Precision | Recall | F1 Score |
|----------------------|----------|-----------|--------|----------|
| Supervised (SGD)     | 49.2%    | 55.9%     | 49.2%  | 51.4%    |
| Semi-Supervised (LLM) | **85.7%** | High      | High   | High     |

The semi-supervised approach significantly outperformed the supervised model by effectively utilizing unlabeled data.

---

## 📊 Visual Analytics

- **Review Volume by Brand**: Brand H_ has more reviews → stronger customer engagement.
- **Top Countries per Brand**: US dominates Brand H_, showing regional brand strength.
- **Star Ratings**: Predominantly 5-stars, but 1-stars highlight service gaps.
- **Emotion Distribution**: 'Joy' most common, 'Anger' least frequent.
- **Star Rating vs Emotion**: Joy/surprise linked to higher ratings.
- **Brand vs Emotion**: Brand H_ consistently scores better across emotional categories.

---

## 📈 Key Technologies Used

- `pandas`, `matplotlib`, `seaborn` for data exploration
- `sklearn` for ML pipelines
- `nltk`, `spacy` for advanced NLP
- `googletrans`, `langdetect` for LLM-powered preprocessing
- Jupyter & Python for end-to-end automation

---

## 💡 Strategic Insights

- **Brand H_** shows higher joy/satisfaction, needs minor optimization.
- **Brand Z_** reveals emotional dissatisfaction — actionable intelligence for service and engagement revamp.
- Incorporating **LLMs for translation and sentiment mapping** significantly enhances the analysis.

---

## 📚 References

- Liu (2022), Pang & Lee (2008), Miner et al. (2012)
- Bottou (2010), Zhu & Goldberg (2009) on semi-supervised learning
- Manning et al. (2008), Silge & Robinson (2017) on NLP best practices
- Bird, Klein & Loper (2009) for NLTK use in NLP

---

## 📌 Conclusion

This study highlights how combining **NLP, LLMs**, and semi-supervised learning techniques can transform unstructured review data into strategic insights for brand management. The success of the semi-supervised model in leveraging unlabeled data underscores the growing role of intelligent algorithms in modern marketing analytics.

---

