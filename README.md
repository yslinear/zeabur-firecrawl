# FireCrawl - Distributed Web Crawling System

A powerful API service that takes URLs, crawls them, and converts them into clean markdown or structured data. FireCrawl crawls all accessible subpages and provides clean data for each, with no sitemap required.

## Features

- **Scraping**: Get content in LLM-ready format (markdown, structured data, screenshot, html)
- **Crawling**: Extract content from all URLs of a web page in LLM-ready format
- **Mapping**: Input a website and get all website URLs with high performance
- **Extraction**: Get structured data from single page, multiple pages or entire websites with AI

## Services

This template deploys the following services:

### Playwright Service

- Handles web scraping and browser automation
- Supports proxy configuration
- Can block media content for faster scraping

### API Service

- Main API endpoint handling requests
- Manages job queues and processing
- Integrates with Redis for caching and rate limiting

### Worker Service

- Processes background jobs
- Handles queue tasks
- Manages crawling operations

### Redis

- Handles caching and rate limiting
- Manages job queues
- Provides data persistence

## Environment Variables

The following environment variables can be configured:

```bash
# Required
OPENAI_API_KEY=                        # OpenAI API key for AI processing
MODEL_NAME=                            # The AI model name to use
PUBLIC_DOMAIN=                         # Domain for your FireCrawl API

# Optional
OPENAI_BASE_URL=                       # Custom OpenAI API base URL
SUPABASE_URL=                         # Supabase project URL
SUPABASE_ANON_TOKEN=                  # Supabase anonymous token
SUPABASE_SERVICE_TOKEN=               # Supabase service role token
PROXY_SERVER=                         # Proxy server for Playwright service
PROXY_USERNAME=                       # Proxy server username
PROXY_PASSWORD=                       # Proxy server password
BLOCK_MEDIA=true                      # Block media content for faster scraping
SLACK_WEBHOOK_URL=                    # Slack webhook URL for notifications
LLAMAPARSE_API_KEY=                   # LlamaParse API key
SCRAPING_BEE_API_KEY=                 # ScrapingBee API key
SERPER_API_KEY=                       # Serper API key
SEARCHAPI_API_KEY=                    # SearchAPI API key
LOGGING_LEVEL=                        # Logging level
BULL_AUTH_KEY=                        # Bull queue authentication key
POSTHOG_API_KEY=                      # PostHog API key
POSTHOG_HOST=                         # PostHog host
SELF_HOSTED_WEBHOOK_URL=              # Self-hosted webhook URL
```

## Getting Started

1. Deploy this template on Zeabur
2. Configure the required environment variables
3. Access your API endpoint and start crawling

For more detailed documentation, visit [FireCrawl Documentation](https://docs.firecrawl.dev)
