# Pi Fishing GPS

A DIY, offline-first fishing GPS built around a Raspberry Pi 5, for Virginia and the Chesapeake Bay. It shows a depth map, NOAA tidal current arrows and wind, rates the bite from real trip data, and ranks fish species from a photo, all on the device.

[![Demo screenshot of the Pi fishing GPS map with depth bands, current arrows and a wind compass. Demo data, not for navigation.](https://keemwilliams.github.io/pi-fishing-gps/og/home.jpg)](https://keemwilliams.github.io/pi-fishing-gps/)

**Project site: https://keemwilliams.github.io/pi-fishing-gps/**

This repository holds the project page and the README only. The application code is private, so there is nothing to install or run from here. The site documents what I have built, what the data showed and what is still planned.

**Not for navigation.** This is a hobby project. The maps in the screenshots are a made-up demo river. Tide and current numbers are predictions, not measurements.

## Status

| Part | Status |
|---|---|
| Offline map with depth bands, numbers and spots (MapLibre, Svelte) | Built, on demo data |
| Tidal current arrows from NOAA CO-OPS predictions | Built, on demo values |
| Wind compass on the map and wind dial on the Today screen | Built, on demo data |
| Bite score re-weighted from 58,254 coastal Virginia trips | Built |
| Fish identification model, 43 species plus Other, 82.1% top-1 on unseen photos | Trained on a laptop, not on a Pi yet |
| Assistant that answers typed questions from the device's own data | Built. Speech is not installed |
| Raspberry Pi 5 hardware, GPS, sonar, LTE, pressure sensor | Planned. Nothing bought yet |

## Read more

- [Overview and FAQ](https://keemwilliams.github.io/pi-fishing-gps/)
- [Hardware for a Raspberry Pi 5 fishing GPS](https://keemwilliams.github.io/pi-fishing-gps/hardware/)
- [Offline fishing map with depth charts](https://keemwilliams.github.io/pi-fishing-gps/map-and-depth-charts/)
- [Tide and current arrows from NOAA predictions](https://keemwilliams.github.io/pi-fishing-gps/tidal-currents/)
- [Wind on a fishing map](https://keemwilliams.github.io/pi-fishing-gps/wind/)
- [Fishing bite forecast: what 58,254 Virginia trips showed](https://keemwilliams.github.io/pi-fishing-gps/bite-score/)
- [Fish identification on a Raspberry Pi](https://keemwilliams.github.io/pi-fishing-gps/fish-id/)
- [Offline voice assistant for fishing](https://keemwilliams.github.io/pi-fishing-gps/voice-assistant/)
- [Data sources and credits](https://keemwilliams.github.io/pi-fishing-gps/data-sources/)
- [Safety and limits](https://keemwilliams.github.io/pi-fishing-gps/safety/)
- [Roadmap: what is built and what is planned](https://keemwilliams.github.io/pi-fishing-gps/roadmap/)

## One result worth sharing

I tested the usual bite-forecast inputs against 58,254 recorded recreational fishing trips from coastal Virginia (NOAA MRIP). Water temperature was the clearest signal. Moon phase, solunar windows and barometric pressure showed no detectable effect on whether a trip caught a fish. The chart and the method are on the [bite score page](https://keemwilliams.github.io/pi-fishing-gps/bite-score/).

## Credits

NOAA CO-OPS, NDBC, the National Weather Service, NOAA MRIP, USGS, OpenStreetMap contributors, Virginia DWR and VMRC data, iNaturalist observers, MapLibre, Svelte, Skyfield, Meteocons and others. The full list with terms is on the [data sources and credits](https://keemwilliams.github.io/pi-fishing-gps/data-sources/) page. The fish identification model was trained partly on CC BY-NC photos, so it is for non-commercial use only.

Raspberry Pi is a trademark of Raspberry Pi Ltd. This project is not affiliated with or endorsed by Raspberry Pi Ltd, NOAA or any other organisation named here.
