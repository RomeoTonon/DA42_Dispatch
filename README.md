# DA42 Dispatch

Mass & balance, performance and briefing pack for the NewCAG DA42 fleet (F-GUPM, F-GZJX, F-HKAF).

Everything is in one file, `index.html`: the AFM chart data, the airport/runway database (OurAirports), the NewCAG form pages and the Diamond chart images are embedded. No build step and no server code.

## Notes
- **Live METAR** uses `https://aviationweather.gov/api/data/metar`. If the browser blocks the request, the page falls back to the "Open METAR/TAF" link and paste box.
- **Fleet map** embeds ADS-B Exchange (`globe.adsbexchange.com`). If ADS-B Exchange refuses to be shown inside another site, the Flightradar24 / FlightAware / ADS-B Exchange buttons still open each aircraft in a new tab.
- Entries are saved in the browser (localStorage) of each user.
- **Print** the briefing pack from the "Briefing pack" tab (A4, NewCAG pages 1–2 followed by the AFM charts).

## Updating data
Aircraft empty masses and moments are in the `AC` list near the top of the script in `index.html`. Always check the AFM for up-to-date data.

For training and planning only. The pilot in command remains solely responsible for mass, balance and performance.

© 2026 Roméo Tonon
