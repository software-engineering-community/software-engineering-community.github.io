---
title: SECO Website
---

This is the SECO (Software Engineering Community) Website repository. Content
from this repository is published to https://seco.rocks/ automatically.

# add a manual event

Add a line with `"status": "upcoming"` to
[addevents.json](addevents.json).

Fields are:

|||
|----|----|
|`status`| `upcoming` or `past` |
| `local_date` | ISO date like `2023-04-25` |
| `local_time` | 24h time (local CET/CEST) like `12:00` |
| `link` | link to the event website |
| `name` | name of the event |

full example:

```
{"status": "upcoming", "local_date": "2023-04-25", "local_time": "12:00", "link": "https://www.devday.de/", "name": "Dev Day 2023"}
``` 

Make sure that the file contains a valid JSON array.

python3 -m json.tool < addevents.json

must not fail.
