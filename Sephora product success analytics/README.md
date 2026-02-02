# Sephora Product Success & Customer Review Insights  
### Product + Consumer Analytics Case Study 

**Adriana Cruz** | MS Business Analytics Candidate (UT Austin) | Marketing Analytics + Executive Storytelling  
**Tools:** Python (Pandas, Matplotlib, NLTK), Jupyter Notebook, Canva
**Dataset:** Sephora Products + Reviews (Kaggle)

---

## TL;DR  
This project analyzes Sephora product metadata and ~1.09M customer reviews to understand what drives high-performing products. I define a “High Performer” segment using customer engagement signals, benchmark performance across categories and brand tiers, and mine review phrases (n-grams) to uncover the highest-stakes customer expectations that influence satisfaction and dissatisfaction.

---

## Business Question  
Sephora carries thousands of skincare and beauty products across brands, categories, and price points. This analysis asks:

**What distinguishes Sephora’s high-performing products, and what do customer reviews reveal about the drivers of satisfaction and pain points?**

This is designed as an executive-facing analytics brief: insights are structured to support **merchandising, brand partnership, and product strategy decisions**.

---

## Dataset  
This project uses two main data sources from Kaggle:

- **Product metadata:** price, ratings, review counts, category hierarchy, brand info, engagement (“loves”)  
- **Customer reviews (~1.09M):** rating, recommendation flags, and written review text

> Note: I link to the dataset rather than uploading full raw data to GitHub (size + licensing).  
Kaggle Link: [ **(LINK)**](https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews)

---

## What I Built (Analytical Workflow)

### 1) Exploratory Data Analysis (EDA)  
I profiled the product dataset to understand structure and quality:
- schema review (columns + data types)
- missing value analysis (e.g., sale price often missing)
- basic distributions and sanity checks

**Why it matters:** EDA ensures the analysis uses reliable columns and avoids misleading conclusions caused by missing or inconsistent data.

---

### 2) Feature Engineering: Defining “High Performer”  
I created a binary KPI label:

- **high_performer = 1** for products above a defined engagement threshold (based on “loves” percentile)  
- **high_performer = 0** for all others

**Why it matters:** A clear success definition turns “what drives winners?” into a measurable question that can be compared across price, category, and brand.

---

### 3) Product Benchmarking (Winners vs Non-Winners)  
Using grouped aggregation (`groupby`), I compared high performers vs others across:
- price metrics (avg price for winners vs non-winners)
- customer satisfaction proxies (ratings, review volume)

**Why it matters:** This isolates what differs for “winning” products vs the baseline catalog.

---

### 4) Category Performance (Volume vs “Hit Rate”)  
I evaluated category performance in two ways:
- **Winner volume:** which categories contain the most high performers  
- **Success rate (“hit rate”):** share of products in a category classified as high performers

**Why it matters:** “Most winners” can simply reflect category size. “Hit rate” better reflects where Sephora has the highest probability of success.

---

### 5) Brand Benchmarking with Tiering (Fixing Catalog-Size Bias)  
A key issue: brands have very different catalog sizes (some have 10 products, others have 200+).  
To avoid unfair comparisons, I benchmarked brands using:

- total products per brand  
- winner count  
- success rate (winner share)

Then I segmented brands into tiers:
- **Emerging:** 10–19 products  
- **Established:** 20–49 products  
- **Powerhouse:** 50+ products

**Why it matters:** A brand with 10 products can look “perfect” by chance. Tiering creates fairer, more executive-relevant comparisons.

---

### 6) Review Analysis: Sentiment Labeling + Phrase Mining (NLP)  
I consolidated review files into a single dataset and created an interpretable sentiment proxy using star ratings:
- **Positive:** rating ≥ 4  
- **Negative:** rating ≤ 2  
- **Neutral:** rating = 3

Then I performed lightweight NLP / text mining:
- text cleaning + stopwords (NLTK + custom beauty-domain filtering)
- phrase extraction with **n-grams** (2–3 word phrases)
- comparison of top phrases in positive vs negative reviews

**Why it matters:** Star ratings alone don’t explain *why* customers love or dislike products. Phrase mining surfaces repeatable themes tied to satisfaction and churn.

---

### 7) “High-Stakes Attributes” Overlap Analysis  
I identified phrases that appear frequently in **both** positive and negative reviews.  
This overlap signals “high-stakes expectations” — product attributes customers care about most:
- deliver well → loyalty  
- fail → dissatisfaction

**Why it matters:** These themes are strategic levers for merchandising and product strategy (and can guide early warning monitoring).

---

## Key Insights (Executive Summary)

### Insight 1: High-performing products are not necessarily premium-priced  
Winners were often **lower-priced on average**, suggesting success is driven by perceived value and performance rather than luxury positioning alone.

### Insight 2: Category success is uneven — some categories have higher “hit rates”  
Categories vary in their probability of producing winners. Measuring both *volume* and *success rate* helps prioritize investment and shelf strategy.

### Insight 3: Brand performance depends on scale  
**Emerging brands represent high-upside breakout opportunities, while established brands deliver the most reliable and scalable performance.**  
Powerhouse brands win at volume but naturally show lower “winner concentration” due to large assortments.

### Insight 4: Review themes reveal the most important customer expectations  
Phrase mining surfaced recurring drivers of satisfaction and dissatisfaction tied to:
- sensitive/acne-prone skin compatibility  
- hydration + softness outcomes  
- sensory deal-breakers (smell/fragrance)  
- SPF finish issues (white cast)  
- value perception (“worth price tag”)

### Insight 5: The same attributes drive both love and hate  
Overlapping themes show that customers are outcome-driven — the features they praise most are also the ones that trigger disappointment when expectations are unmet.

---

## Strategic Recommendations  
1. **Prioritize sensitive-skin-safe innovation**  
   Sensitive/acne-prone compatibility is a dominant consumer segment and recurring theme.

2. **Reduce sensory friction to protect satisfaction**  
   Smell/fragrance and white cast appear as repeatable deal-breakers.

3. **Adopt a tier-based brand investment strategy**  
   Emerging = nurture breakout winners; Established = scale reliable performers; Powerhouse = anchor partnerships + monitor consistency.

4. **Integrate review-theme monitoring into merchandising decisions**  
   Use recurring complaint phrases as early warning signals for customer churn risk.

---

## Deliverables  
- **Notebook:** full Python analysis + visualizations  
- **Deck (PDF):** executive-style summary presentation  
