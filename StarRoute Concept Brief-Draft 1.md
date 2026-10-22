
# StarRoute Concept Brief

## Overview
StarRoute is an API that answers questions about stars using public astronomical data. It returns the distance between two stars and plots a theoretical route between them, including the travel time at a chosen speed and notable objects along the way, such as black holes and nebulae. It gives writers and game designers realistic distances and travel times without requiring them to do the astronomy themselves.

Star data comes from the Gaia catalog, which is published by the European Space Agency.

## Target Users
StarRoute is aimed at creators looking for believable astronomical data, such as science fiction writers and game developers. It may also interest hobbyists, astronomers, and content creators.

## Key Features

### Route Planning
Given two stars and a travel speed, StarRoute returns the travel time, a theoretical route, and any hazards or points of interest along the way.

- Example query: "How long would it take to get from the Sun to Alpha Centauri at 0.8 times the speed of light?"
- Example response: a JSON file containing the travel time, route, and points of interest along the way.

### Star Identification
If given a star's catalog designation (such as HD 172167), StarRoute returns its common name and galactic coordinates, if known.

- Example query: "What is the name and position of the star HD 172167?"
- Example response:
  "name": "Vega",
  "galactic_longitude": 67.45,
  "galactic_latitude": 19.24

### Star Search
Given a star or a galactic coordinate, StarRoute returns a list of nearby stars (up to 1,000 in V1).

## Explicitly Out of Scope for V1
- Filtering by star type (for example, red dwarfs). V1 returns a general list of nearby stars only.
Routes that extend beyond the mapped region.
- Estimating the positions of stars with unknown locations. If a star's location isn't in the source data, StarRoute can't plot a route to or through it.

## Open Questions

- StarRoute's visual interface is undecided. The API will return text-only responses, but they could be used to populate a graphic, such as a split-screen view.

- Points-of-interest data source. Star catalogs like Gaia only contain the locations of stars. Objects such as black holes and nebulae may require a second data source.
