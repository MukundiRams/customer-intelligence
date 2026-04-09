# Customer Intelligence Platform — Customer Segmentation & Personalisation System

## Project Overview
This notebook implements an end-to-end customer segmentation and product 
recommendation system for a fictional South African retail bank, RetailCore. 

The system:
- Generates 2000 synthetic but realistic banking customers using controlled 
  statistical distributions
- Performs exploratory data analysis with validation, cleaning and visualisation
- Applies KMeans clustering with PCA dimensionality reduction to identify 
  4 distinct customer segments
- Recommends personalised bank products for each segment based on financial 
  eligibility and ownership gap analysis
- Predicts the segment and recommended products for new customers in real time
- Generates natural language segment summaries using the Google Gemini API

## Reproducibility
All random processes use a fixed seed (numpy.random.seed(42)) to ensure 
fully reproducible results.



## Conclusion & Business Recommendations

This analysis identified four distinct customer segments within the bank's 
customer base:

- **Premium Loyalists (16%)** — High-value, deeply engaged customers requiring 
  wealth deepening strategies
- **Stable Middles (32%)** — Reliable core customers ready for product depth 
  expansion  
- **Emerging Potentials (32%)** — Financially disciplined low-income customers 
  representing significant growth opportunity
- **Financially Vulnerable (20%)** — At-risk customers requiring intervention 
  over revenue focus

### Key Strategic Insights
1. Digital disengagement is the earliest and most reliable churn signal
2. Product depth (active_products_count) is the strongest retention predictor
3. Branch visit spikes in digitally inactive customers signal distress, 
   not engagement
4. LSM 1-4 customers are underserved — entry-level products represent 
   significant untapped revenue with manageable risk

### Limitations & Future Work
- Silhouette scores below 0.25 indicate overlapping cluster boundaries.s
- Recommendation gap scores are uniform for new products — ownership 
  tracking should be extended to all catalogue products
- Model should be retrained quarterly as customer behaviour evolves


