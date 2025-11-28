# 🔥 Final Summary & Visual Report

This section summarizes the insights extracted from trading behavior compared with the Bitcoin Market Sentiment (Fear & Greed Index).  
All supporting visualizations are included below.

---

# 📊 1. Trade Distribution Across Sentiments

### *How different sentiment days impact trade activity*  
✔ Shows whether Fear / Greed leads to heavier or lighter trading volume.

![Total Trades by Sentiment](outputs/total_trades_by_sentiment.png)

---

# 💰 2. PnL Distributions by Sentiment

### *How profit/loss distribution shifts in Fear vs Greed days*

![PnL Distribution by Sentiment](outputs/pnl_distribution_boxplot.png)

(*If you used a different filename, update accordingly*)

---

# 🔥 3. Heatmaps: Win Rate & Avg PnL

### Win Rate Heatmap  
Shows which leverage buckets perform well under different sentiment states.

![Win Rate Heatmap](outputs/winrate_heatmap.png)

### Average PnL Heatmap  
Shows which trade Sides and Sentiments combine for best/worst outcomes.

![Avg PnL by Side × Sentiment](outputs/avgpnl_side_sentiment_heatmap.png)

---

# 📈 4. Daily Sentiment vs Daily Mean PnL

### *Sentiment correlates weakly with raw PnL, but patterns emerge around volatility periods.*

![Daily PnL vs Sentiment](outputs/daily_pnl_vs_sentiment.png)

---

# 📉 5. Scatterplot: Leverage vs PnL (Colored by Sentiment)

### *High leverage amplifies outcomes, especially during Greed/Fear regimes.*

![Leverage vs PnL scatter](outputs/leverage_vs_pnl_scatter.png)

---

# 📆 6. Event Study (Extreme Sentiment 5% Days)

## Extreme Greed (+/- 3 days window)

![Extreme Greed Window](outputs/extreme_greed_window.png)

## Extreme Fear (+/- 3 days window)

![Extreme Fear Window](outputs/extreme_fear_window.png)

---

# 🤖 7. ML Model Feature Importances

### *Even though sentiment isn’t a strong standalone predictor, leverage & size carry predictive signal.*

![Random Forest Feature Importances](outputs/rf_feature_importances.png)

---

# 🧠 Key Insights

### 1. **Sentiment ≠ PnL Predictor (Linear)**  
Correlation is near zero. But patterns show up at extremes.

### 2. **Leverage Dominates Risk Behavior**  
High leverage magnifies losses especially during Greed or Fear spikes.

### 3. **Top Traders Reduce Leverage on Extreme Days**  
Bottom traders do the opposite (strong psychological signal).

### 4. **Event Windows Show Predictable Volatility**  
Both greed and fear extremes cause volatility shifts in the following 1–2 days.

### 5. **ML Models Prefer Structural Features**  
- Leverage  
- Position size  
- Trade side  
matter WAY more than sentiment score.

---

# 📁 Output Directory Summary

All charts are saved in:

./outputs/

These are ready to be included in:
- GitHub repo  
- ds_report.pdf  
- Assignment submission  

---

# 🎯 Final Verdict

While sentiment alone does not predict profitability,  
**its interaction with leverage and trader behavior reveals powerful hidden patterns**—  
especially around extreme sentiment events.

This supports building **event-driven risk controls** and **behavior-based segmentation**,  
rather than sentiment-based predictive models.

