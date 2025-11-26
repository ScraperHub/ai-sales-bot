# AI Sales Bot with Crawlbase Web MCP 🚀

This repository shows how to build a simple **AI-powered sales lead generation bot** using Crawlbase Web MCP and Claude Desktop. The bot crawls websites, extracts business data, and outputs it as a structured CSV — ready for outreach or CRM import.

---

## How to Set Up the AI Sales Bot

Follow these steps to set it up from scratch.

### Step 1: Install and Configure Crawlbase Web MCP on Claude Desktop

Start by setting up [Crawlbase Web MCP Server](https://crawlbase.com/mcp) so Claude can access the web:

1. Open Claude Desktop and go to `File → Settings → Developer → Edit Config`.
2. Save the [short script for Claude](https://github.com/crawlbase/crawlbase-mcp) in `claude_desktop_config.json`.
3. Replace `your_token_here` and `your_js_token_here` with the tokens from your [Crawlbase account dashboard](https://crawlbase.com/dashboard/account/docs).
4. Save your settings and restart Claude Desktop.

> Once done, Claude has web access through Crawlbase — giving it a clean, powerful crawler for structured data extraction.

### Step 2: Open Claude Desktop and Enter Your Custom Prompt

Now that everything’s connected, teach Claude what to do. Paste this prompt into Claude Desktop:

```

You are an expert AI Sales Bot that uses Crawlbase Web MCP to extract and organize business leads.
Generate a CSV file of B2B SaaS companies in Singapore that offer CRM or marketing automation.
Steps:

1. Use Crawlbase Web MCP to crawl company websites.
2. Extract: Company Name, Website, Contact Email, LinkedIn, Industry, Description.
3. Return results in CSV format.
   Output headers:
   Company Name, Website, Contact Email, LinkedIn,Industry, Description

```

Hit enter to begin.

![Build AI sales bot screenshot](https://githubusercontent.com/ScraperHub/ai-sales-bot/main/build-ai-sales-bot-1.jpg)

### Step 3: Let Claude Run the Crawlbase Query

After a few moments, Claude compiles the results and displays them as a CSV file inside the chat window.

![Build AI sales bot screenshot](https://githubusercontent.com/ScraperHub/ai-sales-bot/main/build-ai-sales-bot-2.jpg)

You can copy the table directly into Google Sheets or Excel. It’s already structured and ready for filtering, sorting, or importing into your CRM.

![Build AI sales bot screenshot](https://githubusercontent.com/ScraperHub/ai-sales-bot/main/build-ai-sales-bot-3.jpg)

---

## Summary

Now you have a fully working **AI Sales Bot** that scrapes, cleans, and exports leads automatically. Claude handles reasoning and formatting, while Crawlbase Web MCP does the crawling and data collection.

> Result: high-quality, up-to-date business leads without writing a single line of code.

---

## References

- [Crawlbase Web MCP](https://crawlbase.com/mcp)  
- [Crawlbase MCP GitHub Script](https://github.com/crawlbase/crawlbase-mcp)  
- [Crawlbase Account Dashboard](https://crawlbase.com/dashboard/account/docs)  
```

---

