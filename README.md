# 🏒 Fantasy Hockey – Playoff Probability Simulation

This project uses Monte Carlo simulation and probability modeling to evaluate whether Ryan should continue competing for playoffs or trade players in a fantasy hockey keeper league.

Objective:  
Estimate end-of-season point totals and compute probability of making playoffs under multiple scenarios.

---

## 📊 Problem Context

Ryan is 12 matchups into a 20-matchup season.

- Current total: 104 points
- 8 teams qualify for playoffs
- 8 matchups remaining (13–20)
- Trade deadline: After matchup 17

Decision:
- Continue competing for playoffs
- Or trade top players for future draft picks

---

## 🔢 Simulation Approach

Two simulation methods were used:

### 1️⃣ Historical Resampling (Bootstrap)

- Randomly sampled from past weekly points (with replacement)
- Simulated 10,000 season outcomes

**Average Final Points:** 197  
- 10th percentile: 182  
- 90th percentile: 213  

---

### 2️⃣ Normal Distribution Simulation

- Fitted normal distribution using historical mean and standard deviation
- Generated future matchup points probabilistically

**Average Final Points:** ~197.7  

Pros:
- Captures variability and trend  
Cons:
- Assumes normality

---

## 🎯 Playoff Probability Estimation

Using historical 8th-place thresholds:

### Based on 2016–17 Season
- Probability of making playoffs: **~70%**

### Based on 2017–18 Season
- Probability of making playoffs: **~84.7%**

---

## 📈 Sensitivity Analysis

### Competitive Threshold Scenarios

| 8th Place Threshold | Probability Ryan Qualifies |
|----------------------|----------------------------|
| 162 points           | 99%+                       |
| 170 points           | 99%                        |
| 190 points           | ~70–85%                    |
| 198 points           | ~50%                       |

---

### Weighted Recent Performance

Using 1:3 weighting (2016–17 : 2017–18):

- Projected Final Points: ~195

---

## 💡 Strategic Insights

- Expected final total ≈ 197 points.
- If 8th-place cutoff ≈ 190 → Ryan is likely to qualify.
- If cutoff rises to ~198 → Qualification becomes uncertain (~50%).

---

## 🧠 Trade Deadline Strategy

By matchup 16:

- ≥ 160 points → ~97% playoff probability  
- ~152 points → ~88% playoff probability  

Recommendation:
Wait until matchup 16 before making trade decisions.

If performance tracks near expected value → Compete.  
If performance falls significantly short → Consider trading.

---

## 🛠 Techniques Used

- Monte Carlo Simulation  
- Bootstrap Resampling  
- Probability Distribution Modeling  
- Scenario Analysis  
- Sensitivity Testing  

---

## 🎯 Skills Demonstrated

- Predictive simulation modeling  
- Probabilistic decision-making  
- Risk quantification  
- Scenario-based strategic analysis  
- Data-driven tradeoff evaluation  

---

This project demonstrates how simulation and probability modeling can support strategic decision-making under uncertainty.
