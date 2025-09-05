# Exploring Language Patterns in Multilingual Climate Messages
## Overview
During the LUNE-TWO Fellowship, I co-created a multilingual dataset of climate messages in English, Yoruba, Hausa, and Igbo alongside 2 linguists. I wanted to see what more could be learned from it, so I ran an experiment: what happens when we cluster these messages using embeddings?
This project is my exploration of that question.

## What I Did
- Cleaned and tokenised the climate messages.
- Used XLM-Roberta to generate sentence embeddings.
- Applied  `K-Means clustering` and tested cluster quality.
- Visualised patterns with `PCA` and `t-SNE`.

## What I Found
- Yoruba and Igbo messages often clustered together, which makes sense given their shared Niger–Congo roots.
- Hausa, from a different language family (Afro-Asiatic), formed its own group.
- The clustering quality was solid (Silhouette Scores: Yoruba 0.605, Hausa 0.579, Igbo 0.618).
- Visual plots gave a clear picture of these language relationships.

<img width="948" height="527" alt="Screenshot 2025-04-17 at 06 21 45" src="https://github.com/user-attachments/assets/bc330102-4228-4c7f-ae50-db3969940404" />

  
## Why It Matters
This exercise shows how AI/ML techniques can reveal structure in underrepresented languages and hints at applications like:
- Better multilingual climate communication.
- Tools for translation, retrieval, or summarisation in African contexts.
- Making crucial information more accessible across language barriers.

## Next Steps
- Try other models like AfriBERTa and mBERT.
- Expand to more African languages.
- Test downstream tasks such as classification or topic modelling.
