# FireCrawl - Distributed Web Crawling System

FireCrawl is a powerful API service that takes URLs, crawls them, and converts them into clean markdown or structured data. It crawls all accessible subpages and provides clean data for each, with no sitemap required.

## Features

- **Scraping**: Scrapes URLs and gets content in LLM-ready format (markdown, structured data, screenshot, html)
- **Crawling**: Scrapes all URLs of a web page and returns content in LLM-ready format
- **Mapping**: Input a website and get all website URLs - extremely fast
- **Extraction**: Get structured data from single page, multiple pages or entire websites with AI

## Services

This template deploys the following services:

### 1. Playwright Service

- Handles web scraping and browser automation
- Supports proxy configuration
- Can block media content for faster scraping

### 2. API Service

- Main API endpoint handling requests
- Manages job queues and processing
- Integrates with Redis for caching and rate limiting

### 3. Worker Service

- Processes background jobs
- Handles queue tasks
- Manages crawling operations

### 4. Redis

- Handles caching and rate limiting
- Manages job queues
- Provides data persistence

## Getting Started

1. Deploy this template on Zeabur
2. Configure the required environment variables
3. Access your API endpoint and start crawling!

For more detailed documentation, visit [FireCrawl Documentation](https://docs.firecrawl.dev)

## Issues

For questions and support, please visit the [GitHub Issues](https://github.com/yslinear/zeabur-firecrawl/issues)
