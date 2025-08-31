📊 Amazon Review Sentiment Analyzer (n8n + AI + Google Sheets)

🚀 Project Overview

This project automates the process of collecting Amazon product reviews, analyzing their sentiment using AI, storing results in Google Sheets, and sending daily summary reports via email.

Built with n8n + OpenRouter AI + Google Sheets + Gmail API, it runs daily at 8 AM and provides a clear overview of customer sentiment trends.


---

⚡ Workflow Features

⏰ Daily Automation → Runs every morning at 8 AM (via Cron trigger)

🌐 Amazon Review Scraper → Fetches reviews directly from Amazon product pages

🤖 AI Sentiment Analysis → Classifies reviews as Positive, Negative, or Neutral with confidence score

📊 Google Sheets Dashboard → Logs reviews + sentiment data for tracking over time

📧 Email Summary Report → Sends a daily summary of review sentiment to your inbox



---

🛠️ Tech Stack / Nodes Used

Schedule Trigger → Runs workflow daily

HTTP Request → Fetches Amazon product reviews (HTML)

Code Node (JavaScript) → Extracts and cleans reviews from raw HTML

OpenRouter LLM → Analyzes review sentiment (Positive / Negative / Neutral)

Parse Sentiment Node → Parses AI output into structured JSON

Google Sheets Node → Appends results to dashboard

Prepare Email Summary → Generates daily report text

Gmail Node → Sends daily email



---

📂 Repository Contents

/AI_Review_Sentiment_Workflow
 ├── workflow.json         # n8n workflow export (importable into n8n)
 ├── README.md             # Project documentation
 ├── /docs
 │    ├── workflow.png     # Screenshot of workflow (add after exporting)
 │    └── sample-email.png # Example of email summary


---

📹 Demo Video
🔑 How to Run Locally

1. Clone the repo

git clone https://github.com/Ayokanmii/Analyze-Sentiment

2. Import workflow.json into your n8n instance (via Import Workflow).


3. Set up the required credentials:

OpenRouter API Key (for AI sentiment analysis)

Google Sheets API (for logging reviews)

Gmail OAuth2 (for email summary delivery)



4. Save & activate the workflow.




---

📌 Example Output (Daily Email)

Dear ShopWise Team,

Here is the daily sentiment analysis for product reviews:

Review 1: Great product, works perfectly... (positive, Confidence: 0.92)
Review 2: Stopped working after 2 weeks... (negative, Confidence: 0.89)

View full details: [Google Sheets Dashboard Link]

Best regards,  
ShopWise Analytics


---

👤 Author

Olatunji Ayokanmi Damilola – Developer
