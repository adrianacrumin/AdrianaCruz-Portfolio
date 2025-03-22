# Entry-Level Luxury Car Market Analysis

## Dataset  
 **I scraped approximately 5,000 user posts from the Entry-Level Luxury Performance Sedans forum on Edmunds.com. These posts contain organic conversations about a range of car brands and models, offering valuable insight into how consumers talk about cars — what they care about, what they compare, and what they want.**  
Each post includes:
1. Date of posting
2. User-submitted message content


## Project Overview  
This project was designed to help J.D. Power better understand brand positioning and consumer preferences in the entry-level luxury car space. Using real social media conversations, we applied frequency analysis, association rules, and multidimensional scaling (MDS) to uncover competitive relationships and feature associations across the top brands.

### **Key Business Questions:**  
1. Which car brands are most frequently mentioned in entry-level luxury car discussions?
2. How are brands associated with one another in consumer conversations?
3. What does the brand landscape look like in terms of perceived similarity?
4. What are the five most important features that people care about when discussing these cars?
5. Which brands are most strongly tied to those features?
6. Which brand is most “aspirational” — the one people say they want to own?
7. What recommendations can we give manufacturers based on these consumer-driven insights?
---
## My Role
This was a group project, and I contributed in the following ways:

1. Web Scraping (Solo):
   - I personally built and ran the scraper to collect ~5,000 posts from Edmunds.com. I navigated the site's old forum structure, handled pagination, cleaned the data, sorted it from newest to oldest, and exported it into a clean CSV format for the team to use in all later tasks.
2. Task D: Brand Relationship Insights
   - Togehter we analyzed the lift ratios and MDS map from Tasks B and C to explain which brands are closely associated in consumers’ minds, and what those associations mean from a competitive strategy perspective.
3. Task E: Attribute Analysis
   - Together we identified the top 5 most frequently mentioned car attributes (e.g., performance, design, reliability), and mapped them to the brands they’re most strongly associated with in the conversations.
4. Task F: Strategic Recommendations
   - Based on the attributes and brand connections, we all contributed to the final client-facing advice — outlining how different car brands should market their strengths and what features matter most to buyers in this segment.

---
## Results & Insights  

• **Top 10 Brands Mentioned:** Included BMW, Audi, Lexus, Acura, Infiniti, and others. These were identified based on frequency after normalizing model mentions into brand-level categories.
• **Brand Associations (Lift Ratios):** For example, Audi and BMW were often co-mentioned, suggesting strong head-to-head comparisons in the minds of consumers.
•**MDS Mapping:** Brands that cluster together on the MDS map reflect perceived similarity (e.g., Acura and Infiniti were closer to each other than to BMW or Audi).

---
## Assignment Requirements  
*(This project was completed as part of a university assignment focused on competitive intelligence and text analytics.)*

The original assignment was designed around a real-world scenario: J.D. Power & Associates is seeking insights into how consumers perceive different entry-level luxury car brands in the U.S. Our job was to act as data consultants and use online forum data to explore brand positioning, key attributes, and consumer sentiment.

**Below is a high-level summary of the assignment goals (rephrased for academic integrity):**

- Scrape ~5,000 posts from the **Edmunds.com Entry-Level Luxury Performance Sedans** forum, capturing user conversations.
- Analyze brand frequency and standardize mentions at the brand (not model) level.
- Calculate **brand associations** using lift scores (while avoiding duplicate counts within the same post).
- Use **multidimensional scaling (MDS)** to visualize the relative similarity between brands.
- Identify the **top 5 most frequently mentioned car attributes** and match them to associated brands.
- Offer **business advice** based on observed brand-attribute links.
- Determine which brand appears most **aspirational** — based on how people express desire to buy or own it.

All insights were generated from real user discussions — no surveys, no assumptions — giving the client (J.D. Power) a grounded understanding of how these brands are talked about in the wild.

---

## What I Learned from This Project  

- **Real-world forums are messy **— scraping requires patience, smart structure handling, and cleanup.
- **Association analysis (like lift) provides more than just co-occurrence;** it reveals deeper competitive framing.
- **MDS is a powerful way to visually compare how brands are positioned in consumers’ minds.**
- **Combining qualitative forum data with quantitative techniques** gives you insights that feel both grounded and strategic.

---

## Tools & Techniques Used  
- **Python** (Requests, BeautifulSoup, Pandas, Scikit-learn, Matplotlib)  
- **Text Mining & NLP**
- **Web Scraping**
- **Frequency & Lift Calculations**
- **Multidimensional Scaling (MDS)**

---

