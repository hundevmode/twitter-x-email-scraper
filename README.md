# twitter-x-email-scraper
Extract verified emails from Twitter profiles — ultra-fast, no login or API keys required. Perfect for lead generation, B2B outreach, and marketing lists.  ⚡ Fast and reliable 📧 Verified business emails only 🧠 Works without login or auth 📈 Up to 1,000,000 results per run 💰 $2 per 1,000 results

# 🐦 Twitter (X.com) Email Scraper

Effortlessly extract enriched profile data from Twitter (X.com) by providing a list of usernames. No cookies, tokens, or authentication needed — simply paste the usernames and get structured results.

Afipy - [Link](https://console.apify.com/actors/mSaHt2tt3Z7Fcwf0o/input)

---

## ✨ Features

- ✅ **No Login Required**: Just provide Twitter handles — no need for API keys or session cookies.
- ⚡ **Fast & Scalable**: Built to process hundreds of thousands of usernames quickly.
- 🎯 **Targeted Output**: Limit your results by specifying how many user profiles to return.
- 🧠 **Smart Handling**: Automatically skips empty lines or duplicates in your username input.

---

## 🛠️ How It Works

1. 📝 **Paste Usernames**: Enter one Twitter handle per line.
2. 🔢 **Set Limit (optional)**: Choose how many profiles to retrieve — from a few to a million.
3. 🚀 **Run the Actor**: Scraper connects to a structured database, queries user records, and returns them in bulk.

---

## 🧾 Input Format

| Field         | Type     | Required | Description                                                     |
|---------------|----------|----------|-----------------------------------------------------------------|
| `usernames`   | string   | ✅       | Twitter handles separated by new lines                          |
| `max_results` | integer  | ❌       | Optional max number of results to return (min: 500, max: 1,000,000) |

Example input (Manual mode):

```json
[
  {
    "email": "elon@tesla.com",
    "name": "Elon Musk",
    "screenname": "elonmusk",
    "followers": 182000000,
    "created_at": "2009-06-02T20:12:29Z"
  },
  {
    "email": "naval@angellist.com",
    "name": "Naval",
    "screenname": "naval",
    "followers": 2000000,
    "created_at": "2007-11-19T23:06:00Z"
  }
]
```

⚙️ Use Cases
• 💼 Lead generation based on Twitter presence  
• 🧠 Competitive analysis & influencer tracking  
• 📣 Building outreach or email marketing lists

⸻

📌 Notes  
• Output is capped to the number set in `max_results`. If you input 200,000 usernames but set `max_results` to 50,000 — only the first 50,000 matches will be returned.  
• Supports **newlines** as separators, **not commas**.  
• `max_results` must be **at least 500** and no more than **1,000,000**.

⸻

Start collecting enriched Twitter profile data with just a few clicks — no coding required!
