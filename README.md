# Twitter (X.com) Email Scraper

Extract verified business emails from Twitter/X profiles at scale.

## [Open the Actor on Apify](https://console.apify.com/actors/mSaHt2tt3Z7Fcwf0o/source)

This actor is designed for teams that need fast, reliable **Twitter email scraping** for lead generation, B2B outreach, and market research.

## Why this Twitter email scraper

- No login flow in input
- No user-side cookies required
- No external API keys required from end users
- Built for high-volume runs (up to 1,000,000 results per run)
- Clean output for CRM and outreach workflows

## Pricing

- **$2 per 1,000 results**
- Plus Apify platform usage

## What you can extract

- Verified email (when available)
- Name
- Screen name / username
- Followers count
- Profile metadata used for enrichment workflows

## Input schema

| Field | Type | Required | Description | Example |
|---|---|---|---|---|
| `usernames` | `string` | Yes | Usernames separated by new lines | `elonmusk\nnaval` |
| `max_results` | `number` | No | Maximum results to return | `10000` |

### Example input

```json
{
  "usernames": "elonmusk\nnaval\nlexfridman",
  "max_results": 10000
}
```

## Output example

```json
[
  {
    "email": "example@company.com",
    "name": "Example Name",
    "screenname": "example",
    "followers": 123456,
    "created_at": "2011-01-01T00:00:00Z"
  }
]
```

## Best use cases

### 1. B2B lead generation
Build targeted lead lists from niche Twitter/X audiences.

### 2. Sales prospecting
Enrich username lists with email-ready contact data.

### 3. Influencer and creator research
Find reachable profiles for partnerships and campaigns.

### 4. Market intelligence
Collect contactable profiles around vertical-specific accounts.

## Notes

- `max_results` controls output cap.
- Usernames should be newline-separated.
- If an email is not found for a profile, that profile may be skipped depending on actor logic.

## Related actor (followers/following)

Need usernames or user IDs at scale first?

- [Twitter (X) Follower Scraper — $0.10 / 1K](https://console.apify.com/actors/bIYXeMcKISYGnHhBG/source)

## FAQ

### Is this an official Twitter API?
No. This is an Apify actor for practical scraping workflows.

### Do I need to configure cookies or tokens?
No input-side cookie setup is required.

### Can I run large jobs?
Yes, up to 1,000,000 results per run (plan and data availability dependent).

## SEO keywords

twitter email scraper, x email scraper, twitter x.com email scraper, scrape emails from twitter profiles, twitter lead generation scraper, twitter b2b email finder, no login twitter scraper, twitter contact scraper, twitter outreach data

---

## Start now

### [Run Twitter (X.com) Email Scraper on Apify](https://console.apify.com/actors/mSaHt2tt3Z7Fcwf0o/source)
