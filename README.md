# The Pookies List

A shared list for two: movies and TV to watch, Copenhagen restaurants to try, date ideas, and upcoming plans.

- Hosted on GitHub Pages (`index.html`, no build step).
- Data lives in Supabase (table `items`). Rows are only readable and writable with the private list key, which each phone gets once from the private link and keeps in local storage.
- Movie posters and info come from Apple iTunes Search, TV from TVmaze, and restaurants from OpenStreetMap. None of them need API keys.
