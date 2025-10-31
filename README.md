# n8n-Campaign-Allocator
AI-powered n8n workflow for automated marketing campaign budget allocation and ROI optimization.
# 🧠 n8n-Campaign-Allocator

AI-powered **n8n workflow** for automated marketing campaign **budget allocation and ROI optimization**.

---

## 🚀 Overview
This project uses **n8n** automation to read campaign performance data from a CSV file, analyze historical ROI by channel, and automatically recommend optimized budget allocations to maximize conversions within given constraints.  

The workflow integrates:
- CSV Upload and Parsing  
- Budget Parameter Setup  
- ROI and Conversion Optimization Logic  
- Google Sheets Output for Recommendations  

---

## 📂 Input Data (CSV Format)
Upload your campaign data via the webhook node using a CSV file with columns like:

| channel | historical_spend | conversions | roi | min_budget | max_budget |
|----------|------------------|--------------|-----|-------------|-------------|
| Google   | 10000            | 50           | 2.5 | 5000        | 15000       |
| Meta     | 5000             | 20           | 1.8 | 2000        | 7000        |
| LinkedIn | 3000             | 10           | 1.2 | 1000        | 5000        |

---

## ⚙️ How It Works
1. **CSV Upload:** User uploads campaign performance data through an n8n webhook.  
2. **Parse CSV:** The workflow reads and validates the data.  
3. **Budget Parameters:** Total budget and constraints are read from workflow inputs.  
4. **Optimization Engine:** Calculates optimal allocations per channel to maximize ROI or conversions.  
5. **Google Sheet Output:** Writes recommended allocations, expected conversions, and ROI scores to a connected Google Sheet.  

---

## 🧮 Output (Google Sheet)
| channel | recommended_budget | expected_conversions | expected_roi | notes |
|----------|--------------------|----------------------|---------------|-------|
| Google   | 12000              | 65                   | 2.8           | Max ROI channel |
| Meta     | 6000               | 28                   | 2.0           | Increased spend |
| LinkedIn | 3000               | 12                   | 1.3           | Within cap |

---

## 🧩 Tech Stack
- **n8n** (no-code workflow automation)  
- **Google Sheets API** for results output  
- **Custom JavaScript nodes** for optimization logic  
- **CSV webhook input** for campaign data ingestion  

---

## 🧠 Use Case
Perfect for marketing analysts and data teams who want:
- Automated performance analysis  
- Data-driven budget optimization  
- Real-time integration with marketing dashboards  

---

## 🪄 Setup Instructions
1. Import the workflow JSON file into n8n.  
2. Update credentials for Google Sheets and webhook.  
3. Upload your campaign CSV file through the webhook endpoint.  
4. Execute the workflow to generate optimized budget recommendations.

---

## 📜 License
This project is released under the **MIT License** — free for personal and commercial use.

---

## 👤 Author
**Vanshita Bansal & Agrim Mehta**  
💡 *Part of the n8n AI-driven Campaign Optimization Series*
