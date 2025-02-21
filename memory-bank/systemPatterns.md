# System Patterns

## Core Architecture
```mermaid
sequenceDiagram
    User->>Scraper: Execute scraping job
    Scraper->>Note.com: HTTP Request
    Note.com-->>Scraper: HTML Response
    Scraper->>Parser: Extract structured data
    Parser->>Output: Save results (JSON/CSV)
```

## Key Components
1. Request Manager - Handles HTTP operations
2. Header Rotation - Manages User-Agent rotation
3. DOM Parser - Extracts structured data
4. Error Handler - Manages retries/exceptions

## Data Flow
1. URL Queue -> Request Manager
2. Raw HTML -> Parser
3. Structured Data -> Output Module
4. Errors -> Monitoring System
