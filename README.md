# ASA_DataFest_Duke_2025
https://dukestatsci.github.io/datafest/

ASA DataFest Duke 2025: Analyzing Pandemic-Driven Shifts in Savills’ Client Leasing Behavior
By Arth Vijaywargia

Framing the Problem: How COVID Reshaped Leasing Behavior: Savills, a global real estate firm, sought to understand how COVID-19 altered client leasing patterns across key industries and major U.S. markets. Our core question: Did leasing slow during the pandemic, and how did industries adapt their geographic footprint in response to remote work, economic shifts, and urban access?
We analyzed leasing, occupancy, unemployment, and walkability data across 10 major markets: Austin, Chicago, Dallas/Ft Worth, Houston, Los Angeles, Manhattan, Philadelphia, San Francisco, South Bay/San Jose, and Washington D.C. We focused on Technology/Media/Advertising, Financial Services, and Legal Services—Savills’ highest-value client sectors.
Methods & Cleaning - Market Mapping: We consolidated submarkets (e.g., “Chicago Suburbs” → Chicago) using dplyr::case_when() and filtered out non-core areas. Timeline Standardization: Data was split into pre-pandemic (before 2020 Q1), pandemic (2020 Q1–2023 Q1), and post-pandemic (2023 Q2+). Cleaning: Removed rows with missing data, flagged outliers (<500 SF or >1M SF), and standardized industry labels.
Key Questions & Insights: 1. Did Leasing Slow Down? Line charts showed a sharp drop in leased square footage (SF) and occupancy in 2020 Q2. Tech rebounded post-2021 Q1, aligning with vaccine rollouts. However, occupancy lagged—highlighting hybrid work’s impact and “phantom demand.” 2. Did Geography Shift? Heatmaps and walkability scatterplots revealed: Tech’s presence decentralized from San Francisco/South Bay to Dallas and Manhattan. Manhattan retained dominance due to high walkability (score: 89) and transit (score: 84). Philadelphia emerged as a post-pandemic finance hub. Walkability proved a resilience factor—markets like D.C. and Manhattan maintained leasing strength despite remote trends. 3. Did This Affect Unemployment? We found a positive correlation: Markets with greater SF declines (e.g., South Bay: -24%) had smaller unemployment spikes, likely due to remote adaptability. Houston was an outlier—SF down, unemployment up—suggesting sector-specific strain (energy). Walkable cities absorbed shocks better than car-dependent ones.
What This Means for Savills: Hybrid is Here to Stay: Companies lease space strategically, prioritizing transit and talent access. Tech’s Two-Track Approach: Cost-efficient hubs (Austin) coexist with prestige locations (Manhattan). Walkability Matters: High-walkability markets are more resilient—an important client advisory angle. Unemployment ≠ Leasing Collapse: SF decline can reflect remote work, not economic weakness.


Next Steps: Focus on emerging hybrid hubs: Chicago, Philly, D.C., San Francisco. Promote flexible space strategies for legal/finance clients. Use EPA walkability data to guide investment strategies. Track tech’s leasing surges tied to innovation (e.g., AI, biotech).


Limitations & Future Work: Missing data: Lease terms and subleasing activity were unavailable but essential. Granularity: Neighborhood-level walkability could improve precision. Sector dives: Explore legal stability and tech’s space use (offices vs. labs).

Bottom Line: Leasing isn’t dying—it’s evolving. With the right data, Savills can lead clients into the next era of strategic space planning.
