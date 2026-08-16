# Indy Crash Map

## Live links
- https://picturedigits.github.io/indy-crash-map

Interactive map of serious crashes involving vulnerable roadway users (pedestrians and cyclists) and motorists for Indianapolis, Indiana. Python notebook (`data/GetIndyCrashData.ipynb`) downloads and cleans data from a public dashboard in CSV format, which LeafletJS code displays as heatmap clusters or symbol map points.

## Credits

Map design by [Jack Dougherty](https://jackdougherty.org) and [Ilya Ilyankou](https://ilyankou.com) at [Picturedigits Ltd](https://www.picturedigits.com) in collaboration with [Central Indiana Cycling](https://centralincycling.org/) and [BCU Labs](https://labs.bostoncyclistsunion.org) of the [Boston Cyclists Union](https://bostoncyclistsunion.org)

## Map
- Zooming in automatically shifts display from broad heatmap clusters to street-level symbol points
- Mobile-first design works both on smaller screens (click arrow to expand legend on smartphone) and larger screens
- Copy browser link to share your view of the map (location, zoom level, data layer) with others
- Filter by crash type (involving pedestrians, cyclists & micromobility users, other vulnerable users, or motorists only)
- Filter by date range (2021 onward), severity (with fatalities, or with any injury), and interstate highway (inferred from the crash's street address, so may be inaccurate)
- Click symbol points for popup info about specific crashes

### Run map on your local computer
- Requires python3
- Clone (download) repo from GitHub and serve it as a static site, then open `index.html`.
- Example: type in your terminal:
```bash
python3 -m http.server 8000
```
- Then visit `http://localhost:8000`.
- Note: alternatively, just double-click the HTML file to open in your browser, but it will only work if the CSV is located on a remote server, not a local file.

## License

GNU General Public License v3.0
