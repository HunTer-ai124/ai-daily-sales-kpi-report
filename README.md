# AI Daily Sales KPI Report (n8n + Gemini)

An automated workflow that turns raw sales data into a daily executive briefing, delivered by email. Works for any company by editing one Settings node.

## What it does
1. Runs every morning on a schedule
2. Reads sales orders from Google Sheets
3. Calculates today vs yesterday KPIs: revenue, orders, average order value, new customers, top product, top and worst region, % change
4. Google Gemini writes a short executive summary with recommendations (prompted never to invent numbers)
5. Builds a formatted HTML report and sends it via Gmail

## Tools
n8n, Google Sheets API, JavaScript, Google Gemini, Gmail API

## Make it work for any company
Edit the **Settings** node: company name, sheet link, column names, currency, recipients. No logic changes needed.

## Reliability
- Automatic retries if the AI service is busy
- The report still sends with the KPI table if the AI fails

## Demo
[Watch the demo video](LINK)

Built during my data analytics training at 10Alytics.
