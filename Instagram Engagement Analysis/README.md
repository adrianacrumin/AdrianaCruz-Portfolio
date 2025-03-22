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

1. “Savannah”-type images (like animals, warm landscapes) showed up more in popular posts.
2. “Tundra”-themed content (snow, ice, cold settings) was more common in lower-performing ones.

---
## Assignment Requirements  
(*For academic transparency, these are the original instructions.*)  

On Instagram, choose the National Geographic page (Natgeo) -- do not use hashtags. Write a
scraper to extract (i) image URLs (do not extract video URLs, it may end up costing you quite a bit of money to run analytics on video), (ii) post caption (the text description of a post), (iii) # likes and (iv) # comments. You don’t need actual comments for this assignment. Scrape around 500 image posts.

Using the image URLs, obtain image labels from Google Vision cloud (you will have to create an account with Google to get your credentials as a json file, though the first $300 are free, which should be more than plenty for this assignment). You will need to write a script to access the Google Vision API. You can also use IBM Watson Vision Analytics (the basic account is free) as an alternative (if you are not a Google fan). Read about Google Vision here: For Google Vision API, look here.

Task A. Create a metric for engagement by using a weighted sum of # likes and # comments.
[]

Task B. Using TF-IDF scores, run a logistic regression with engagement (binary) as the
dependent variable, and the image labels as independent variables. []

Task C. Perform topic modeling (LDA) on the image labels. Choose an appropriate number of
topics. [] Now take the quartiles with highest and lowest engagement scores. What are the differences in the average topic weights of pictures across the two quartiles (e.g., greater proportion of some topics in highest engagement quartile)? []

Task D. What advice would you give National Geographic if it wants to increase engagement on
its Instagram page based on your findings in Tasks B and C?

Deliverables: Create a Python notebook with all code. Also submit all data files. Write the
names of all team members inside the notebook.
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
