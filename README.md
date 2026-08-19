## 📊 Business Problem Diagnostics & SQL Results

### 1. Payment Channel Risk Analysis
* **Core Insight:** COD orders exhibit a 9.68% return rate, driving higher relative reverse freight losses.

![Payment Channel Output](Screenshot%202026-08-19%20160309.png)

---

### 2. Category Defect Concentration (Window Function: `DENSE_RANK`)
* **Core Insight:** Hair Growth Actives Serum (7 returns) and Oat Extract Gentle Cleanser (6 returns) ranked #1 in returns across respective lines.

![Product Ranking Output](Screenshot%202026-08-19%20160434.png)

---

### 3. Geographic High-Risk Delivery Clusters
* **Core Insight:** West Bengal (12.77%), Delhi (8.89%), and Madhya Pradesh (8.44%) flagged into the highest delivery risk tiers.

![Geographic Risk Output](Screenshot%202026-08-19%20160528.png)

---

### 4. Root-Cause Defect Decomposition
* **Core Insight:** Skin irritation accounts for >40% of returns in Cleansers and 33% in Body Care.

![Root Cause Output](Screenshot%202026-08-19%20160621.png)

---

### 5. Chronic Returner Segmentation (CTE Pipeline)
* **Core Insight:** Isolated 10 repeat returners placing an average of 4.30 orders per user.

![Customer Segmentation Output](Screenshot%202026-08-19%20160703.png)
