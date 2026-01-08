# Daily Business News (Fixed XML) – n8n Workflow

This n8n workflow fetches the latest business news from the Economic Times RSS feed, filters news from the last 24 hours, and generates a daily report.

## Features

- **Automated Trigger:** Runs every day at 9:00 AM.
- **RSS Fetch:** Retrieves news from [Economic Times RSS](https://economictimes.indiatimes.com/rssfeedsdefault.cms).
- **XML Parsing:** Parses the RSS XML feed.
- **News Extraction:** Extracts news items with title, link, and publication date.
- **Filtering:** Only includes news from the last 24 hours.
- **Report Generation:** Compiles a formatted daily news report.

## Workflow Steps

1. **Daily Trigger:** Starts the workflow every day at 9:00 AM.
2. **Fetch RSS:** Downloads the RSS feed as a string.
3. **Parse XML:** Converts the RSS XML into JSON.
4. **Extract News Items:** Maps and extracts relevant news fields.
5. **Filter Last 24 Hours:** Keeps only news published in the last 24 hours.
6. **Generate Report:** Formats the filtered news into a readable report.

## Example Output

```
📊 Daily Business News Report
📅 Wed Jan 08 2026

1. News Headline 1
Link: https://...

2. News Headline 2
Link: https://...

...
```

## Usage

1. **Import** this workflow into your n8n instance.
2. **Activate** the workflow.
3. The workflow will run automatically every day at 9:00 AM and generate a daily business news report.

---

**Note:**  
You can customize the trigger time or RSS feed URL as needed.
