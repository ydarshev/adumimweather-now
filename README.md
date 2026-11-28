# adumimweather-now, branch `warnings`

The Israel Meteorological Service's weather warnings that name the area of
Ma'ale Adumim (the IMS regions "הרי המרכז", "מדבר יהודה", Jerusalem, or the
whole country) and are in force, for the strip on https://adumimweather.co.il.
Read from the IMS's warnings feed every 10 minutes; the IMS's own words,
verbatim. This branch is rewritten at every change (one commit). The branch
`main` holds the station's readings (now.json).

**Source: the Israel Meteorological Service (https://ims.gov.il/he/IMSWarnings).
The IMS is not responsible for this data as shown here.**
אזהרות מזג האוויר באדיבות השירות המטאורולוגי הישראלי, כלשונן. השירות אינו
אחראי לנתונים כפי שהם מוצגים כאן.

`warnings.json`: `items`, the strongest colour first, each with `kind`,
`color` (`yellow` / `orange` / `red`, or `null`), `text` (the IMS's
description), `title`, `issued_utc`, `from_utc` (or `null`) and `to_utc`
(the end of its validity; for an item whose hours could not be read, 12 hours
after its issue, with `hours_read` false). An empty list: no warning for the
area now.
