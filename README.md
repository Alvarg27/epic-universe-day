# Park day planner

A phone-first planner for Universal Epic Universe, Magic Kingdom and Disney's Hollywood Studios: live waits, rain now and forecast, a re-planning ride order, real walking distances, and an optional location button. Open: https://alvarg27.github.io/epic-universe-day/

## Where the numbers come from

- **Live waits, ride status (open / down / closed / refurbishment), park hours, showtimes:** ThemeParks.wiki, fetched by the page every minute.
- **Rain now:** weather.gov station observations (Orlando airport for Epic, Kissimmee for the Disney parks). **Forecast:** weather.gov hourly grid (chance, amount, thunder) plus the NBM and ECMWF models via Open-Meteo.
- **Wait predictions:** TouringPlans posted-wait history (Epic: every day since opening; Disney parks: Oct–Nov 2025 and Jun–Nov 2026), blended per date from the last week, the same weekday, recent weeks of the same day type and the same weeks last year. Backtested over the last 14 days on days the model didn't see: average miss about 10 min at Epic, 6 at Magic Kingdom, 9 at Hollywood Studios.
- **Walking:** shortest route on the parks' guest footpaths from OpenStreetMap (service roads left out), at about 65 m a minute; checked against 19 known walks. Where a land's paths aren't mapped (Epic's Nintendo area, the Fantasmic! walkway) the walk is estimated from straight-line distance.
- **Fans and dizziness:** our summary of published ride rankings and rider motion-sickness reports.

Map data © OpenStreetMap contributors (ODbL).
