# Decoding Sephora’s Winners: An Analytics Case Study on What Really Drives Product Success


Sephora’s shelves offer a vibrant marketplace across makeup, skincare, and fragrance. But for the brand and its partners, this variety creates a critical business challenge: how do certain products become massive, high-performing “winners,” and what truly drives that success?

This case study uses over 1 million customer reviews and Sephora's product data to deliver a clear, executive-level answer, focusing on two core questions:

- What distinguishes high-performing products from the rest of the catalog?
- What do customers consistently praise or criticize in products that succeed?

This project is an end-to-end demonstration of how consumer analytics can transform raw data into a strategy-ready plan.

---

# The 9-Step Strategy to Uncovering High-Performing Products

## Step 1: Get to Know Your Data (The Catalog Audit)

The first step in any robust analysis is ensuring the reliability of your raw data. We began by loading the Sephora product dataset and performing exploratory profiling, checking the structure, data types, and, crucially, missing values.

The Goal:  
To answer a foundational question: what information can I trust, and what should I avoid using as a key business metric?

The Finding:  
Certain pricing fields, like sale price, were frequently incomplete. However, base price had strong data coverage. This immediate finding shaped which reliable metrics we could use for later comparisons, avoiding inaccurate conclusions based on incomplete data.

---

## Step 2: Define "Success" as a Measurable Outcome

To determine what drives product success, we first needed a clear, measurable definition of what a “high-performing” product is. Since revenue and profit data were unavailable, we used customer engagement as a reliable proxy.

The Proxy:  
Sephora's "loves" signal, a direct measure of customer engagement and desire,was used as the KPI.

The Benchmark:  
We created a binary segmentation:  
High Performers (products above a defined engagement threshold) and  
Non-High Performers (the rest of the catalog).

This step is both feature engineering and a core business decision. Once success is defined, performance becomes measurable against categories, brands, and pricing.

---

## Step 3: Benchmarking: Winners vs. Non-Winners

With the high-performer segment defined, we ran direct comparisons to answer the first executive question: What distinguishes high-performing products from the rest of the catalog?

The Key Discovery:  
High-performing products were not necessarily premium-priced. In many cases, winners were lower priced on average compared to non-winners.

The Strategic Insight:  
This re-frames product success as something driven by perceived value and reliable performance, not just luxury positioning. It suggests that growth can come not only from high-end offerings, but from products that reliably deliver results at accessible price points.

---

## Step 4: Categories: Measuring Both Volume and "Hit Rate"

Next, we mapped where Sephora’s winners concentrate across the product ecosystem. To create a strategy-friendly view, we evaluated category performance in two ways:

Winner Volume: Which categories contain the most high performers.  
Success Rate ("Hit Rate"): Within a category, what percentage of products are winners.

This distinction is critical: Large categories will naturally have a higher volume of winners. The Success Rate reveals something different—where Sephora has the best probability of producing a winning product. This allows leadership to prioritize category investment based on probability, not just size.

---

## Step 5: Brand Performance: Control for Scale is Key

Ranking brands by their winner rate can be misleading, as brand catalogs vary significantly in size. A small brand with a few hits can look exceptional, while a large brand's overall success rate is naturally diluted.

The Solution:  
Tiering: To correct for this bias and support fair benchmarking, we segmented brands into three tiers based on catalog size:

Emerging Brands: 10–19 products (The "up & coming" tier)  
Established Brands: 20–49 products  
Powerhouse Brands: 50+ products

The Executive Interpretation:  
The Emerging tier represents the high-upside breakout opportunities that Sephora may want to invest in, tapping into the desire for the "new." Established brands deliver reliable and scalable performance, while Powerhouse brands remain critical anchor partners.

---

## Step 6: Shift from Product Metrics to Customer Voice

Product metrics tell what happens. Customer reviews explain the crucial “why.” We consolidated over one million review files and created an interpretable baseline for sentiment:

Positive: 4–5 stars  
Negative: 1–2 stars  
Neutral: 3 stars

This star-rating proxy for sentiment is simple, effective, and easy to communicate to stakeholders.

---

## Step 7: Course Correction: Why Phrases Beat Single Words

Our initial approach of analyzing common single words was technically functional but produced results that were not stakeholder-friendly. High-frequency single words were generic (“feel,” “work,” “product”) and lacked actionable context.

The Turning Point:  
We shifted from single-word analysis to phrase extraction using n-grams (2–3 word phrases).

The Result:  
This shift was essential because phrases capture full intent and helped us understand the specific strengths and weaknesses of the products. For example, instead of the generic word “smell,” customers wrote the phrase "get past smell." Instead of “acne,” they wrote "sensitive acne prone.” This contextual detail made the insights far more actionable for product development.

---

## Step 8: Phrase Mining for Business-Ready Themes

Analyzing these 2–3 word phrases allowed us to surface the repeatable themes that drive both satisfaction and pain.

Drivers of Satisfaction (Praise)  
Consistent Pain Points (Criticism)

Hydration and softness outcomes  
Visible improvement (fine lines, brightening)  
Sensitive/acne-prone compatibility

Fragrance and smell as deal-breakers  
SPF finish issues such as white cast  
Value dissatisfaction (“worth price tag”)

---

## Step 9: The Key Insight: High-Stakes Customer Expectations

One of the most important findings was that the same themes appeared in both positive and negative reviews. This is not an analytic flaw; it’s a powerful signal that customers are consistently outcome-driven.

The Strategy:  
The attributes customers praise most are also the ones that trigger disappointment when expectations aren't met.

These become High-Stakes Attributes, areas where consistency matters most for customer satisfaction and retention. This tells leadership exactly what customers care about enough to create loyalty or cause them to churn.

---

# Actionable Recommendations for Sephora

Based on the combined product benchmarking and customer voice analysis, four strategic actions emerge:

- Prioritize Sensitive-Skin-Safe Innovation: Sensitive/acne-prone compatibility is a recurring, high-stakes consumer priority.  
- Reduce Sensory Friction: Smell/fragrance concerns and SPF white cast repeatedly appear as deal-breakers that ruin the customer experience.  
- Adopt Tier-Based Brand Investment: Use the Emerging vs. Established vs. Powerhouse segmentation to guide partnership strategy and growth investment, prioritizing emerging brands for high-upside opportunities.  
- Operationalize Review-Theme Monitoring: Treat recurring complaint phrases as early warning signals for churn risk, and use them to inform both marketing clarity and future product development.
