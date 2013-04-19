world-geometry
==============

I keep needing this data, so rather than trawling through old project files and copying it each time, I'm putting it here.

## [geometry.json](linktogohere)

This file contains SVG path definitions for 221 countries, indexed by their World Bank alpha-3 code. It uses a Robinson projection (Guardian house style for world maps), with a nominal width of 1000 and a height of 507 (Robinson projections always have this ratio).

The original data is sourced from [Natural Earth](http://www.naturalearthdata.com/) - it is a composite of the 10m, 50m and 110m layers (it prefers 110m resolution, but falls back to 50m or 10m if a particular country does not exist at a courser resolution). The data has been compressed by eliminating sub-pixel detail below a certain threshold. This is ideal for most visulations - it appears highly detailed when zoomed out, but is small enough to a) download quickly and b) allow smooth panning/zooming etc.


## [centroids.json](linktogohere)

This file contains hand-adjusted country centroids whose coordinates correspond to the projection in geometry.json.