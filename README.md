# Uber-Trip-Analysis-dashboard
This Power BI project analyzes Uber trip data collected over a defined period to generate business insights into booking patterns, trip values, vehicle usage, and location trends. The dashboard leverages Power BI’s interactive visualizations and advanced DAX measures to surface actionable metrics for stakeholders in the ride-sharing domain.
Dataset & Metrics
Booking Data: Includes over 104,000 Uber trips, capturing booking value, trip distance, trip time, payment method, vehicle type, pickup, and drop-off locations.

Key KPIs:

Total Bookings: 104K

Total Booking Value: $1.6M

Average Booking Value: $15

Total Trip Distance: 349K miles

Average Trip Distance: 3 miles

Average Trip Time: 16 min.

Dashboard Visuals
Booking Patterns by Time:

Time-series and heatmap visuals show booking volume by hour and by day, helping identify periods of peak demand (notably weekends and late afternoons).

DAX queries aggregate bookings by hour and weekday for advanced trend spotting.

Daywise & Payment Analysis:

Line and pie charts compare total bookings across days of the week and payment methods (Uber Pay, Cash, Amazon Pay, Google Pay), highlighting cashless preference and weekend surges.

Calculations use DAX functions like SUM, COUNTROWS, FILTER to segment bookings.

Vehicle Type Analysis:

Bar charts break down booking counts, total value, and trip distance by vehicle category (UberXL, UberX, Green, Comfort, Black).

UberX leads in preference with 39K bookings.

DAX was used to calculate averages and sums by vehicle type.

Location Insights:

Frequent pickup and drop-off points, including Penn Station/Madison Sq West (pickup) and Upper East Side North (drop-off), are highlighted using DAX measures and location-based visualizations.

The dashboard also notes the farthest recorded trip (Lower East Side to Crown Heights North, 144.1 miles).

DAX Queries Used
Average and Total Calculations:

Example: Avg Booking Value = DIVIDE([Total Booking Value],[Total Bookings])

Conditional Segmentation:

Example: Booking counts filtered by day/night with DAX: CALCULATE([Total Bookings], [TripType]="Night Trip")

Time-Based Aggregation:

Example: Bookings by hour using SUMMARIZE, GROUPBY, and COUNTROWS.

Key Insights
Weekends (Saturday, Sunday) and late afternoons are peak hours for Uber demand.

UberX is the preferred choice among vehicle types.

Majority of users opt for online payments over cash.

Specific urban locations consistently top both pickup and drop-off volumes, aiding operational planning.
