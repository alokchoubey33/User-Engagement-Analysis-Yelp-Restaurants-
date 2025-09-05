# 📊 User Engagement Analysis (Yelp Restaurants)

A data analysis project exploring how user engagement on Yelp (reviews, tips, and check-ins) relates to restaurant success metrics such as review counts and average star ratings, with geographic, temporal, sentiment, and user-type insights.

# 🗂️ Table of Contents

Overview

Problem Statement

Research Objectives

Hypotheses

Data Overview

Methods

Analysis & Findings

Recommendations

How to Reproduce

Project Structure

Visuals

Limitations

Future Work

License

Acknowledgements

# 🔍 Overview
This repository analyzes relationships between user engagement signals on Yelp and restaurant success metrics, surfacing correlations, time trends, seasonality, city-level differences, elite user impact, and operational insights like busiest hours.

# 🎯 Problem Statement

In a competitive restaurant market, stakeholders need to understand drivers of success. This project examines how reviews, tips, and check-ins relate to review counts and average ratings for restaurants.

# 📝 Research Objectives

Quantify correlations between engagement (reviews, tips, check-ins) and review count/average star rating.

Examine time trends in engagement and ratings.

Compare engagement between high-rated and low-rated restaurants.

Explore geographic variation in success metrics.

Assess sentiment proxies (useful, funny, cool) and their association with success.

Evaluate elite user contributions and engagement patterns.

# 🧪 Hypotheses

Higher engagement correlates with higher review counts and ratings.

Positive sentiment in reviews and tips contributes to higher ratings and review counts.

Consistent engagement over time is associated with sustained business success.

# 🗃️ Data Overview

Subset of Yelp across 8 metros in the USA and Canada.

Original data as JSON: business, review, user, tip, checkin.

JSON loaded into a relational database for efficient joins.

# 🛠️ Methods

Ingestion from Yelp JSON into relational tables.

Feature engineering for engagement metrics and rating categories.

Descriptive statistics for review counts and ratings.

Correlation analysis across engagement and sentiment proxies.

Temporal analysis with trend/seasonality decomposition.

Geographic aggregation by state and city for success scoring.

# 📈 Analysis & Findings
## ✅ Success Metrics Summary

Average review count ≈ 55.98; median 15; min 5; max 248.

Average star rating ≈ 3.48; median 3.5; min 1.0; max 5.0.

Highest ratings often from small venues at 5.0; highest counts from large chains with slightly lower ratings.

Review count tracks engagement volume more than satisfaction alone.

# ⭐ Engagement vs Rating

Engagement (reviews, check-ins, tips) rises from 1→4 stars.

Slight drop at 5 stars suggests saturation or a niche, highly satisfied audience.

# 🔗 Correlation Among Engagement Types

Reviews, tips, and check-ins are positively correlated, indicating cross-channel spillovers.

Boosting one engagement type can elevate the others.

# 🔼 High vs Low Rated Engagement

High-rated: review_count ≈ 63.10, checkin_count ≈ 80.72, tip_count ≈ 8.07.

Low-rated: review_count ≈ 37.15, checkin_count ≈ 64.84, tip_count ≈ 5.46.

Higher ratings align with higher engagement across metrics.

# 🌍 Geography (States & Cities)

Philadelphia leads success scores, followed by Tampa, Indianapolis, and Tucson.

These cities show strong engagement ecosystems for restaurants.

# ⏱️ Temporal Patterns

High-rated restaurants (≥ 3.5) show steady/growing engagement from 2017–2022.

COVID-era dip in tips; review engagement rebounds after 2020.

# 📅 Trend & Seasonality

Reviews: upward trend with strong seasonality; peak engagement Nov–Mar.

Tips: slight downward trend with seasonal components.

# 😊 Sentiment Proxies (useful, funny, cool)

Positive associations among review_count, useful, funny, cool, and a composite success_score.

Indicative pairwise correlations: useful–review ~0.80, funny–review ~0.64, cool–review ~0.65.

# 🏅 Elite vs Non-Elite Users

Elite users are few but contribute a substantial share of reviews.

Building relationships with elite users can increase loyalty and repeat visits.

# 🕘 Busiest Hours

Peak engagement 4 PM–1 AM → guides staffing and promotions (consider late-night offerings).

# 💡 Recommendations

Elevate service quality to sustain higher ratings and engagement.

Encourage cross-channel engagement to leverage positive correlations.

Collaborate with Yelp elite users for advocacy and reach.

Align operations/promos with 4 PM–1 AM peak.

Expand/invest in top cities (Philadelphia, Tampa, Indianapolis, Tucson).

For lagging venues, focus on feedback loops and sentiment monitoring.

# 🙌 Acknowledgements

Yelp Open Dataset
