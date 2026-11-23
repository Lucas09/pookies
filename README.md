# The Pookies List

A shared list for two: movies and TV to watch, Copenhagen restaurants to try, date ideas, and upcoming plans.

- Hosted on GitHub Pages (`index.html`, no build step).
- Data lives in Supabase (table `items`). Rows are only readable and writable with the private list key, which each phone gets once from the private link and keeps in local storage.
- Movie posters and info come from Apple iTunes Search, TV from TVmaze, and places from OpenStreetMap (Nominatim first, Overpass with mirror fallbacks). None of them need API keys.
- Travel: destinations are rows with `kind = 'trip'`; restaurants, sights, activities and stays saved inside a destination are rows with `kind = 'tripitem'` and `data.trip` set to the destination's id. Place search uses OpenStreetMap (Nominatim to find the destination, Overpass for places nearby). No new tables needed.
