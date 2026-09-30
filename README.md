# Simple Topo

A simple web map for viewing NSW topographic maps and aerial imagery. It works on both desktop and mobile devices.

**Live site:** [six.bushwalkingmaps.com](https://six.bushwalkingmaps.com)

**Simple Topo is not a NSW Government service.** It is not operated, endorsed or supported by DCS Spatial Services, so please don't contact them about it. Simple Topo is run by [al3x.au](https://al3x.au); for questions or problems, email [alex@al3x.au](mailto:alex@al3x.au). For official NSW Government mapping, use [SDT Explorer](https://portal.spatial.nsw.gov.au/explorer/index.html) ([about SDT Explorer](https://www.nsw.gov.au/environment-land-and-water/spatial-data-and-mapping/spatial-digital-twin/explorer)). For official Spatial Services products, datasets and support, visit [spatial.nsw.gov.au](https://www.spatial.nsw.gov.au).

## How it works

The site is plain static files. The browser loads map tiles and runs searches, identify and measurements directly against the public NSW Government ArcGIS web services, so there is no server-side component or proxy.

Features:
- lot, address, suburb, point of interest and survey mark search
- coordinate search and identification, across both GDA94 and GDA2020
- distance and area measurement
- CSV dropper, for bulk loading and viewing lots

## Running locally

Serve the `public` folder with any static web server, for example:

```sh
python3 -m http.server 8080 -d public
```

## Data and licence

Map data and imagery are displayed from NSW Government web services under the [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/) licence:

© State of New South Wales (Spatial Services, a business unit of the Department of Customer Service NSW). For current information go to [spatial.nsw.gov.au](https://www.spatial.nsw.gov.au).
