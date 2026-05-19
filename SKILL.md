---
name: web-data-collector
description: A skill for collecting and organizing data from public websites. Supports scheduled scraping, data cleaning, and export to CSV/JSON/Notion/Sheets.
version: 1.0.0
author: chijiao
tags: [web-scraping, data-collection, automation, csv, json]
---

# Web Data Collector

Automatically collect and organize data from any public website. Schedule scraping jobs, clean raw data, and export results to your preferred format.

## What This Skill Does

- Scrapes structured data from public web pages
- Cleans and deduplicates results automatically
- Exports to CSV, JSON, Notion database, or Google Sheets
- Supports scheduled runs (hourly, daily, weekly)
- Handles pagination and infinite scroll pages

## Usage

```
Use this skill when the user wants to:
- Collect product prices, job listings, news articles, or any tabular data from websites
- Monitor a webpage for changes over time
- Export web data into a spreadsheet or database
- Automate repetitive copy-paste data gathering tasks
```

## Example Prompts

- "Scrape all job listings from this URL and save to CSV"
- "Monitor this product page and alert me when the price drops"
- "Collect all articles from this blog and export to Notion"
- "Check this page every day and save new entries"

## Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| url | string | Target URL to scrape |
| selector | string | CSS selector for target elements (optional) |
| schedule | string | Cron expression for scheduled runs (optional) |
| output | string | Output format: csv / json / notion / sheets |

## Notes

- Only works on publicly accessible pages (no login required)
- Respects robots.txt and rate limits
- For authenticated pages, use the browser automation skill instead
