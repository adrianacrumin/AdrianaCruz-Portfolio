# Instagram Engagement Analysis – Group project using Google Vision API, NLP, LDA & Logistic Regression

## Dataset  
 **National Geographic Instagram (scraped ~500 posts)**  
Each post includes:
1. Image URL
2. Caption
3. Like & comment counts
4. Google Vision API labels for each image  

## Project Overview  
This project explores how machine learning and image analytics can help content creators (like NatGeo) understand what drives engagement on social media. We extracted both textual and visual features to model and predict post performance.

As a group of 5, we combined natural language processing (NLP), Google Cloud Vision image analysis, and unsupervised topic modeling (LDA) to uncover which themes and content types lead to higher engagement.

### **Key Business Questions:**  
1. What kind of content gets more likes and comments?
2. Can we predict a post’s engagement just from its caption or image? 
3. Are there certain visual “topics” that consistently perform better?
 
---
## My Role
This was a group effort, and I worked mainly on:

1. Part C(2): I analyzed the topic weights across the top and bottom 25% of posts based on engagement score. The goal was to see if certain visual themes appeared more in highly engaging posts.
2. Part D: I wrote up the final insights and recommendations based on everything we found.

Specifically, I:

- Took the topic weights from the LDA model and matched them back to each Instagram post.
- Calculated engagement scores (likes + comments, normalized) and split the dataset into top and bottom quartiles based on engagement.
- Analyzed how average topic weights differed between the most and least engaging posts.
- Created a heatmap visualization that clearly showed which topics were more common in high-performing vs. low-performing content.
- Wrote up the final recommendation in Part D, connecting the data analysis to practical, real-world advice for NatGeo's content strategy.

---
## Results & Insights  

• Captions alone gave us some predictive power, but not enough on their own (accuracy around 62%)
• Image labels were more useful, and combining both gave us the strongest results
• Topic modeling helped us break down the kinds of images NatGeo posts — and which ones connect better with their audience

Some patterns stood out:

1. “Mountain Animals”-type images showed up more in popular posts.
2. “Rock Formation”-themed content was more common in lower-performing ones.

---
## Assignment Requirements  
*(This project was completed as part of a university course on data analytics and social media intelligence. The original assignment instructions have been reworded to respect academic guidelines.)*

In this group project, our objective was to analyze post engagement on National Geographic’s official Instagram account and uncover what types of content lead to higher audience interaction. The project focused on both **visual** and **textual** features to predict engagement and extract actionable insights.

**Below is a high-level summary of the assignment goals (rephrased for academic integrity):**

- Scraped approximately **500 image posts** from the @natgeo Instagram account (excluding videos).
- Collected the following data from each post:
  - Image URL  
  - Caption text  
  - Number of likes  
  - Number of comments  
- Used the **Google Vision API** to generate descriptive image labels for each photo.
- Created a custom **engagement score** using a weighted combination of likes and comments.
- Used **TF-IDF** to vectorize image labels and captions.
- Trained **logistic regression models** to predict whether a post had high or low engagement.
- Applied **LDA topic modeling** to the image labels to identify recurring visual themes.
- Compared how topic distributions varied across high and low engagement quartiles.
- Delivered final **recommendations** to help National Geographic increase engagement through visual strategy.

This project combined elements of **web scraping, natural language processing, computer vision, and machine learning** to explore how content performs in a real-world social media setting.

---

## What I Learned from This Project  

-**Engagement isn’t random — certain patterns show up clearly in the data.**
**Topic modeling is super useful when you want to understand what’s “in” an image without manually labeling it.**  
- **Collaboration makes projects like this 10× stronger — our group had a great balance of technical work and interpretation.** 
- **Insightful visualizations (like the heatmap and confusion matrix) make all the difference when communicating findings.**  

---

## Tools & Techniques Used  
- **Python** (Pandas, Scikit-learn, Matplotlib, Seaborn)  
- **Google Vision API**
- **TF-IDF** (for text + labels)
-**Logistic Regression**
- **LDA (Latent Dirichlet Allocation)**
- **Confusion Matrices & Heatmaps for visualization**

---
