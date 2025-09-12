# Arabic Implicit Emotion Recognition Dataset (AIER)

---

##  Overview

The **Arabic Implicit Emotion Recognition Dataset (AIER)** is a novel resource for implicit emotion recognition in Arabic text.

The dataset comprises **5,266** reviews collected from multiple Arabic sentiment resources, including the Hotel Arabic Review Dataset (HARD), the Book Reviews in Arabic Dataset (BRAD), and the Arabic Reviews Dataset by Elsahar et al. Each instance is meticulously annotated with one of six emotions—**anger, fear, joy, sadness, disgust, and surprise**— as well as semantic roles (**cue and cause**), providing a robust foundation for multiple natural language processing (NLP) tasks such as Emotion recognition, Implicit emotion detection, Semantic role labeling and Emotion cause detection.

Following the WASSA 2018 Implicit Emotion Shared Task, explicit emotion words in the reviews were **masked** with a **[MASK]** token. This process eliminates direct lexical cues of emotion, requiring models to rely on **contextual and linguistic information** for inference.


---


##  Dataset Description
- **Language:** Arabic  
- **Domain:** Reviews 
- **Total Size:** 5,266 reviews
- **Annotation:** Semi-automatic annotation
- **Subset Release:** 1,000 samples for early access  
- **Format:** CSV (UTF-8 encoded)  

### Data Columns
- `ID` → Unique identifier for each instance  
- `text` → The Arabic review  
- `cue` → The lexical trigger word indicating emotion  
- `emotion` → The annotated emotion class (anger, fear, joy, sadness, disgust, surprise)  
- `cause` → The cause or stimulus of the emotion expressed  

---

##  Dataset Versions
- **Subset Release** → Contains **1,000 samples** for early access and reproducibility.  
- **Full Dataset (upcoming)** → The complete dataset (5,266 reviews) will be released upon official publication of the paper.  

---


##  File Structure
```
AIER Dataset (subset).csv    # Subset release, contains the reviews along with their corresponding annotations.
README.md          # This file, offering detailed information about the dataset's contents and usage.
```

---

## Explore the Research

This dataset was utilized in the study titled "**Enhancement of Implicit Emotion Recognition in Arabic Text: Annotated dataset and baseline models**" (accepted in IEEE Access, 2025). The research investigates the challenges of implicit emotion recognition in Arabic and evaluates a range of models, from classical machine learning to BERT-based architectures and Generative LLMs.

### Paper Reference:

... 

---


## Abstract

Emotion recognition in textual data has emerged as a rapidly advancing task within the field of Natural Language Processing (NLP). Implicit Emotion Recognition (IER), which aims to identify emotions primarily through contextual cues rather than overt or explicit emotional expressions, remains in its early stages. Despite the significant progress in emotion recognition tasks, current research has largely ignored IER, particularly for low-resource languages such as Arabic. 

This study aims to comprehensively address this task for the Arabic language, including dataset construction, annotation, modeling, and evaluation. Specifically, the study (1) presents the first annotated dataset for Arabic Implicit Emotion Recognition (AIER); (2) annotates the dataset with emotion, cue, and cause using a semi-automatic annotation tool, validated by four native Arabic speakers and linguists; (3) investigates the potential of two categories of transformer-based models: masked language models, exemplified by pre-trained Bidirectional Encoder Representations from Transformers (BERT)-based architecture, through a series of fine-tuning experiments, and causal-based models, such as generative Large Language Models (LLMs), via a zero-shot prompting approach; and (4) evaluates the performance of four distinct algorithmic models on the proposed dataset :classical Machine Learning (ML), Deep Learning (DL), BERT-based, and generative LLMs. 

The experimental results demonstrate that BERT-based models outperform ML, DL models, and generative LLMs. Notably, the fine-tuned MARBERTv2 model achieves superior performance compared to other pre-trained models, obtaining an impressive F1-score of 79.83% on the AIER dataset.


---


## 🧾 Citation
If you use this dataset in your research or any other work, please cite the following paper:


**IEEE Access paper (BibTeX):**
```bibtex
@article{...,
  author    = {...},
  title     = {Enhancement of Implicit Emotion Recognition in Arabic Text: Annotated dataset and baseline models},
  journal   = {IEEE Access},
  year      = {2025},
  doi       = {10.1109/ACCESS.xxxxxxx},
}
```

---

##  License
This dataset is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.  

For any further inquiries or questions about the dataset, please reach out to the authors of the paper.

---


## Future Work
- Release of the **full dataset** (5,266 reviews) after official IEEE Access publication.  
