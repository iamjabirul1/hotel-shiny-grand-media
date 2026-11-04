# hotel-shiny-grand-media

Public image host for the Hotel Shiny Grand social pipeline.

Instagram's Graph API fetches an image from a URL it can reach without
credentials, and the pipeline repository is private, so the photos it publishes
live here instead.

- `library/<name>-ig.jpg` are 1080x1350 (4:5) centre crops, the format Instagram
  asks for.
- Only marketing photos the hotel already publishes on its own Facebook page and
  website belong here. No tokens, no queue files, no internal state.

Serve pattern:

    https://raw.githubusercontent.com/iamjabirul1/hotel-shiny-grand-media/main/library/<name>-ig.jpg

The pipeline reads the base URL from the repository variable `IG_IMAGE_BASE`.
