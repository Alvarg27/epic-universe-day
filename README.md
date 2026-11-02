# Park day planner

A phone-first planner for Universal Epic Universe, Magic Kingdom and Disney's Hollywood Studios: live waits, rain now and forecast, a re-planning ride order, real walking distances, and an optional location button. Open: https://alvarg27.github.io/epic-universe-day/

## Where the numbers come from

- **Live waits, ride status (open / down / closed / refurbishment), park hours, showtimes:** ThemeParks.wiki, fetched by the page every minute.
- **Rain now:** weather.gov station observations (Orlando airport for Epic, Kissimmee for the Disney parks). **Forecast:** weather.gov hourly grid (chance, amount, thunder) plus the NBM and ECMWF models via Open-Meteo.
- **Wait predictions:** TouringPlans posted-wait history. Each date is predicted only from the same kind of day: party and special-event nights (Magic Kingdom's Halloween and Christmas parties, Hollywood Studios' Jollywood Nights), read from the park's schedule, are kept apart from normal days. Within that: the most recent week (55%), adjusted per ride by how that weekday usually compares over the last 12 weeks (only when there are 3+ matching days), past days with the same weekday (25%), recent days of the same type (15%), the same weeks last year (5%). Tested on the last 28 days, each predicted without seeing it; the page shows the typical miss for the weekday you're on (about 5–12 min depending on park and day).
- **Walking:** shortest route on the parks' guest footpaths from OpenStreetMap (service roads left out), at about 65 m a minute; checked against 19 known walks. Where a land's paths aren't mapped (Epic's Nintendo area, the Fantasmic! walkway) the walk is estimated from straight-line distance.
- **Fans and dizziness:** our summary of published ride rankings and rider motion-sickness reports.

Map data © OpenStreetMap contributors (ODbL).
