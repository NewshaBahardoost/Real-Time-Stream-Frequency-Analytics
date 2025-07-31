# ⚡ Real-Time Stream Frequency Analytics

## Overview
This project simulates **real-time data stream processing** to estimate item frequencies under strict memory constraints. The approach is inspired by **Count-Min Sketch algorithms**, which approximate frequency counts efficiently for high-volume data streams.

---

## Business Goal
- Monitor **large-scale user activity** (e.g., ad clicks, page views) in real time.
- Approximate item counts **without storing full data**, reducing memory costs.
- Enable **fast decision-making** in marketing campaigns and online platforms.

---

## Approach
1. Streamed dataset containing **millions of item IDs**.
2. Used **5 hash functions** and a limited-size memory array.
3. Computed approximate frequencies for each unique item.
4. Calculated **relative error** and analyzed accuracy across frequency ranges.

---

## Example Results
- Low-frequency items had higher error (expected behavior).
- High-frequency items (frequent clicks) had **<100% relative error**, providing reliable real-time estimates.

![Relative Error Plot](images/relative_error_plot.png)

---

## Tools Used
- Python, Hash-based algorithms
- Data streaming concepts
- Log-log error analysis

---

## Business Impact
- Enables **real-time monitoring of ads, clicks, and product views**.
- Supports **budget allocation** for online advertising.
- Reduces infrastructure costs by avoiding full data storage while maintaining acceptable accuracy.

---

🔗 **View Notebook:** [Real-Time Frequency Analysis](stream_frequency_analysis.ipynb)
