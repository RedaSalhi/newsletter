# The Quant Brief - Weekly Newsletter Automation

A comprehensive automation framework for generating professional quantitative finance newsletters targeting investment professionals.

## Overview

**The Quant Brief** is a 4-6 page professional LaTeX newsletter designed for:
- Portfolio managers
- Risk managers
- Sell-side quants
- Fintech developers
- Institutional investors

## Core Mission

Generate weekly newsletters covering quantitative finance developments, market analysis, academic research, and actionable insights for investment professionals.

## Research Protocol

### Phase 1: Market Data Collection

**MANDATORY:** Only use sources published/updated between `[START_DATE]` and `[END_DATE]`

#### US Markets
- S&P 500, Nasdaq, Dow Jones weekly performance
- VIX levels and volatility patterns
- Sector rotation and leadership changes
- Treasury yield movements (2Y, 10Y, 30Y)
- Options expiration impacts (if applicable)

#### Global Markets
- European indices (DAX, CAC 40, FTSE, STOXX 600)
- Asian markets (Nikkei, Hang Seng, CSI 300, KOSPI)
- Currency movements (DXY, EUR/USD, USD/JPY, GBP/USD)
- Commodities (Gold, Oil, Bitcoin, Agricultural)

#### Credit & Fixed Income
- Corporate spreads (IG, HY)
- Government bond yields globally
- Credit market flows and issuance

### Phase 2: News & Events Analysis

Search for specific developments:
- **Central Bank Actions**
- **Geopolitical Events**
- **Economic Data:**
  - Employment reports, inflation data
  - GDP releases, manufacturing PMI
  - Consumer confidence, retail sales

### Phase 3: Academic Research Curation

Find 2-3 recent papers from approved sources.

#### Sources to Search
- arXiv.org (sections: q-fin.*, cs.LG, stat.ML)
- SSRN.com recent publications
- NBER working papers
- Google Scholar (filter by date)

#### Required Criteria
- **Strict Condition:** Published between `[START_DATE]` and `[END_DATE]`
- **Topics:** Quantitative finance, algorithmic trading, risk management, portfolio optimization, machine learning in finance, market microstructure

#### Analysis Requirements
- Summarize methodology and key findings
- Extract practical implications for investment professionals
- Identify implementation strategies
- Note any significant information or results

### Phase 4: Earnings & Corporate Analysis

#### Major Earnings Reports
- S&P 500 companies reporting during the week
- Focus on: revenue beats/misses, guidance changes, margin trends
- Sector-specific developments
- Management commentary on outlook

#### Corporate Actions
- M&A announcements, spin-offs, special dividends
- Share buyback programs, debt issuance
- Strategic partnerships, major contracts

#### Regulatory Filings
- 10-K, 10-Q filings with material changes
- 8-K current reports for significant events
- Insider trading patterns (Form 4 filings)

## Content Structure

### 1. Executive Summary (200 words)
- Week's dominant theme in one sentence
- 3-4 key market moves with specific numbers
- Major policy/earnings/research developments
- Forward-looking statement about next week's catalysts

### 2. Breaking News & Market Moves
- **US Markets:** Specific index levels, weekly changes, record highs/lows
- **Global Markets:** Regional performance with correlation analysis
- **Cross-Asset:** Currency, commodity, credit market interactions
- **Volume/Flow Analysis:** Unusual trading patterns, ETF flows

### 3. Research Paper Analysis (2-3 papers)
For each paper:
- Authors and Publication Date
- Methodology Summary (mathematical models, data sources)
- Key Findings (quantitative results, statistical significance)
- Practical Applications (implementation for PM/RM/traders)
- Market Relevance (current market conditions alignment)

### 4. Global Earnings & Corporate Disclosures (1-2 companies)
For each company:
- **Financial Metrics:** Revenue, EPS vs. consensus, margins
- **Strategic Developments:** Guidance, CapEx, acquisitions
- **Valuation Analysis:** P/E, PEG, sector comparisons
- **Risk Assessment:** Balance sheet, competitive position
- **Sector Implications:** Broader industry trends

### 5. Market Dashboard
Create table with:
- US Indices: Levels, weekly/monthly/YTD changes
- Volatility Metrics: VIX, MOVE index, currency vol
- Fixed Income: Yield levels, spreads, steepening/flattening
- Alternative Assets: Gold, Bitcoin, commodity indices
- Statistical Significance: Note unusual moves (>2 standard deviations)

### 6. Global Market Outlook
- **Next Week's Calendar:** FOMC meetings, economic releases, earnings
- **Geopolitical Events:** Elections, trade negotiations, summits
- **Technical Analysis:** Support/resistance levels, options expiration
- **Risk Scenarios:** Binary outcomes, tail risks, correlation breakdowns

## Output Specifications

### LaTeX Requirements

```latex
% Use this exact document structure:
\documentclass[11pt,a4paper]{article}
\usepackage[margin=1in]{geometry}
\usepackage{amsmath,amsfonts,amssymb}
\usepackage{booktabs,hyperref,xcolor}
\definecolor{quantblue}{RGB}{0,51,102}
\definecolor{quantgray}{RGB}{64,64,64}
% [Include full preamble from previous example]
```

### Content Guidelines
- **Length:** 4-6 pages when compiled
- **Citations:** Include hyperlinks to all sources
- **Data Tables:** Use professional booktabs formatting
- **Emphasis:** Use `\emphasis{}` for key points, `\metric{}` for numbers
- **Mathematical Notation:** Proper LaTeX formatting for formulas

## Quality Standards

### Accuracy
- All market data must be verified from primary sources
- **Timeliness:** Only include information from the specified week
- **Professional Tone:** Suitable for institutional investment professionals
- **Actionable Insights:** Each section must provide implementable strategies
- **Quantitative Focus:** Emphasize statistical significance, model validation

## Critical Instructions

### Search Strategy
- Use date filters religiously - only `[START_DATE]` to `[END_DATE]`
- Prioritize primary sources: Fed websites, company IR pages, arXiv
- Cross-validate data from multiple sources
- Focus on institutional-grade content over retail/general news

### Research Depth
- **Academic Papers:** Read abstracts, conclusions, and key results tables
- **Earnings Analysis:** Don't just report numbers - analyze implications
- **Market Data:** Include statistical context (historical percentiles, z-scores)
- **Forward-Looking:** Always include next week's catalysts

### Professional Standards
- **No Speculation:** Only report verified information
- **Balanced Analysis:** Include both bullish and bearish perspectives
- **Risk Disclosure:** Note uncertainties and limitations
- **Attribution:** Properly cite all sources with hyperlinks

## Weekly Customization Variables

- **Week Dates:** `[START_DATE]` to `[END_DATE]`
- **Focus Theme:** Adapt based on week's dominant story
- **Calendar Events:** Customize outlook section for upcoming events

