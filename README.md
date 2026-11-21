# adumimweather-now

What the Israel Meteorological Service's station in Ma'ale Adumim (station
218) measured over the last 50 hours, at 10-minute steps, for the first
screen of https://adumimweather.co.il. Updated within minutes of each new
reading. This repository is rewritten at every update (one commit).

**Source: the Israel Meteorological Service (https://ims.gov.il), raw station
data. The IMS is not responsible for this data as shown here.**
נתוני תחנה גולמיים באדיבות השירות המטאורולוגי הישראלי. השירות אינו אחראי
לנתונים כפי שהם מוצגים כאן.

`now.json`: `first_utc` and `last_utc` (UTC), `step_min` (10), and one array
per field from `first_utc` on, `null` where the station sent nothing valid:
`td` air temperature (C, the reading), `td_max` / `td_min` (C, the highest and
lowest in the 10 minutes), `rh` relative humidity (%), `ws_kmh` mean wind
(km/h), `wd` wind direction (degrees), `rain_mm` (mm in the 10 minutes).
