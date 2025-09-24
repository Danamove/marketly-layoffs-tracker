# Tech Layoffs Tracker

A real-time tracker of tech industry layoffs with automatic data updates.

## Features
- Interactive filtering by month, industry, and location
- Live search across all data fields
- Sortable columns
- Responsive design
- Automatic data updates from external sources

## Files
- `index.html` - Main website
- `data.json` - Layoffs data (updated automatically)
- `update_script.js` - Data fetching and update logic

## Data Sources
Since layoffs.fyi doesn't provide an official API, we use:
1. **Manual updates** to `data.json`
2. **Web scraping** (respectfully with rate limiting)
3. **Alternative APIs** like Intellizence or TrueUp.io
4. **News monitoring** for layoff announcements

## Automatic Updates

### Option 1: Manual JSON Updates
Simply edit `data.json` with new layoff entries.

### Option 2: Scheduled Updates
Set up automation using:
- **GitHub Actions** (free, scheduled runs)
- **Node.js cron job** (if you have a server)
- **Cloud functions** (AWS Lambda, Vercel, etc.)

### Option 3: News API Integration
Monitor tech news APIs for layoff keywords and automatically add entries.

## Current Data (2025)
- **96,861** total employees laid off
- **413** companies with layoffs
- Data sourced from press releases, SEC filings, and news reports

## Usage
1. Open `index.html` in a web browser
2. Data loads automatically from `data.json`
3. Use filters and search to explore the data

## Future Enhancements
- Real-time notifications for new layoffs
- Data visualization charts
- Export functionality
- API integration with multiple sources
- Mobile app version