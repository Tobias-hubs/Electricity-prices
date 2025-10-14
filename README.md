Implements a Java CLI application that fetches and analyses hourly electricity prices, with optional CSV‑based consumption cost calculation.

## Features
- CLI prompts for Swedish price zone (SE1–SE4).
- Fetches hourly electricity prices from [elprisetjustnu.se](https://elprisetjustnu.se) for today and tomorrow.
- Analyses and displays:
  - Average price
  - Cheapest and most expensive hour
  - Best start times for 2h, 4h, and 8h charging windows
- Lists all hourly prices with SEK, EUR, and exchange rate.
- Uses Java record for the Consumption data model to reduce boilerplate and keep the code concise. 

- **Extra credit:** Optional import of a CSV file (`yyyy-MM-dd HH:mm,kWh`) to calculate total cost based on actual consumption data. To test simply press "j" and write consumption.csv to load. 
- Handles missing or invalid price data gracefully.

## Testing
- Verified functionality with both large datasets and a minimal 7‑row `consumption.csv`.
- Cross‑checked total cost calculations against known price data from the API.
- Confirmed robustness when price data is missing for some dates (skips those hours).

## Issue
Related to #2 
