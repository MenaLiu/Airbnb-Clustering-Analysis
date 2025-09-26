# Airbnb-Clustering-Analysis  
An unsupervised learning project applying clustering and PCA to segment Airbnb listings in Auckland.  
The study explores property characteristics, pricing patterns, and amenities to identify market segments.  

## Problem Statement  
How can clustering uncover meaningful market segments in Auckland’s Airbnb listings?  
This project investigates:  
- What property characteristics best differentiate listings?  
- How does PCA simplify high-dimensional features like amenities?  
- What distinct clusters emerge among Auckland Airbnb properties?  
- How can segmentation guide pricing and hosting strategies?  

## Methods  
**Data (Jan–Jun 2025):**  
- Source: [Airbnb](https://insideairbnb.com/get-the-data/) (Auckland subset)  
- ~6 months of listings  
- Features: price, review score, accommodates, bedrooms, bathrooms, room type, top 20 amenities (grouped into Safety, Essentials, Comfort, Extras)  

**Techniques Applied:**  
- Data cleaning & transformation → median imputation, quantile-based price levels (Low/Medium/High)  
- Feature engineering → amenities aggregated into 4 categories  
- PCA → visualization & variance explanation  
- K-means clustering (k=2–4 tested, k=3 selected)  
- Elbow & Silhouette methods → optimal cluster selection  

## Key Findings  
- **Cluster 1 (Low-cost, basic):** Budget listings, limited amenities, smaller capacity; essentials only (e.g., Wi-Fi, smoke alarms).  
- **Cluster 2 (Mid-range, comfort):** Medium-priced properties for 2–4 guests, offering balanced comfort (kitchen, heating, family/business friendly).  
- **Cluster 3 (High-end, feature-rich):** Premium listings with higher capacity, extra amenities (self-check-in, washers, luxury features).  

PCA confirmed that **price, capacity, and grouped amenities** explained most of the variation.  
Correlation analysis highlighted redundancy between bedrooms and accommodations, validated via a robustness dataset.  

## Conclusion  
The three-cluster segmentation provides actionable insights for Airbnb hosts in Auckland:  
- **Cluster 1 (Low-cost):** Compete on affordability, maintain minimum standards, and invest in low-cost upgrades (Wi-Fi, self-check-in).  
- **Cluster 2 (Mid-range):** Use dynamic pricing; highlight comfort and suitability for families/business travelers.  
- **Cluster 3 (High-end):** Position as premium stays; market unique features (designer interiors, outdoor spaces) to justify exclusivity.  

These results can help hosts refine pricing, improve amenities, and tailor marketing to their segment.  
